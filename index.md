---
layout: page
title: Welcome to New Life Fellowship - Student Group!
tagline: Supporting tagline
---
{% include JB/setup %}

<head>
    <link href="themes/2/js-image-slider.css" rel="stylesheet" type="text/css" />
    <script src="themes/2/js-image-slider.js" type="text/javascript"></script>
</head>

<div id="sliderFrame">
  <div id="slider">
    <a href="https://www.facebook.com/groups/564531400284272/" target="_blank">
      <img src="images/christmas.jpg" alt="We are a group of Chinese students
	  around Twin-city-Minnesota seeking the truth of Jesus Christ." />
    </a>
    <a class="lazyImage" href="images/Jesus-Cross.jpg" title="Our faith">Our faith</a>
    <img src="images/bible-study.jpg" alt="#biblestudy" />
    <a class="lazyImage" href="images/image-slider-4.jpg" title="">Slide 4</a>
  </div>
  <div id="biblestudy" style="display: none;">
    Join our Weekly Bible Study @<a href="https://www.google.com/maps/place/1120+5th+St+SE,+Minneapolis,+MN+55414/@44.9824569,-93.238446,17z/dat\
  a=!3m1!4b1!4m2!3m1!1s0x52b32d0d867d49b7:0xfb1c35546f49c8f6?hl=en">CRU House</a>. Need a ride? Feel free to email to nlf.campus@gmail.com or contact Yang Shuo @ 952-297-6289
  </div>
  <!--thumbnails-->
  <div id="thumbs">
    <div class="thumb">
      <div class="frame"><img src="images/christmas-thumb.jpg" /></div>
      <div class="thumb-content"><p>Who are we?</p>Young Chinese Christians - most of us are students</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/Jesus-Cross-thumb.jpg" /></div>
      <div class="thumb-content"><p>What we believe?</p>Our faith lies in the resurrection of Jesus Christ</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/bible-study-thumb.jpg" /></div>
      <div class="thumb-content"><p>Weekly Bible Study - Join us!</p>Let us study His words together!</div>
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
  {% for post in site.posts limit: 5 %}
  <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  <span> - {{ post.author }}</span></li>
  {% endfor %}
</ul>
