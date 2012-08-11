---
layout: post
title: "Born From Cardboard"
date: 2012-08-05 10:43
comments: true
author: Chris
categories: 
---

This is the second in a series of articles which outline the development of <a href="http://atomicbrawl.com">Atomic Brawl</a>. Check out the previous post <a href="/blog/2012/08/03/who-we-are/">here</a>.

### Digital Paper

Our goal for the game was simple - create something fun. Too often games, _especially_ those played in the browser, are just thinly veiled compulsion loops that prey on human psychology to keep you clicking over and over, but aren't really all that enjoyable to play. We decided to focus on creating a fun core game experience first, and then build on that solid foundation. So we started developing playable paper prototypes of, what we were calling at the time, 'Villainy'.

<!-- more -->

### Focus

We had a vague idea of what we wanted Villainy to be. An online collectible card game that took advantage of the digital medium by having complex interactions between the pieces in play. Said another way, we wanted the fun and design sensibilities of an board or card game, that could be played through the convenience of online. It only made sense that we started prototyping with pen and page.


### Version 0

The very first iteration of the game was lane based:

<img src="/images/born_from_cardboard/board.png" />

In each lane you could play a 'Unit' (now called a Brawler) which would automatically start wandering down that lane and start attacking enemies. Our original inspiration for this concept was a collectable multiplayer <a href="http://www.popcap.com/games/plants-vs-zombies/online">Plants vs Zombies</a>, or kind of like multiplayer tower defence.

We had the concept of 'Avatars' (now called Cores), which represented your team of characters. These avatars had unique abilities that affected the game, and formed the basis of your team. Just like now, the goal of the game at this stage was to destroy your opponent's avatar.

Itching to try the game out, we created some templates for cards, printed off a stack of 'em and went crazy creating about 100 different of cards that we could used with our ever shifting rule-set.

<img src="/images/born_from_cardboard/cards.png" />

All the basic cards types in this version (Cores, Brawlers, Traps, Items)  are all still in the game today. The only addition since then has been 'Structures', which are essentially immobile Brawlers. The big thing that was dropped was the idea of "attack patterns", which were super cool but only really made sense when the Brawlers were on autopilot.


### Beer, Pizza, Rule Changes, And More Rule Changes

The hardest part of this stage of development was tweaking and tuning the rules, trying to find the fun factor. We bribed some friends to come over for a few nights of beer, pizza and play-testing to help us out. We played a boat-load of games, and toyed around with tons of different facets of the game mechanics. Here's a short list of core choices we made that shaped the game we have today:

#### The Death Of Automatic, Lane-Based Movement

As I mentioned earlier, in this version of the game you played a unit and it moved forward and attacked according a defined rate and pattern. The issue with this was that you could almost never react to what your opponent was doing (especially when they were reacting to what you were doing), as once a unit was played it was out of your control. We couldn't decide if the game was about your macro decisions, in deck construction and high lane choices, or micro decisions - carefully choosing who attacks whom, who moves where, etc. It was a _very_ tough call, but we decided a more tactics-like experience was more fun.

#### No More Attack Patterns

One huge difference between this and what we have now is the concept of attack and effect patterns. This was something that we were first drawn to in <a href="http://en.wikipedia.org/wiki/Phantasy_Star_Online_Episode_III:_C.A.R.D._Revolution">Phantasy Star Online Episode III: C.A.R.D Revolution</a> (that name is _out of control_). Attack patterns forced you to consider your positional strategy, and in a lane-based game it had a large impact on which lane you choose to play various cards. This was dropped for two reasons: It was really tough to forecast how patterns would impact the game, and from a UI standpoint it was difficult to do this on a hex based grid (something we decided on after the prototype).

#### Real-Time vs. Turn-Based Gameplay

We toyed around with a real-time versus turn-based gameplay. While real-time is fun, turn-based gameplay was something that we knew would attract those wanting a more thought-based strategic system opposed to a twitch based one. Furthermore, we knew that turn-based would eventually allow us to go the asynchronous route, a decision made further down the line, which was an attractive option in and of itself.


### TL;DR

We wanted to make a game! So we built a bunch of paper prototypes, which helped us shape what we were attempting to make. Our original concept shifted from a macro-oriented multiplayer tower defence game to a micro-oriented multiplayer tactics game. Paper prototyping helped us quickly and efficiently tune what we were building.

See the third post in this series <a href="/blog/2012/08/11/hacking-away/">here</a>.
