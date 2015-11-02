---
layout: post
author: Thomas Hunsaker
name: bitdroid-2-2-released
title: BitDroid 2.2 Released
time: 2012-11-22 13:14:00.000000000 -08:00
tags:
- dev
- apps
- bitdroid
- android
image: /img/green_square.png
---
After completely rewriting BitDroid, I was sure to take advantage of all the new features that Android 4+ devices have to offer. One of those features I hadn't used before was [AsyncTask]("http://developer.android.com/reference/android/os/AsyncTask.html") which helps to load data in the background without tying up the UI thread. 
Android 4+ devices force this behavior, in order to increase the speediness of applications, and prevent the user from wondering if the app is doing anything or not.

With this release I modified the original code to fetch user history to first pull the list and second pull the click counts for each item, and then add them to the list as they are loaded. 
This has significantly increased load speed as the user gets to see the most pertinent information first, the links, and then the link counts, shortly thereafter. 
As seen below the links are present, and the refresh animation (in the upper right) is still spinning, once they load the hyphens will turn to numbers.
![BitDroid History](http://1.bp.blogspot.com/-1zHEcCDS2b0/UK6SXEZmmzI/AAAAAAAAPIw/8f6WD2nvuwU/s1600/BitDroid_2_2_History_Samsung_G3.png) I also took inspiration from Pocket, which checks the clipboard when you first load the app and asks if you want to save it to read later. 
I've added a fairly unobtrusive prompt that should get attention or be ignored depending on what the user wants to do. 
![BitDroid Clipboard](http://4.bp.blogspot.com/-KrcYPJ0Cj7Y/UK6TZtOjjGI/AAAAAAAAPI4/fh0BMUVW8WM/s1600/BitDroid_2_2_Main_Clipboard_Samsung_G3_chop.png)
BitDroid version 2.2 has been pushed to the play store, look for an update in the next few hours.  

BitDroid Free &nbsp;&nbsp;
<a href="http://play.google.com/store/apps/details?id=com.thunsaker"><img alt="Get it on Google Play" src="http://www.android.com/images/brand/get_it_on_play_logo_large.png" style="width: 200px;"></a>

BitDroid Donate &nbsp;&nbsp;
<a href="http://play.google.com/store/apps/details?id=com.thunsaker.BitDroid.Donate"><img alt="Get it on Google Play" src="http://www.android.com/images/brand/get_it_on_play_logo_large.png" style="width: 200px;"></a>