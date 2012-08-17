---
layout: post
title: "Hacking On HTML5"
date: 2012-08-17 09:58
comments: true
categories: 
author: Chris
published: true
---

This is the third in a series of articles which outline the development of <a href="http://atomicbrawl.com">Atomic Brawl</a>. Check out the previous post <a href="/blog/2012/08/05/born-from-cardboard/">here</a>.

### Choosing Our Tech

We knew roughly what we were building by through the <a href="/blog/2012/08/05/born-from-cardboard/">prototyping</a> we had done prior. Coders at heart we moved onto the always fun task of choosing what technology to use on the front-end. <!-- more -->

We decided to use Javascript and HTML for a variety of reasons: 

- We wanted something that would work both on mobile devices and PCs.
- Our graphical requirements were quite simple, we know we could hit our targets within the boundaries of HTML.

So with that, we dug in and started to figure out how we could do this. Our first step was toying with the [HTML5's](http://en.wikipedia.org/wiki/HTML5) new [Canvas](http://en.wikipedia.org/wiki/Canvas_element) element.

### Stepping Into Canvas

Canvas is quite simple to use for anyone who has used similar tech. The API is familiar, and while there are quirks, our initial impressions were positive. Our first goal was simple: Using Canvas, layout a hexagon based grid with click detection:

<a href="http://shorrockin.com/atomic-brawl-tech-demos/2-isometric-math/index.html"><img src="/images/hacking_with_html/hex_grid.png" /></a>

You can play with this [here](http://shorrockin.com/atomic-brawl-tech-demos/2-isometric-math/index.html) (with [source](https://github.com/shorrockin/atomic-brawl-tech-demos/tree/master/2-isometric-math)). Click to add or remove tiles.

In very little time we had our grid laid out. While ugly - it proved that it could be done pretty simply. Our next proof of concept was to see how difficult it was to animate things. 

### Moving, Moving, Moving

As we started adding animation we felt the need to wrap this all up in a nice clean framework. While there are quite a few to choose from these days, at the time, there wasn't. We started to put together something that would:

- Take care of efficiently redrawing things.
- Allow us to efficiently animate things on a board.
- Provide us a reusable system of components that would could quickly use going forward.

With that, we came up with:

<a href="http://shorrockin.com/atomic-brawl-tech-demos/8-animation/index.html"><img src="/images/hacking_with_html/animation.png" /></a>

Like the previous example you can play with this one [here](http://shorrockin.com/atomic-brawl-tech-demos/8-animation/index.html) (with [source](https://github.com/shorrockin/atomic-brawl-tech-demos/tree/master/8-animation)). Click on a hexagon to add or remove it, and click on the stationary guy to move him around the board. He will choose the most efficient route given the current state of the board.

This is by no means production quality code but it does achieve a few things:

- Outlines techniques on how you can animate with dirty region detection, that is, not redrawing the whole screen on every animation frame.
- Shows how to do [A* Pathfinding](http://en.wikipedia.org/wiki/A*_search_algorithm) on a hexagon grid.
- Proves you can get very reasonable frame-rates for simple animations.

Now sadly, that last statement was only partially true. One of our reasons for going with HTML was that we wanted to ensure that everything ran well on mobile devices as well. When we wrote this (last year) we couldn't squeeze out more than 15 FPS on a first generation iPad. 

Most of this time was spent in clearing and redrawing, especially when semi-opaque images were involved. One technique we didn't experiment with at the time, which may of helped, was using multiple Canvases to represent the different layers.

Regardless, after some time, this lead us to re-evaluate how we were doing things. Perhaps we didn't even need Canvas?

### Moving To CSS3

<a href="http://atomicbrawl.com">Atomic Brawl</a> is not a title that relies on graphical sophistication. We started to wonder if we could do what we needed with just HTML utilizing [CSS3](http://www.css3.info/) to animate when needed. It took us about a week to re-write the core abstraction layer to use HTML instead of Canvas and the performance benefits were dramatic. 

At this point, there was no compelling reason to Canvas. We could achieve all the animations we needed without it, and had great performance. 

You can check-out the resulting CSS3 based animation by checking out our [Tutorial](http://atomicbrawl.com/tutorial).

### TL;DR

We decided to prototype using HTML5, specifically, Canvas. It ran well and did everything we needed to. Performance on mobile devices was sadly, not up to par. Using straight HTML with CSS3, we were able to achieve the same visual results with great performance on mobile. 

 









