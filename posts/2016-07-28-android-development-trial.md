---
title:  "Android Development Trial"
date:   2016-07-28 19:00:00 +0800
categories: blog
tags: android blog
---

> TL;DR
>
> I learn that some of the Android approaches are what I missed in the projects I've been working on, such as I18n, at the same time, I also find that the documentation of Android is kind of terrible, especially when it comes to the versions of Android APIs.
>
> After finish this little _A humanitarian APP against sound activated light switches in some scenes_ app, I found that even though I've got the functionalities I want, however, I wasn't in the ___correct___ way of doing Android development.. will do better maybe the next time :P

About 2 months ago, when I was on vacation, I spent about 5 days to try Android development, for fun, and of course for some benifits.

The app is named "[Cry for Light](https://github.com/unknownmoon/android-cry-for-light)", which is "A humanitarian APP against sound activated light switches in some scenes".

Why should there be an app like that?

### The Story

The story starts from that our company replaced some light switches to _sound activated light switches_, in the pantris.

In the pantries, there're several water coolers, to provide cool and especially hot water. In one of the pantries, there are some tables for having meals, along with a foosball table (that's great!).

As you probably have been aware of, it takes sometime to fulfill a bottle with _hot_ water, and takes more time to finish a meal or play foosball, however, the light will only be triggered by a relatively loud voice, and keep on for about 1 minitues or some, additionally, the light will _off_ anyway before the next trigger.

Hence the situation becomes that one enter the pantry area, make a loud noice to turn the light on, and then if one washes one's cup before fulfill hot water, it's highly likely the light will be off during fulfilling the hot water, after the light is off, we can barely see things, such as the level of the hot water in you cup/bottle.. sounds dangerous right? That would be even __better__ if you're in a queue to wash your cup or fulfill water, not to mention the _dinner_ or _foosball_ stuff..

OK, since we're in such a smart company, as a developer, we should save our own lives, right?

The requirements are really simple: since we have smartphones with light sensors and speakers, why shouldn't we just monitor the brightness of the env and play sound once it turns dark?

### Learn Android Development

I was thinking to develop a web app + use Chrome to achieve the goal, but just accidently found some Android materials, so why didn't I try something new, as long as I was using Nexus 5X?

The Android development toolchains are awesome now, I mean the Android Studio turned from eclipse-based to intellij-idea-based. I got the env set up in my MacBook really easily.

As I didn't really want to dig into Android development, I decided to _support Android 6+ on Nexus 5X only_, so that it would be easier and quicker to get started and achieve my goals, however, when I went to the documentation, I was kind of lost: how can I find the complete set of APIs/Components I need, specifically the approaches for the latest APIs (at that time).

If you've seen the documentation of Android, you'll find that apart from the basic concepts, most of the examples are kind of _backward compatible_. That's great, for the others, but not for me. I don't really want the `v7 appcompact` lib or `v4 appcompact` lib, I only want the latest!

Yes I can use the latest libs only, but then the documentation becomes less helpful and harder to find what a _new_ android developer need... that's the terrible part...

### What I learn

I learnt the basic concepts such as intents, activities, services, learnt how to layout and use the assets, learnt how to use notifications... a lot of Android fundamentals (even though I've forgotten a lot of them now LOL), but the most impressive part is how Android uses the resources.

In my previous work projects, I don't think we worried a lot about __Theme__, __I18n__, __Responsive__(i.e layouts and different image assests for different views), and an important one __Performance__.

In Android, it suggest that one should externalise the strings, numbers or other values, for easier I18n, and by doing that, say externalise the colours, one can change the colour scheme very easily.

Android also provides a mechanism to load different resources for different devices (DPI, screen size or so). This is a non-trivial part of improving the user experiences on mobile devices. _Responsive_ is always mentioned by our team, but rarely turned into practice. 

Another important reminder is the _Performance_. In the guide of Android, it always highlights what should be considered in order to improve the performance. Such as should not leave a service running whenever unnecessary (Most of Chinese apps are doing really great job to always keep their services UP, which occupy a lot of memory of the device). Regarding the performance, even though our devices are getting better and better, we should not rely on that "the user devices are capable for that", since if every app thinks the same, our devices are dying anyway...

### Well...

Actually, I learnt that I should focus more on what I'm doing, web development, and improve my shortages such as mobile web, performance, responsive, and make some really good apps :P
