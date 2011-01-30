---
layout: post
title: Building iPhone Apps with HTML, CSS and Javascript
subtitle: By Jonathan Stark
summary: Recapping points Jonathan made so that I can use them more readily.
categories:
- iphone
- html5
---
### Chapter 01: Getting Started
* html
* css
* javascript

### Chapter 02: Basic iPhone Styling
* Set the viewport of the width of the device
* Create an iphone specific stylesheet
* Create iPhone style look and feel (CSS: titlebar, cells)
* Add jQuery for click logic
* Add images and CSS for nav button

<pre>&lt;meta name="viewport" content="user-scalable=no, width=device-width" /&gt;

&lt;link rel="stylesheet" href="/css/desktop.css" type="text/css" media="only screen and (min-width: 481px)" /&gt;
&lt;link rel="stylesheet" href="/css/iphone.css" type="text/css" media="only screen and (max-width: 480px)" /&gt;

#header {
	text-shadow: 0px 1px 0px #fff;
	-webkit-gradient(linear, left top, left bottom, from(#ccc), to(#999));
}

ul li:first-child a {
	-webkit-border-top-left-radius: 8px;
	-webkit-border-top-right-radius: 8px;
}

ul li:last-child a {
	-webkit-border-bottom-left-radius: 8px;
	-webkit-border-bottom-right-radius: 8px;
}
</pre>

### Chapter 03: Advanced iPhone Styling
* Replace content via Ajax
* Track history or the buttons
* Adding an icon
* Full screen mode
* Change the status bar
* Change the icons
* Custom startup graphic

<pre>&lt;meta name="apple-mobile-web-app-capable" content="yes" /&gt;
&lt;meta name="apple-mobile-web-app-status-bar-style" content="black" /&gt;

web-root/apple-touch-icon.png
&lt;link rel="apple-touch-icon"  href="custom-icon.png" /&gt;
&lt;link rel="apple-touch-icon-precomposed"  href="custom-icon-precomposed.png" /&gt;
&lt;link rel="apple-touch-startup-image"  href="custom-startup-graphic.png" /&gt;
</pre>
### Reference
* [Jonathan Stark's Blog](http://jonathanstark.com/blog/)
