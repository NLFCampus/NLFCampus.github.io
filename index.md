---
layout: page
title:   
tagline: Supporting tagline
---
{% include JB/setup %}

<head>
    <link href="themes/2/js-image-slider.css" rel="stylesheet" type="text/css" />
    <script src="themes/2/js-image-slider.js" type="text/javascript"></script>
</head>

<div id="fb-root"></div>
<script>(function(d, s, id) {
   var js, fjs = d.getElementsByTagName(s)[0];
   if (d.getElementById(id)) return;
   js = d.createElement(s); js.id = id;
   js.src = "//connect.facebook.net/en_US/sdk.js#xfbml=1&appId=286591694835592&version=v2.0";
   fjs.parentNode.insertBefore(js, fjs);
 }(document, 'script', 'facebook-jssdk'));</script>

<div id="sliderFrame">
  <div id="slider">
    <a href="https://www.facebook.com/groups/564531400284272/" target="_blank">
      <img src="images/slider-1-about-us.jpg" alt="" />
    </a>
    <a class="lazyImage" href="images/slider-2-bible-study.jpg" title="">Bible Study</a>
    <a href="http://www.tcccc.org/zh-hant/sermon_mand" target="_blank">
      <img src="images/sermon2.jpg" alt="请点击图片进入讲道" />
    </a>
    <a class="lazyImage" href="images/weekly-verse.jpg" title="">Slide 4</a>
    <a class="lazyImage" href="images/prayer.jpg" title="">Slide 5</a>
  </div>
  <div id="biblestudy" style="display: none;">
    Join our Weekly Bible Study @<a href="https://www.google.com/maps/place/1120+5th+St+SE,+Minneapolis,+MN+55414/@44.9824569,-93.238446,17z/dat\
  a=!3m1!4b1!4m2!3m1!1s0x52b32d0d867d49b7:0xfb1c35546f49c8f6?hl=en">CRU House</a>. Need a ride? Feel free to email to nlf.campus@gmail.com or contact Yang Shuo @ 952-297-6289
  </div>

  <div id="sermon" style="display: none;">
    请点击<a href="http://www.tcccc.org/zh-hant/sermon_mand">这里</a>聆听马牧师的讲道
  </div>

  <!--thumbnails-->
  <div id="thumbs">
    <div class="thumb">
      <div class="frame"><img src="images/christmas-thumb.jpg" /></div>
      <div class="thumb-content"><p>关于我们</p>我们是由明尼苏达双城地区的中国基督徒学生学者组成的校园团契</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/Bible.jpg" /></div>
      <div class="thumb-content"><p>每周查经</p>欢迎和我们一起来学习神的话，了解这位创造宇宙万物的真神</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/listen-to-sermons.jpg" /></div>
      <div class="thumb-content"><p>轻轻听......</p>双城华人基督教会国语部马天岚牧师的讲道</div>
      <div style="clear:both;"></div>
    </div>
    <div class="thumb">
      <div class="frame"><img src="images/walking-with-god.jpg" /></div>
      <div class="thumb-content"><p>每周经文</p>在神的话语里我们与主同行</div>
      <div style="clear:both;"></div>
    </div>
	<div class="thumb">
	  <div class="frame"><img src="images/praying.jpg" /></div>
      <div class="thumb-content"><p>请聆听我们为你的祷告</p>先别走开......</div>
      <div style="clear:both;"></div>
    </div>
	
  </div>
  <!--clear above float:left elements. It is required if above #slider is styled as float:left. -->
  <div style="clear:both;height:0;"></div>
  </br>
</div>

<ul class="posts">
  {% for post in site.posts limit: 5 %}
  <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  <span> - {{ post.author }}</span></li>
  {% endfor %}
</ul>

<iframe src="//www.facebook.com/plugins/like.php?href=http%3A%2F%2Fnlfcampus.github.io%2F&amp;width&amp;layout=button_count&amp;action=like&amp;show_faces=true&amp;share=true&amp;height=21&amp;appId=286591694835592" scrolling="no" frameborder="0" style="border:none; overflow:hidden; height:21px;" allowTransparency="true"></iframe>
