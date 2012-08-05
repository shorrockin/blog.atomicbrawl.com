---
layout: post
title: "Born From Cardboard"
date: 2012-08-05 10:43
comments: true
author: Chris
categories: 
---

This is the second in a series of articles which outline the development of <a href="http://atomicbrawl.com">Atomic Brawl</a>. 
Check out the first post <a href="/blog/2012/08/03/who-we-are/">here</a>.

### Digital Paper

Our target for the game was simple - create something fun. Too often games, especially those played in browser, are just thinly
veiled compulsion loops that prey on very basic mental hooks. We wanted to focus on creating a fun core game experience first, 
and then build on that solid foundation. To do so, we started making a playable non-digital version of, what we were calling at 
the time, 'Villainy'.

<!-- more -->

### Core Focus

We had a vague idea of what we wanted Villainy to be. We wanted an online collectible card game, that took advantage of the 
digital medium by having complex interactions between the pieces in play. Said another way, we wanted the fun and design sensibilities
of an offline physical game that could be played through the convenience of online. It only made sense that we started prototyping 
with pen and page. 


### Version 0

The very first iteration of the game was lane based:

<img src="/images/born_from_cardboard/board.png" />

In each lane you could play a 'Unit' (now called Brawler) which would have to stick to that lane. Our original inspiration on this
concept was from envisioning a collectable multiplayer <a href="http://www.popcap.com/games/plants-vs-zombies/online">Plants vs Zombies</a>.

We had the concept of 'Avatars' (now called Cores), which represented your team of characters. These avatars would have some 
unique abilities which globally effected the game and would be the basis for your team. As it is now, the concept of the game at
this stage was to destroy your opponents avatar.

We then had a few different card template that we used to construct a variety of different cards that we could play with:

<img src="/images/born_from_cardboard/cards.png" />

All the cards types in this version are all still in the game today. The only addition was 'Structures' which are essentially 
immobile Brawlers. The templates here are super flexible, and we printed off a sack of em and created about 50 different types 
of cards that we could used with our ever shifting rule-set.


### Beers, Pizza and Rule Changes

The hardest part of this stage of development was tweaking and tuning the rules, or the 'fun' factor. Eventually we bribed
some friends to come over for a night of beer, pizza and Villainy to help us in this. We played a lot of games, and toyed around
with tons of different facets of the game. Here's a short list of core choices we made to help shape the game today:

#### Lane Based Movement

As I mentioned earlier, in this version of the game you played a unit and it moved forward and attacked according to some rules
we had defined. Our problem with this was that you could almost never react to your opponent reacting to you, as once a unit was
played it was out of your control. We couldn't decide if the game was about your macro decisions, in deck construction and high 
lane choices, or micro decisions - carefully choosing who attacks whom, who moves where, etc. In the end, we decided a more tactics
like experience was a more enganging choice.

#### Real Time vs. Async

We toyed around with a real time versus asynchronous gameplay. While real time is fun, asynchronous gameplay was something that
we knew would attract more people, like ourselves, who have full-time jobs and don't often have the ability to sit down and 
play through a full game. 

#### Attack Patterns

One huge difference between this and what we have now is the concept of attack and effect patterns. This was something that I was
first drawn to in <a href="http://en.wikipedia.org/wiki/Phantasy_Star_Online_Episode_III:_C.A.R.D._Revolution">Phantasy Star Online Episode III: C.A.R.D Revolution</a> 
(that name is out of control). Attack patterns forced you to really consider your positional strategy, and in a lane based game it had a 
large impact on which lane you choose to play various cards. This was dropped for 2 reasons. The first was thas it was mentally
challenging to forcast how patterns would impact the game. The second was that from a UI standpoint it was difficult to do this 
on a hex based grid (something we obviously decided on after the prototype).


### TL;DR

We want to make a game. We made a paper prototype. This helped us think about what we were attempting to make. Our original
concept shifting from a macro-oriented multiplayer tower defense, to a micro-oriented multiplayer tactics game. Paper prototyping
helped us quickly and efficiently tune what we were building.

