---
title:  "Android Development Trial"
date:   2016-07-28 19:00:00 +0800
categories: blog
tags: android blog
---

> TL;DR
>
> I learnt some of the Android approaches that I missed in the projects I've been working on, such as I18n, at the same time, I also find that the documentation of Android is kind of terrible, especially when you only want to use the latest version of Android APIs _without_ backward compatibility.
>
> After finish this little _A humanitarian APP against sound activated light switches in some scenes_ app, I found that, even though I've got the functionalities I want, however, I wasn't in the ___correct___ way of doing Android development, for example, I didn't use the layouts and components properly.. will do better maybe the next time :P

About 2 months ago, when I was on vacation, I spent about 5 days (say 8 work hrs/day) to try Android development, for fun, and, of course, for some benifits.

The app is named "[Cry for Light](https://github.com/unknownmoon/android-cry-for-light)", which is "A humanitarian APP against sound activated light switches in some scenes". Literally, it cries when the brightness is low :P

Why should this app exist?

### The Story

The story starts from that our company replaced some light switches of the pantries to _sound activated light switches_.

In the pantries, there're several water coolers, to provide cool and especially hot water, and in one of the pantries, there are some tables for having meals, along with a foosball table (that's great!).

As you probably have been aware of, it definitely takes sometime to fulfill a bottle with _hot_ water, and takes more time to finish a meal or play foosball.

Unfortunately, the new lights will only be triggered by a relatively louder voice, and then keep on for about 1 minitue or so. They're going to be _off_ anyway before the next turning on, even if the loud voice is still there... (great job right?)

Hence if one washes one's cup before fulfill hot water, it's highly likely the light will be off during fulfilling the hot water, after the light is off, we can barely see things, so the hot water might run out of one's cup if one don't stop at the proper time... sounds dangerous right?

That would be even __better__ if you're in a queue to wash your cup or fulfill water, not to mention the _dinner_ or _foosball_ stuff..

OK, even we're in such a smart company, as a developer, we should make our own lives easy, right?

Thus, the requirements are really straightforward: since we have smartphones with light sensors and speakers, why not just monitor the brightness of the env and play sound once it turns dark? As long as it turns dark anyway...

### Learn Android Development

I was thinking to develop a web app + using Chrome routine, but just accidently found some Android materials, so why not I try something new? A bonus that I was using Nexus 5X :P

The Android development toolchains are awesome now, I mean the Android Studio turned from eclipse-based to intellij-idea-based. I got the env set up in my MacBook really easily.

As I didn't really want to dig into Android development, I decided to _support Android 6+ on Nexus 5X only_, so that it would be easier and quicker to get started and achieve my goals, however, when I went to the documentation, I was kind of lost: how can I find the complete set of APIs/Components I need, specifically the Android approaches using only the latest APIs?

If you've seen the documentation of Android, you'll find that apart from the basic concepts, most of the examples are kind of _backward compatible_. That's great, for the others, but not for me. I don't really want the `v7 appcompact` lib or `v4 appcompact` lib, I only want the latest!

Yes I can use the latest libs only anyway, but then the documentation becomes less helpful and harder to find what a _new_ android developer need... that's the terrible part...

### What I learn

I learnt the basic concepts such as intents, activities, services, learnt how to layout and use the assets, learnt how to use notifications and perferences... a lot of Android fundamentals (even though I've forgotten a lot of them now LOL), but the most impressive part may be how Android works with the resources.

In my previous work projects, I don't think we worried a lot about __Theme__, __I18n__, __Responsive__(i.e layouts and different image assests for different views), and an important one, __Performance__. We didn't do a lot of __Test__ too... sounds bad :(

In Android, it suggests that one should always externalise the strings, numbers or other values, for easier I18n and more, and by doing that, say externalise the colours, one can change the colour scheme very easily.

Android also provides a mechanism to load different resources for different devices (DPI, screen size or so). This is a non-trivial part of improving the user experiences on mobile devices. _Responsive_ is always mentioned by our team, but rarely turned into practices. 

Another important reminder is the _Performance_. In the guide of Android, it always highlights what should be considered in order to improve the performance. Such as should not leave a service running whenever unnecessary.

After reading the parts related to performance, I finally understand why my phone is so slow after installed a lot of Chinese Android apps, even though I don't open a lot by myself.

Most of Chinese apps are doing really great job to always keep their services UP, which occupy a lot of memory of the device.

Regarding the performance, even though our devices are getting better and better nowadays, we should not rely on that "the user devices should be capable for that", since if the developers of every app think like the same, our devices are dying anyway...

### Well...

Actually, I also learnt that I should focus more on what I'm doing, web development, and improve my shortages such as mobile web, performance, responsive, in order to make some really good apps :P
