---
layout: post
title: "Effortless Style by Heydon Pickering"
date: 2016-09-28
---

<link rel="stylesheet" type="text/css" href="/css/two-fonts-experiment.css">


<p>These are my notes from video tutorial <a href="https://vimeo.com/101718785">"Effortless Style"</a> by Heydon Pickering on Vimeo</p>

<h2 class="experiment">Experiment & fun</h2>

<p>This is my quick experiment to check how we can use two fonts in one tag - without any additional tags like SPAN</p>

<div class="example">
	<p class="example-header">Examples of Base rules</p>
	<div class="example-body">
{% highlight css %}@import url('https://fonts.googleapis.com/css?family=Indie+Flower');
@import url('https://fonts.googleapis.com/css?family=Lobster&text=%26');


.experiment{
	font-family: Lobster, 'Indie Flower';
}{% endhighlight %}
	</div>
</div>

<p class="sassmeister" data-gist-id="dbbdf12e4af675e6dde6d98838f4fb0a" data-height="580" data-theme="monokai"><a href="http://sassmeister.com/gist/dbbdf12e4af675e6dde6d98838f4fb0a">Play with this gist on SassMeister.</a></p><script src="http://cdn.sassmeister.com/js/embed.js" async></script>


