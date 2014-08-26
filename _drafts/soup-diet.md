---
layout: post
title:  "My app tried The Cyril APK Diet, you won't belive how it changed!"
date:   2014-08-26 13:18:58
tags: 
- apps
- soup
- dev
---

<style>
	.apk_text {
		color:teal;
	}
</style>

Upworthy title aside, apps have gotten quite bloated lately, with higher resolution assets and numerous libraries that ease development but also contribute, sometimes significantly, to APK size. [Cyril Mottier][cyril] wrote a great article about reducing the size of android apps: [Putting Your APKs On Diet][apk-diet] The post describes general common sense things like, don't include resources you aren't using; to more advanced, use ProGuard to obfuscate and minify code.

I put one of my apps, [Soup][soup-play], on the Cyril APK Diet, here are the results:

**Initial File Size**: <span class="apk_text">5.10 MB</span>

##1. Remove Unused/Old Res Folders
**Easy - Quick**  
I removed both ldpi/mdpi folders. Specified resConfigs for language (got rid of unwanted language resources from Play Services, among other dependencies.)  
**APK Size**: <span class="apk_text">4.40 MB</span> - <span class="apk_text">13% Total Reduction</span>

##2. Android lint
**Easy - Time-consuming**  
I ran lint, using `gradlew lint` from the terminal, then removed unused drawables/layouts/menu and other resource files that lint discovered. You have to be careful here, if you are referencing a drawable in code, lint doesn't necessarily see that, so you should, as Cyril points out, "Know your code like the back of one’s hand."  
**APK Size**: <span class="apk_text">4.19 MB</span> - <span class="apk_text">17.8% Total Reduction</span>

##3. Minify PNGs
**Medium - Fairly quick**  
I minified PNGs using [PNGoo][pnggoo], there are loads of tools on that page for all platforms, GUI and command line.  
**APK Size**: <span class="apk_text">4.16 MB</span> - <span class="apk_text">18.4% Total Reduction</span>

##4. ProGuard
**Difficult - Very Time-consuming**  
This took the longest, the first attempt to run threw a whole bunch of warnings, I cleaned up redundant dependencies from included libraries. This is really easy to enable just add 
{% highlight groovy %}
runProguard true
proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.txt'
{% endhighlight %}
to your build.gradle, however it is incredibly difficult to make work depending on your included dependencies. After a few hours of searching Google, StackOverflow and GitHub I gave up. I was able to remove some proguard warnings using a few helper libraries, but got stuck on Dagger, like [many][dagger-issues-1], [many][dagger-issues-2], [others][dagger-issues-3]. I could get some warnings to go away, but then another error popped up elsewhere. I don't know how much space I would save if I could actually get ProGuard to run. I'll take another look at it when Dagger 2 is released, it should remove some of the problems I and others encountered.  
**APK Size**: <span class="apk_text">Unknown</span>

##Conclusion
You should definitely attempt to clean up any code/resources that you aren't using in your apps. I saved ~1MB, doesn't seem like much, but considering the relatively small effort (excluding ProGuard) that it required, well worth it. Maybe you will have better luck with ProGuard than I did. Happy dieting.

[cyril]: http://cyrilmottier.com/about/
[apk-diet]: http://cyrilmottier.com/2014/08/26/putting-your-apks-on-diet/
[soup-play]: https://play.google.com/store/apps/details?id=com.thunsaker.soup
[pnggoo]: http://pngquant.org/
[dagger-issues-1]: https://plus.google.com/u/0/+Ond%C5%99ej%C4%8Cerm%C3%A1k/posts/HMiCxi4wh7J
[dagger-issues-2]: https://github.com/square/dagger/issues/202
[dagger-issues-3]: http://stackoverflow.com/questions/23951753/dagger-proguard-obfuscation-errors-creating-object-graph
