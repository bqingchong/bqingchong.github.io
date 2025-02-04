---
layout: post
title:  Handouts
date:   
categories: jekyll update
---

<style>
.password {
  --svg-color: #808390;
  --text-color: #414856;
  --weak-color: #F04545;
  --medium-color: #FFA850;
  --strong-color: #47C796;
  --width: 180px;
  --height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  input {
    background: none;
    border: 0;
    outline: none;
    width: 22px;
    height: var(--height);
    z-index: 1;
    position: relative;
    appearance: none;
    transition: all .6s ease-out;
    cursor: pointer;
    color: var(--text-color);
    font: 400 14px 'Poppins', sans-serif;
  }
  .check {
    display: none;
    width: var(--height);
    height: var(--height);
    padding: 5px 2px 5px 8px;
    box-sizing: border-box;
    position: absolute;
    right: 0;
    z-index: 3;
    cursor: pointer;
    svg {
      fill: none;
      stroke: var(--strong-color);
      stroke-width: 2px;
      stroke-linecap: round;
      stroke-linejoin: round;
      stroke-dashoffset: 26;
      stroke-dasharray: 26;
      transition: stroke-dashoffset .6s ease;
    }
  }
  .lock {
    width: 180px;
    height: var(--height);
    position: absolute;
    right: 0;
    &::before,
    &::after {
      content: "";
      position: absolute;
      background: var(--svg-color);
      pointer-events: none;
    }
    &::before {
      right: 8px;
      bottom: 9px;
      width: 6px;
      height: 6px;
      border-radius: 50%;
      transition: bottom .2s ease-out .4s, right .4s ease-out;
    }
    &::after {
      right: 10px;
      bottom: 5px;
      width: 2px;
      height: 10px;
      border-radius: 2px;
      transition: bottom .4s ease-out .4s, border-radius .2s ease-out .4s, width .2s ease-out .4s, right .4s ease-out, height .4s ease .8s;
    }
    svg {
      display: block;
      height: 100%;
      width: 100%;
      fill: none;
      stroke: var(--svg-color);
      stroke-width: 2px;
      stroke-linecap: round;
      stroke-linejoin: round;
      stroke-dashoffset: 263;
      stroke-dasharray: 0 263 71 263;
      transition: all .6s ease-out;
    }
  }
  &.active {
    input {
      width: var(--width);
      padding: 0 var(--height) 0 5px;
      cursor: text;
      box-sizing: border-box;
    }
    .check {
      display: flex;
      &.submit {
        svg {
          stroke-dashoffset: 0;
          stroke-dasharray: 26;
        }
        & ~ .lock {
          &::before,
          &::after {
            opacity: 0;
            right: 9px;
            transition: right .2s ease-out, opacity .2s ease-out;
          }
        }
      }
      &.active {
        & ~ .lock {
          &::before {
            animation: wink-animation .6s linear alternate;
            background: var(--medium-color);
          }
          &::after {
            animation: wink-animation .6s linear alternate;
            background: var(--medium-color);
          }
        }
      }
    }
    .lock {
      &::before {
        right: 3px;
        bottom: 11px;
        transition: bottom .1s ease-out .1s, right .4s ease-out .2s, background .2s ease-out, opacity .2s ease-out;
      }
      &::after {
        right: 15px;
        bottom: 11px;
        width: 6px;
        height: 6px;
        border-radius: 50%;
        transition: height .2s ease-out, bottom .2s ease-out, border-radius .2s ease-out .2s, width .2s ease-out .2s, right .4s ease-out .2s, background .2s ease-out, opacity .2s ease-out;
      }
      svg {
        stroke-dashoffset: 207;
        stroke-dasharray: 0 263 177 263;
      }
    }
    .indicator {
      width: 180px;
      height: var(--height);
      position: absolute;
      right: 0;
      &::before {
        content: "";
        position: absolute;
        left: 0;
        bottom: 0;
        width: 0;
        height: 2px;
        border-radius: 5px;
        background: transparent;
        z-index: 3;
        transition: background .6s ease-out, width .6s ease-out;
      }
      &.weak {
        &::before {
          width: 33.3%;
          background: var(--weak-color);
        }
      }
      &.medium {
        &::before {
          width: 66.6%;
          background: var(--medium-color);
        }
      }
      &.strong {
        &::before {
          width: 100%;
          background: var(--strong-color);
        }
      }
    }
  }
}

@keyframes wink-animation {
  0% {
    height: 6px;
  }
  10% {
    height: 1px;
  }
  20% {
    height: 6px;
  }
  80% {
    height: 6px;
  }
  90% {
    height: 1px;
  }
  100% {
    height: 6px;
  }
}

//--- ## BASIC #############
body {
  background: #E8EBF3;
  height: 100vh;
  font: 400 16px 'Poppins', sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  .socials {
    position: fixed;
    display: block;
    left: 20px;
    bottom: 20px;
    > a {
      display: block;
      width: 30px;
      opacity: var(--opacity, .2);
      transform: scale(var(--scale, .8));
      transition: transform .3s cubic-bezier(0.38,-0.12, 0.24, 1.91);
      &:hover {
        --scale: 1;
      }
    }
  }
}
</style>

<style>
a:link, a:visited{
  color: black;
  text-decoration: none;
}
a:hover {
  color: orange;
  text-decoration: none;
}
a:active {
    color: red !important;
}
</style>

<head>
    <br />
    <h2 style="font-family:Verdana">
        Hua Lo Geng Training Handouts
    </h2>
    <p style="font-family:Verdana"> These are some of the handouts I prepared to train for the Hua Lo Geng Cup.</p>
</head>
<br />
<body>
    <ul>
        <li><a href="~/css/HLG Lecture/A1Series.pdf"> Lecture 1: Series Computation </a></li>
        <li> Lecture 2: Linear Diophantine Equations</li>
    </ul>
</body>
<br />
<hr />
<br />
<head>
    <h2 style="font-family:Verdana">
        Physics Week Challenge
    </h2>
    <p style="font-family:Verdana">
        This is a project to introduce new topics in physics. For any chosen week, three problems will be posted daily on a given theme. These problems are at introductory levels only.
    </p>
    <br />
    <h3>Week 1: Circuit Analysis</h3>
    <ul>
        <li><a href="/main_pages/PWC/W1D1.html">Parallel and Series Circuits</a></li>
        <li><a href="/main_pages/PWC/W1D2.html">Ammeters and Voltmeters</a></li>
        <li><a href="/main_pages/PWC/W1D3.html">Kirchhoff's Laws</a></li>
        <li><a href="/main_pages/PWC/W1D4.html">Exploiting Equipotential Points</a></li>
        <li><a href="/main_pages/PWC/W1D5.html">RLC Circuits</a></li>
        <li><a href="/main_pages/PWC/W1D6.html">Star-Delta Transformation</a></li>
        <li><a href="/main_pages/PWC/W1D7.html">Thevenin's Theorem and Norton's Theorem</a></li>
    </ul>
    <br />
    <h3>Week 2: ????????</h3>
    <ul>
        <li><a asp-controller="PWC" asp-action="" ></a>?????_?</li>
        <li><a asp-controller="PWC" asp-action="" ></a>???_??</li>
        <li><a asp-controller="PWC" asp-action="" ></a>?????_???</li>
        <li><a asp-controller="PWC" asp-action="" ></a>??????_???_?</li>
        <li><a asp-controller="PWC" asp-action="" ></a>?_???</li>
        <li><a asp-controller="PWC" asp-action="" ></a>???__?_</li>
        <li><a asp-controller="PWC" asp-action="" ></a>??_</li>
    </ul>
    <br />
    <hr />
    <br />
    <h2 style="font-family:Verdana">
        UEC Preparation Notes
    </h2>
    <br />
    <hr />
    <br />
    <h2 style="font-family:Verdana">
        Mock Papers
    </h2>
    <br />
    <ul>
        <li><a href="/main_pages/Files/Mock CJR2024.pdf" > Mock CJR Cup 2024 </a></li>
        <li><a href="/main_pages/Files/Mock_HLG_2024.pdf" > Mock HLG Cup 2024 </a></li>
        <li><a style="color:black"> Mock CJR Cup 2025 </a></li>
        <li><a style="color:black"> Mock HLG Cup 2025 </a></li>
        <li><a style="color:black"> Self-Hosted Codeforces Educational Round </a></li>
    </ul>
    <br />
    <hr />
    <br />
    <h2 style="font-family:Verdana">
        More Notes
    </h2>
    <br />
    <h3> 
        Enter password to access
    </h3> 
</head>
