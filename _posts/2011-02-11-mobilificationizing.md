---
layout: post
name: mobilificationizing
title: Mobilificationizing
time: 2011-02-11 08:35:00.001000000 -08:00
tags:
- mobile
- jquery
- productive
- sickday
---

If you are reading this on a desktop computer, the screen shots are for you. If you have a smartphone or other smaller screened device let me know in the comments how it looks and what does/doesn't work.  

I was feeling under the weather recently, and as a result I stayed home from work to sleep longer, take some medicine and get better. After waking up around 10am I realized that there were a few things I was putting off because I didn't have time during the day at work, and most of my free night-time is taken up by a side-project that I've been working on for the last few months [StudyBuddyCampus](http://studybuddycampus.com/) and normal life things.  

I took the opportunity to make some changes to my wife's blog about our family. It now has 3 columns and she loves it! Go take a look: [http://tommyandalisha.blogspot.com/](http://tommyandalisha.blogspot.com)  

I finally got around to fixing the obnoxious problem I have when I visit this very site on my phone, the fixed-width sidebar. I know that I haven't been the best at updating and that is partly due to me wanting to play Halo/Call of Duty/etc or just not feeling like I have anything interesting to say. I feel that, as a heavy mobile internet user, I should have a site that looks good on a phone.

My site was slapped together a few years ago using asp.net/c# with master pages. Their was no concern in my mind for a mobile site, luckily master pages are wonderful and all I needed to do was create a duplicate of my existing template and start chopping. First thing I did was move the sidebar on top so that it sits on top of the content it normally flanks. Then I gave each main wrapper a width of 100% so that it would stretch to whatever screen size it was given. I checked it out on my phone and realized that the phone thought the web page was much wider than the phone's screen. I added the following meta tag to prevent this and tell the page to fit the width of the device and not assume a desktop size.

<script src="https://gist.github.com/thunsaker/822624.js"></script>
<!--<script src="https://gist.github.com/822624.js?file=Viewport%20-%20Fill%20Device%20Width"></script>-->

<div style="text-align:center; margin-bottom:10px;">
    <img src="http://4.bp.blogspot.com/-GImTO5Hg7PQ/TVVw-T1jwnI/AAAAAAAAFTU/ocY9iXBkqsk/s400/th_mobile_menu_portrait.png" style="width:240px;" />
</div>

After a few more tweaks to the general layout and adjusting the padding/margins I got the site to look somewhat presentable. I used some fancy jQuery magic to get the sidebar er...menu to show/hide when the arrow in the upper right-hand is touched.  

<script src="https://gist.github.com/thunsaker/822640.js"></script>
<!--<script src="https://gist.github.com/822640.js?file=jQuery%20Mobile%20Dropdown%20Menu"></script>-->

<div style="text-align:center; margin-bottom:10px;">
    <img src="http://2.bp.blogspot.com/-BTVbQpM7L4I/TVVw-wfqTAI/AAAAAAAAFTY/2Y1dcD4ccIA/s400/th_mobile_portrait.png" style="width:240px;" />
</div>

Now all I needed to do was redirect users to the correct master page when visiting my site on a mobile phone. I found the following code online and added it to all pages in need of the mobile layout.  

[C# Mobile Master Page Switch.cs](https://gist.github.com/thunsaker/826115)

<!--<script src="https://gist.github.com/thunsaker/826115.js"></script>-->
<!--<script src="https://gist.github.com/826115.js?file=C%23%20Mobile%20Master%20Page%20Switch.cs"></script>  -->

After that was in place I realized that images from my posts were a little bit too wide for the average phone screen. Instead of manually resizing all of my images, I once again turned to jQuery for some help. Using an example I found, I check each image's width, if it is wider than the current width of the body tag, it reduces its size to fit nicely within the confines of the given screen.  

<script src="https://gist.github.com/thunsaker/822655.js"></script>
<!--<script src="https://gist.github.com/822655.js?file=jQuery%20Reformat%20images%20for%20Mobile.js"></script>  -->

All in all the process was fairly painless to convert an existing site, most of the work was getting the formatting correct. In the future I'd like to build a site from the ground up with current mobile browsers in mind, but that's for another sick day...  