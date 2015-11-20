---
title:  "Bootstrap 3 v.s. Foundation 5"
date:   2015-04-02 02:10:00 +0800
categories: tech
tags: css-framework front-end blog
---

Now I'm looking for a HTML/CSS/JS framework for build a theme for this blog, there are two of the frameworks on the top of the list - [Bootstrap][bootstrap-link] and [Foundation][foundation-link].

Based on the articles I found, it seems that Foundation wins. Following are the pros of Foundation:

* Foundation 5 provides a better grid system than Bootstrap 3 - [The Block Grid](http://foundation.zurb.com/docs/components/block_grid.html)
* Foundation 5 is using `rem` as sizing unit while Bootstrap 3 is using `px`, namely Foundation 5 is closer to the concept `responsive` or `mobile-first`
* Foundation 5 provides some useful features, such as form validation ([Abide](http://foundation.zurb.com/docs/components/abide.html)), [Interchange](http://foundation.zurb.com/docs/components/interchange.html), [right-to-left support](http://foundation.zurb.com/docs/components/rtl.html), [pricing tables](http://foundation.zurb.com/docs/components/pricing_tables.html), [tours](http://foundation.zurb.com/docs/components/joyride.html), and [off-canvas navigation](http://foundation.zurb.com/docs/components/offcanvas.html) <sup>[[1]]</sup>

However, Bootstrap 3, or generally Bootstrap, is occupying a larger market, which means that there are much more themes in the wild than Foundation.

Other than the comparison above, people are also discussing about that for using Foundation, one need more customisation than using Bootstrap. It takes longer than using Bootstrap for initialising a project. It sounds like that if we don't use third party themes, using Foundation could reduce the similarity of the web application comparing using Bootstrap.

There are other thoughts learned from the articles, that I found when people evaluating this kind of frameworks, they consider more about the grid system, sizing unit and how good the framework fits the requirement of mobile-first/responsive design.

All in all, Foundation 5 is decided to be used for the theme of this blog, if nothing special happens.

__Bibliography__

1. [Should You Use Bootstrap or Foundation?][1]
1. [Foundation 5 Features that Bootstrap Doesn't Have][2]
1. [Grid System Comparison: Bootstrap 3 v.s. Foundation 5][3]
1. [Bootstrap vs. Foundation: Which Framework is Better?][4]
1. [Responsive CSS Framework Comparison][5]
1. Why rem
    - [There's more to the CSS rem unit than font sizing](https://css-tricks.com/theres-more-to-the-css-rem-unit-than-font-sizing/)
    - [Font sizing with rem](http://snook.ca/archives/html_and_css/font-size-with-rem)
    - [What's the Deal With Em and Rem?](http://designshack.net/articles/typography/whats-the-deal-with-em-and-rem/)

<!-- references -->

[1]: http://blog.teamtreehouse.com/use-bootstrap-or-foundation "Should You Use Bootstrap or Foundation?"
[2]: https://scotch.io/tutorials/foundation-5-features-that-bootstrap-doesnt-have "Foundation 5 Features that Bootstrap Doesn't Have"
[3]: http://www.sitepoint.com/grid-system-comparison-bootstrap-vs-foundation/ "Grid System Comparison: Bootstrap 3 v.s. Foundation 5"
[4]: https://bootstrapbay.com/blog/bootstrap-vs-foundation/ "Bootstrap vs. Foundation: Which Framework is Better?"
[5]: http://responsive.vermilion.com/compare.php "Responsive CSS Framework Comparison"

<!-- links -->

[bootstrap-link]: http://getbootstrap.com/ "Bootstrap Home"
[foundation-link]: http://foundation.zurb.com/ "Foundation Home"
