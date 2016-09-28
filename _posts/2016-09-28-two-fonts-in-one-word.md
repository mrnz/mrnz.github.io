---
layout: post
title: "Effortless Style by Heydon Pickering"
date: 2016-09-28
---

<link rel="stylesheet" type="text/css" href="/css/two-fonts-experiment.css">


<p>These are my notes from video tutorial <a href="https://vimeo.com/101718785">"Effortless Style"</a> by Heydon Pickering on Vimeo</p>

<p>Two things were very interesting to me.</p>

<h2>First</h2>

<p>one is a wee experiment which shows that it is possible to use two fonts in one tag - without any additional tags like SPAN. 
See example below: </p>

<h2 class="experiment">Experiment & fun</h2>

<p>To achieve this effect we need to import google fonts. One of them with additional query parameter - "text". This makes that font deliver to us is just a subset, in this case it only contains one character. Then in the css we can use our normal font stack like this:</p>

<p>font-family: Lobster, 'Indie Flower'</p>

<p>This mainly means: render first font for everything what first font is able to render - this case only one chatracter "&" and then fallback for everything on second font. Of course, this stack can be longer. Here is the complete examples: </p>


<div class="example">
	<p class="example-header">Two fonts in one tag</p>
	<div class="example-body">
{% highlight css %}@import url('https://fonts.googleapis.com/css?family=Indie+Flower');
@import url('https://fonts.googleapis.com/css?family=Lobster&text=%26');

.experiment{
	font-family: Lobster, 'Indie Flower';
}{% endhighlight %}
	</div>
</div>

<h2>Second</h2>

<p>interesting thing is a way how we can us CSS without any classes or ID's. This is very important when we don't have control on HTML.
 Let's say that we have grid with fixed number of elements in a row which is 5. The problem with styling begins when the total number of elements in our grid is not evenly divisible by the fixed number of elements in a row and we want cover whole squer / grid. </p>
<style>
.ex-wrap{
	position: relative;
	width: 300px;
	height: 120px;
}
.ex-wrap div{
  position: relative;
  float: left;
  width: calc(100% / 5);
  height: calc(300px / 5);
  background: black;
  border: green 1px solid;
  box-sizing: border-box;
}
</style>
<div class="ex-wrap">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

  <p>How we can style this grid independently from this number which can change without our knowledge. The solution is brilliant and very informative</p>




<p class="sassmeister" data-gist-id="dbbdf12e4af675e6dde6d98838f4fb0a" data-height="480" data-theme="monokai"><a href="http://sassmeister.com/gist/dbbdf12e4af675e6dde6d98838f4fb0a">Play with this gist on SassMeister.</a></p><script src="http://cdn.sassmeister.com/js/embed.js" async></script>

<p>Play with this gist <a href="http://www.sassmeister.com/gist/dbbdf12e4af675e6dde6d98838f4fb0a">HERE</a> and delete or add divs inside .wrapper. You can also change SASS variable $cols and observe changes. That is COOL!</p>

