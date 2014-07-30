## nlfcampus.github.io

The website for the New Life Fellowship (campus group) of the
[Twin City Chinese Christian Church](http://www.tcccc.org/). Welcome
to visit the website and join us to seek the **truth of life** through
**Jesus Christ**.

## Quick start to making contributions 

### Prerequisites

Make sure you have installed the following software on your local
machine:
- Git
- Ruby
- Jekyll

### Run the website on your local machine

```
$ git clone https://github.com/NLFCampus/NLFCampus.github.io.git
$ cd NLFCampus.github.io
$ jekyll serve --watch`
```

There you go! Launch a browser and visit <http://localhost:4000/> and view
your local copy of the website. Jekyll will monitor any changes you
made to the code so just refresh the page to see your modifications.

## Adding a post

The file name of the post should strictly be:
`yyyy-mm-dd-some-title.md`, for example:
*2014-07-28-about-website.md*.

The file is in [Markdown format](http://daringfireball.net/projects/markdown/).

The post should have the following layout:

```
---
layout: post
title: "关于团契网站以及我的一点想法"
description: ""
author: "杨硕"
category: 团契事工
tags: [网站，事工]
---
{% include JB/setup %}

copy and paste the content here.
```

Please refer to
[here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
for more Markdown syntax that is supported by Github.

## Where and How

### where and how to adjust the paramters for the image slider 

`themes/2/js-image-slider.js`

{% highlight js %}

  var sliderOptions=
    {
	sliderId: "slider",
	startSlide: 0,
	effect: "1,4,5,6,7,8,9,12,13,14,15,17",
	effectRandom: true,
	pauseTime: 3000,
	transitionTime: 500,
	slices: 11,
	boxes: 7,
	hoverPause: 2,
	autoAdvance: true,
	captionOpacity: 0.5,
	captionEffect: "rotate",
	thumbnailsWrapperId: "thumbs",
	m: false,
	license: "b6t80"
    };
	
{% endhighlight %}

all the parameters can be adjusted here.

### where to put posts

`_posts`

### where to modify the template of the website

`_includes/themes/the-minimum/`

### where to modify the layout of the website

`assets/themes/the-minimum/css/style.css`

### where to put the images

`images`
