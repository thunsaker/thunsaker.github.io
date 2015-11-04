---
layout: post
name: you-work-for-me-now
title: You Work for Me Now
author: Thomas Hunsaker
time: 2012-08-31 10:19:00.000000000 -07:00
tags:
- mobile
- hacks
- notifications
- web apps
- android
image: /img/pink_square.png
---

In the last few weeks I have discovered a few services that take boring and 
menial tasks and turn them into automatic automated awesomeness. The general 
rule is: “If it is too difficult to do or remember, most people won’t do it.” 
Basically, any amount of complexity or repetition added to a task makes it easy 
to put off and not ever do, especially things we need to do, like letting your 
wife know when you’ll be home from work. Here’s where [IFTTT](http://ifttt.com/) 
and [on{X}](http://onx.ms/) come into play. They allow normal people 
(non-programmers) to easily setup simple tasks that can automate some of our 
life both online and off.

### IFTTT

If This Then That ([IFTTT](http://ifttt.com)), is the simplest form of logic: __if__ this event happens, __then__ execute __that__ action. If I Tweet, then post to Facebook. IFTTT is the biggest mashup of web services and APIs that I have ever seen, seriously check out their list of ["Channels"](https://ifttt.com/channels) as of this writing there are 50 different services you can connect to.

At its heart IFTTT is about making your digital life simpler by automating tasks. Some common examples include [cross-posting](https://ifttt.com/recipes/search?q=crosspost) a status update, [backing up photos](https://ifttt.com/recipes/search?q=photos), [will it rain tomorrow?](https://ifttt.com/recipes/search?q=rain), and letting people know when you finally [posted to your blog](https://ifttt.com/recipes/search?q=blog). Among options you can have a notification sent via email, sms or push message when a trigger occurs, or have things happen passively and not need to do or see anything. This is especially useful for backing up my photos, pretty much anything I post online can be transferred to my Dropbox account and saved on my home computer. I don’t have to worry about it.

I setup a [special recipe](https://ifttt.com/recipes/54001) to email my dad, who refuses to use Facebook and doesn't have an Android or iPhone, so he can see the awesome pictures of my son, whenever I post them.

<div style="text-align:center; margin-bottom:10px;">
    <img src="http://3.bp.blogspot.com/-s9iW8c8jGvQ/UED0eOlUDwI/AAAAAAAAMn4/kkXdnU2YuJI/s1600/ifttt_email_dad_instagram.png" style="width: 350px;" />
</div>

Recently IFTTT has integrated with the physical world, through the use of Belkin’s recently released set of [WeMo sensor/switches](http://www.theverge.com/2012/6/20/3101746/ifttt-website-redesign-belkin-wemo-switch-motion). These sensors can be setup as triggers or actions, you can have your lights automatically turn on at 6AM, or off at 10PM. You can receive a notification when a switch has been triggered, or turn on/off a light with a text message. The possibilities are pretty amazing when you think about being able to trigger certain actions based on the whether outside. One recipe: [If it gets cold, turn on my bedroom heater](https://ifttt.com/recipes/46031), lets you have a nice warm bed when you need it.

### on{X}
[on{X}](http://www.onx.ms/) was developed by Microsoft as an [experiment](http://www.droid-life.com/2012/06/05/microsoft-creates-onx-app-for-android-wants-to-automate-your-life/) in automating your life through your Android phone. This has the same concept as above, __on X__, or when __X__ happens, __do__ this. The key difference here is that it is using your phone and its many sensors to receive triggers, and perform actions: on{leave my house} turn off my wifi.  

<div style="text-align:center; margin-bottom:10px;">
<img border="0" style="width:250px;" src="http://3.bp.blogspot.com/-_Z0DFoZ9y1Q/UED0eqtnOoI/AAAAAAAAMoA/U-VYeDhn-bI/s320/onx_turn_off_wifi.png" />
</div>

Recipes are written online and then pushed to your phone through the [on{X} app](https://play.google.com/store/apps/details?id=com.microsoft.onx.app) which hooks into all of the hardware sensors, so you can detect your location and perform an action. For example, [send my wife a text message when I leave work](https://www.onx.ms/#!recipeEditPage?scriptId=geoFenceTextMsg), this is great because I don’t have to remember to let her know that I left, it happens automatically and it comes from my phone.

They’ve recently [updated](https://dev.onx.ms/2012/08/30/version-0-58-is-out/) their system to support NFC, proximity sensor, and a few other great enhancements. I’ve setup my phone to [disable wifi](https://www.onx.ms/#!recipeEditPage?scriptId=wiFiOnRegion) when I leave home, [launch Foursquare](https://www.onx.ms/#!recipeEditPage?scriptId=launchAppOnVisit) once I’ve been in a place for longer than 20 minutes, and to message my wife when I leave work. These have saved me time by having my phone do things automatically, things that I might forget or otherwise not have time to do. on{X} hasn’t been around as long as IFTTT so their list of [pre-built recipes](https://www.onx.ms/#recipesPage) isn’t very long, but one of the great things, is that on{X} allows you to [write your own recipes](https://www.onx.ms/#apiPage) and share them with the community. I modified the “launch Foursquare” recipe to only trigger when I am outside the range of my home, since I don’t checkin at my house.

As with my previous post about push notifications, these put our phones to work for us, so we can keep up with our responsibilities, obligations, etc. and also make our lives a little more comfortable. Being able to setup these events and then receiving notice about actionable items helps to use my phone as a tool instead of just a huge distraction. Happy experimenting!