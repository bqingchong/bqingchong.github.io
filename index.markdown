---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

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

<script>
  var hello = ['Ohayo!', '你好！', 'Hola!', 'Xin chào!', 'สวัสดี!', 'Bonjour!', 'नमस्ते!', 'こんにちは!', 'Ciao!', 'வணக்கம்!', '안녕하세요!', 'привет!', 'ہیلو!'];

  function swap(){
    var x = document.getElementById("thello");
    if (x.innerHTML == 'Ohayo!') {
      x.innerHTML = '你好！';
    } else if (x.innerHTML == '你好！') {
      x.innerHTML = 'Hola!';
    } else if (x.innerHTML == 'Hola!') {
      x.innerHTML = 'Xin chào!';
    } else if (x.innerHTML == 'Xin chào!') {
      x.innerHTML = 'สวัสดี!';
    } else if (x.innerHTML == 'สวัสดี!') {
      x.innerHTML = 'Bonjour!';
    } else if (x.innerHTML == 'Bonjour!') {
      x.innerHTML = 'नमस्ते!';
    } else if (x.innerHTML == 'नमस्ते!') {
      x.innerHTML = 'こんにちは!';
    } else if (x.innerHTML == 'こんにちは!') {
      x.innerHTML = 'Ciao!';
    } else if (x.innerHTML == 'Ciao!') {
      x.innerHTML = 'வணக்கம்!';
    } else if (x.innerHTML == 'வணக்கம்!') {
      x.innerHTML = '안녕하세요!';
    } else if (x.innerHTML == '안녕하세요!') {
      x.innerHTML = 'привет!';
    } else if (x.innerHTML == 'привет!') {
      x.innerHTML = 'ہیلو!';
    } else if (x.innerHTML == 'ہیلو!') {
      x.innerHTML = 'Ohayo!';
    }
  }
</script>

<head>
<h1>
  <span style="color:darkgreen" onmouseover="swap()" id="thello">Ohayo!</span> Welcome to my blog!
</h1>
</head>


<body>
<br />
<p style="font-size:larger">
    I will be sharing my notes and other information in this blog.
</p>
<hr />
<br />
<a href="/main_pages/Handouts.html" style="font-family:Verdana;font-size:large" >Handouts and Notes</a>
<p>
    These are some of my handouts and notes which I've used to train my juniors. You may click the title to obtain the resources. 
</p>
<br />
<hr />
<br />
<a href="/main_pages/Articles.html" style="font-family:Verdana;font-size:large">Articles</a>
<p>
    Explore articles on contest preps and interesting math facts!
</p>
<br />
<hr />
<br />
<a href="/main_pages/Projects.html" style="font-family:Verdana;font-size:large;text-decoration:none">Projects</a>
<p>
    Browse throught my recent projects and feel free to contribute!
</p>
<br />

</body>
