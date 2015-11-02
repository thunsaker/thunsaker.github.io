---
layout: post
author: Thomas Hunsaker
title:  "BitDroid is Dead. Long live BitDroid!"
date:   2014-08-25 15:21:35
tags: 
- apps
- bitdroid
- android
- dev
- brevos
- bitly
image: /img/green_square.png
---

BitDroid was my first Android app, since it has evolved with the platform since Android 1.5 it has changed a lot over the years, for the better. Android has grown in leaps and bounds, most notably since the introduction of [Android 4.0][android-4] (Ice Cream Sandwich). As a result Android has started to look (and work) much, much better than before. I had [restyled BitDroid][bitdroid-2-2] before after it broke horribly on all Android 4+ devices due to changes in the underlying system.

![BitDroid Evolution](/img/bitdroid_evolution_history.png)  

<div style="margin-top:-20px; text-align:center; font-size:0.8em;">The Evolution of BitDroid (Left to Right: v.0.5-1, 2, 2.5, 3)</div>

I was ready to retire the BitDroid name (and terrible icon) in favor of something new. BitDroid is dead. Long live BitDroid!

![Brevos Wings](/img/brevos_feature_green.png)

Welcome to Brevos.
Brevos is all new, new icon, new colors, new features, same great bit.ly link creation and statistics.

Brevos is a completely redesigned version of BitDroid, on the inside and out. I swapped all of my web service calls to use [Square's][square] [Retrofit][retrofit] and a combination of [Dagger][dagger] and [Green Robot's][green-robot] [EventBus][eventbus] to make development faster, keep the code cleaner and most importantly, make Brevos more stable to the end user.

![Brevos Main Screen](/img/brevos_main_3_1.png)

The new home screen displays some of your recent links, saving you a tap in the process. 

![Brevos Main Screen](/img/brevos_clicks_3_1.png)

I've added some fancy new graphs to better visualize link performance. I created an on-boarding experience for those new to my app.

<iframe width="100%" height="360" src="//www.youtube.com/embed/-7MdOLRZxRLk" frameborder="0" allowfullscreen></iframe>

One of my favorite new features is the pop-over that displays when you shorten from other apps. This was heavily inspired by [Pocket's][pocket] "Add to Pocket" feature which doesn't take you out of the app you are using to add something to your Pocket.

I hope that you enjoy the new version of <del>BitDroid</del> Brevos and continue sending feedback about things you would like to see. 

<a href="https://play.google.com/store/apps/details?id=com.thunsaker">
	<img alt="Get it on Google Play" style="width:250px;"
		 src="/assets/img/google_play_badge.png" />
</a>

Download or update today!

<div style="text-align:center;">
	<img alt="Brevos Logo" style="width:150px;"
		 src="/img/brevos_wing.png" />
</div>

[android-4]: http://www.theverge.com/2011/10/18/google-android-4-0-ice-cream-sandwich-official
[bitdroid-2-2]: http://thunsaker.github.io/2012/11/22/bitdroid-2-2-released/
[square]: http://square.github.io/
[retrofit]: http://square.github.io/retrofit/
[dagger]: http://square.github.io/dagger/
[green-robot]: http://greenrobot.de/
[eventbus]: https://github.com/greenrobot/EventBus
[pocket]: https://play.google.com/store/apps/details?id=com.ideashower.readitlater.pro