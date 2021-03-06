---
layout: post
author: Thomas Hunsaker
name: rapido-1-2-released
title: 'Rapido 1.2 Released'
time: 2012-10-07 23:42:00.001000000 -07:00
tags:
- mobile
- apps
- android
- rapido
image: /img/teal_square.png
---

Rapido 1.2 now works with Android 4+ devices! I also added the option to send/share to Rapido to make posting messages, and especially ones with links even faster.

![Rapido 1.2 Link Count](http://3.bp.blogspot.com/-36O-KHWszlA/UHL1GkGJ9WI/AAAAAAAANAg/pQVhYW8ZSEQ/s320/rapido_screen_main_1_2_link_count.png)
For twitter posts, links are now counted as 20 characters if you go over the 140 char limit, since they are shortened by Twitter once sent to their servers.  

__Future Plans__  
Link shortening powered by bit.ly with account login
App.net posting*  
Multiple Twitter accounts*  
Facebook Pages*   
Posting photos*   
(*denotes wishful thinking)

__Developer Notes__  
Shortly after releasing the first version of Rapido, I received a message from a friend informing me that the app didn't work on his new phone which ran Android 4 Ice Cream Sandwich. My personal phone still runs Android 2.3 Gingerbread, so I was somewhat puzzled at this since my app wasn't doing anything crazy. Apparently I had failed to read up on the guidelines introduced in Android 3 Honeycomb, which prevents and stops execution of data gathering or other tasks that require the Internet from running in the foreground. What? This took me some time to properly correct, and diagnose since the error message wasn't exactly clear to me.

This seemed easy to solve, just move all of the token fetching and message sending stuff to the background. Done. Well it ended up being a laborious task that took quite a bit of trial and error on my part. Once I'd get one part working another thing would break in the process. I now pay much more attention to the little helps that eclipse drips when it turns some things red and lets me know that they are deprecated. They may continue to work on older versions of the software, but eventually they will break things. Some forums posts said "I just changed the target version to 2.3 and everything worked, again" I hope those people realized that they may have fixed an error message, but they didn't fix the problem.

These changes are obviously necessary due the nature of software. As things get more and more complex the need to revise things and update them arises and this often times means cutting away the legacy stuff that isn't useful or is taxing the whole system for a little convenience and familiarity. The first few times I tried writing an AsyncTask I misunderstood how they worked. I couldn't figure out how to get the background task to communicate with the foreground, this took some more reading and looking at other people's code, my favorite way to learn, to figure out that these Android developers knew what they were doing and this would in fact make my app faster. By the time I got the last few changes in this release I had the AsyncTasks down no problem.
I've been developing multiple apps for work and for fun (at home), it is always exciting to me when I learn something and then can immediately apply it to another project. This is one of the reasons I love programming so much, I am constantly learning and improving. If I get some requests I might write up a more technical post for those others out there that are struggling to make their apps future friendly with Android 4+.

<a href="http://play.google.com/store/apps/details?id=com.thunsaker.rapido"><img alt="Get it on Google Play" src="http://www.android.com/images/brand/get_it_on_play_logo_large.png" style="width: 200px;"></a>