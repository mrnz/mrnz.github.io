---
layout: post
title: "Effortless Style by Heydon Pickering"
date: 2016-09-28
---

<link rel="stylesheet" type="text/css" href="/css/two-fonts-experiment.css">


<p>These are my notes from video tutorial <a href="https://vimeo.com/101718785">"Effortless Style"</a> by Heydon Pickering on Vimeo</p>

<p>Two things ware very inreresting to me.</p>

<h2>First</h2>

<p>one is a wee experiment which shows that it is possible to use two fonts in one tag - without any additional tags like SPAN. 
See example below: </p>

<h2 class="experiment">Experiment & fun</h2>

<p>To achive this effect we need to import google fonts. One of them with additional query parameter - "text". This does that font deliver to us is just a subset, in this case it only contains one character. Then in css we can use our normal font stuck like that:</p>

<p>font-family: Lobster, 'Indie Flower'</p>

<p>This mainly means: render first font for everything what first font is able to render - this case only one chatracter "&" and then fallback for everything on second font. Of course, this stack can be longer. Here's a full example: </p>


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

<p>interesting thing is a way how we can us CSS without any classes or tags. This is very important when we don't have control on HTML.
 Let's say that we have grid with fixed number of elements in a row which is 5. Problem witch styling starts when a total number of elements is 9, 8, 7 or 6 and we want cover whole squer / grid. How we can style this grid independently from this number which can change without our knowledge. The solution is brilliant and very informative</p>

 
<p class="sassmeister" data-gist-id="dbbdf12e4af675e6dde6d98838f4fb0a" data-height="580" data-theme="monokai"><a href="http://sassmeister.com/gist/dbbdf12e4af675e6dde6d98838f4fb0a">Play with this gist on SassMeister.</a></p><script src="http://cdn.sassmeister.com/js/embed.js" async></script>


