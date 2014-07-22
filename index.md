---
layout: page
title: Welcome to New Life Fellowship!
tagline: Supporting tagline
---
{% include JB/setup %}

<head>
    <link href="themes/2/js-image-slider.css" rel="stylesheet" type="text/css" />
    <script src="themes/2/js-image-slider.js" type="text/javascript"></script>
</head>

<div id="sliderFrame">
  <div id="slider">
    <a href="http://www.menucool.com/jquery-slider" target="_blank">
      <img src="images/chrismas.jpg" alt="Welcome to jQuery Slider" />
    </a>
    <a class="lazyImage" href="images/image-slider-2.jpg" title="Pure Javascript. No jQuery. No Flash.">Pure JavaScript</a>
    <a href="http://www.menucool.com/javascript-image-slider"><b data-src="images/image-slider-3.jpg">Image Slider</b></a>
    <a class="lazyImage" href="images/image-slider-4.jpg" title="">Slide 4</a>
  </div>
  <!--thumbnails-->
  <div id="thumbs">
    <div class="thumb">
      <div class="frame"><img src="images/thumb1.jpg" /></div>
      <div class="thumb-content"><p>HTML Content</p>Thumbnails allows any HTML content</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/thumb2.jpg" /></div>
      <div class="thumb-content"><p>Customizable</p>Thumbnail style is customizable</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/thumb3.jpg" /></div>
      <div class="thumb-content"><p>Variety of Layouts</p>Just a CSS tweak.</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/thumb4.jpg" /></div>
      <div class="thumb-content"><p>Integration</p>Built-in functions for the thumbnails</div>
      <div style="clear:both;"></div>
    </div>
  </div>
  <!--clear above float:left elements. It is required if above #slider is styled as float:left. -->
  <div style="clear:both;height:0;"></div>
  </br>
</div>


###Latest Posts

<ul class="posts">
  {% for post in site.posts limit: 1 %}
  <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  <span> - {{ post.author }}</span></li>
  {% endfor %}
</ul>
