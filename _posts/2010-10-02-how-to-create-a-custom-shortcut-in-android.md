---
layout: post
author: Thomas Hunsaker
name: how-to-create-a-custom-shortcut-in-android
title: How to Create a Custom Shortcut in Android
time: 2010-10-02 23:13:00.000000000 -07:00
tags:
- custom
- hacks
- gmail
- cyanogen
- android
- shortcuts
image: /img/teal_square.png
---

I'd been wanting a quick and easy way to compose a new email. I tried my hand at whipping up a simple program that just installed a homescreen shortcut, but ran into namespace issues and didn't feel like putting more than an hour into it.  

A few days later while messing around with my homescreen shortcuts/widgets and discovered how to use the Custom Shortcuts option available in some aftermarket launcher programs such as [ADW Launcher](http://jbthemes.com/anderweb/category/adwlauncher/) and [LauncherPro](http://www.launcherpro.com/). I've been running [CyanogenMod 6](http://www.cyanogenmod.com/) (based on Android 2.2/Froyo) for about a month now, which includes ADW, so my screenshots and examples will reflect that.

Any Android hacks you'd like to share in the comments?  

### How to Create a "New Email" Shortcut ([Google Doc](href="https://docs.google.com/document/pub?id=1oYxJ1d170BBqouPVRmU0hHanzuNlzymwziDhzvO5mxs))  

On the homescreen and either long-press on empty space or hit Menu, Add:  

<img src="http://1.bp.blogspot.com/_DiR5Uh09_qs/TKjP0Ezz7-I/AAAAAAAAFJc/abQ1Go0CUWk/s320/homescreen+add.png" style="width:480px; height:320px;" />

Select "Custom shortcut" from the list:  

<img src="http://1.bp.blogspot.com/_DiR5Uh09_qs/TKjP4qkhW-I/AAAAAAAAFJg/c-WcuzonbOM/s320/homescreen+cutom+shortcut.png" style="width:480px; height:320px;" />

Select "Pick your activity":  

<img src="http://4.bp.blogspot.com/_DiR5Uh09_qs/TKjPDcyiMxI/AAAAAAAAFJU/Sn3nSn8ITWY/s320/homescreen+shortcut+pick+your+activity.png" style="width:480px; height:320px;" />

Select "Activities" (this displays a list of all activities for every installed program):  

<img src="http://2.bp.blogspot.com/_DiR5Uh09_qs/TKjP98o0YBI/AAAAAAAAFJk/j_iWrheC-Uw/s320/homescreen+cutom+shortcut+Activities.png" style="width:480px; height:320px;" />

Tap "Gmail" in the list:  

<img src="http://2.bp.blogspot.com/_DiR5Uh09_qs/TKjPBQaLPoI/AAAAAAAAFI8/M4gmBtaocig/s320/homescreen+activities+gmail.png" style="width:480px; height:320px;" />

Sift through the various activities available within the messaging app to find "Compose(.ComposeActivityGmail)":  

<img src="http://4.bp.blogspot.com/_DiR5Uh09_qs/TKjPDNX6sUI/AAAAAAAAFJQ/Cv4eUgxZQEc/s320/homescreen+gmail+ComposeActivityGmail.png" style="width:480px; height:320px;" />

Once you have selected the activity, it will return you to the Custom shortcut dialog. Enter a name, if you don't like the default, that will display on the homescreen (you can also change the icon by touching the default icon.)  
Hit "Ok" when you are done:  

<img src="http://1.bp.blogspot.com/_DiR5Uh09_qs/TKjPCNjOSeI/AAAAAAAAFJE/8V6HYrL9wIs/s320/homescreen+custom+shortcut+gmail.png" style="width:480px; height:320px;" />

Huzzah! You've added a Custom Shortcut  

<img src="http://4.bp.blogspot.com/_DiR5Uh09_qs/TKjQqMtJifI/AAAAAAAAFJo/lTyTWD3FlTY/s320/homescreen+done.png" style="width:480px; height:320px;" />

These instructions relate to semi-stock Android 2.2 your mileage may vary. You can also do the same for pretty much any other application that has a "Compose..." or "Edit..." activity. I was able to create a New Gmail, New Event, and New Tweet shortcut, just had to hunt the right activity down in the list (though this didn't work for the default messaging application).  

Enjoy!
