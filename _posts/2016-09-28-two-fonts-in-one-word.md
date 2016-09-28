---
layout: post
title: "How to use two fonts in one HTLM tag"
date: 2016-09-28
---

<link rel="stylesheet" type="text/css" href="/css/two-fonts-experiment.css">


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


See <a target="_blank" href="https://vimeo.com/101718785">source video</a>

