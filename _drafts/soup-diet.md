My app tried the Cyril diet, you won't even recognize it!

[Cyril Mottier][cyril] wrote a great article about reducing the size of android apps: [Putting Your APKs On [A] Diet][apk-diet] The post describes general common sense things like, don't include resources you aren't using; to more advanced, use ProGuard to obfuscate and minify code.

I put one of my apps, [Soup][soup-play], on the Diet, here are the results.

Initial File Size

Specified resConfigs for language (got rid of unwanted language resources from Play Services, among other dependencies.) Easy. Quick.

Removed ldpi/mdpi folders. Easy. Quick.

Ran lint, removed unused drawables/layouts/menu and other resource files. Easy. Time-consuming

ProGuard, this took the longest, the first attempt to run threw a whole bunch of warnings, which took me qutie some time and effort to correct. Easy to enable, difficult to make work. Very time-consuming.

[cyril]: http://cyrilmottier.com/about/
[apk-diet]: http://cyrilmottier.com/2014/08/26/putting-your-apks-on-diet/
[soup-play]: https://play.google.com/store/apps/details?id=com.thunsaker.soup