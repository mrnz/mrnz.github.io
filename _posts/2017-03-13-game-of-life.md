---
layout: post
title: "Game of Life"
date: 2017-03-13
---

<link rel="stylesheet" type="text/css" href="/css/game-of-life.css">

<div id="game">
    <table id="grid"></table>
    <div id="info">
        Generation: <span id="generations"></span>
        Cells alive: <span id="alive"></span>
    </div>
    <div class="buttons">
        <button id="next" type="button" name="button" class="next"></button><!--
     --><label id="autoplay-label" for="autoplay" class="css-label">
             <input class="css-checkbox" id="autoplay" type="checkbox" name="autoplay" />
             Autoplay
        </label>
        <label id="speed-label" for="speed">
            Speed
            <input type="range" id="speed" min="10" max="1000">

        </label>
    </div>
</div>

<script type="text/javascript" src="/js/game-of-life.js"></script>




