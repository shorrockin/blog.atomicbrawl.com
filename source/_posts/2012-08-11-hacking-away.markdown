---
layout: post
title: "Hacking Away"
date: 2012-08-11 09:58
comments: true
categories: 
author: Chris
---

This is the third in a series of articles which outline the development of <a href="http://atomicbrawl.com">Atomic Brawl</a>. Check out the previous post <a href="/blog/2012/08/05/born-from-cardboard/">here</a>.

### HTML5! I Choose You!

We knew roughly what we were building by all the <a href="/blog/2012/08/05/born-from-cardboard/">prototyping</a> we had done prior. Programmers at heart we next moved onto the always fun task of choosing what technology to use on the front-end. We eventually went javascript and HTML for a variety of reasons: <!-- more -->

- Our graphical desires at the time were fairly simple. We knew we could achieve what we wanted using straight HTML.
- HTML gives us the flexibility of developing once and being able to play on both PCs as well as mobile devices.
- While not super experienced in Javascript (at that time) it was a fairly simple but seemingly powerful language who's performance was not the dog it once was.

### First Steps

Our first steps were to determine if we could produce a hex based game board using HTML. We also wanted to assess the performance of HTML5 canvas to see what it could handle. Our very first prototype is included below:

<script data-main="/assets/hacking_away/scripts/main.js" src="/assets/hacking_away/scripts/require.js">
</script>

<canvas width="100%" height="300" id="canvas">Your browser doesn't support Canvas YO!</canvas>
<form>
<input id="lock_fps" type="checkbox" checked>Lock FPS</input> / 
<input id="run_animation" type="checkbox" checked>Run Animation Loop</input> / 
<input id="enable_dirty" type="checkbox">Enable Dirty Regions</input> / 
<input id="add_dude" type="button" value="Add Dude"></input> / 
<br>
FPS: <span id="current_fps">N/A</span> (last 10 frames)
</form>



