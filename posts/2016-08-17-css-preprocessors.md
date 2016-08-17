---
title:  "CSS Preprocessors: Less, Sass, Stylus, and PostCSS"
date:   2016-08-17 01:11:11 +0800
categories: tech
tags: css-preprocessor front-end blog less sass stylus postcss
---

CSS preprocessors have been around for years. Now that it's 2016, so which one do I prefer? 

Here are some popular choices: [`Less`](less-link), [`Sass`](sass-link), [`Stylus`](stylus-link), and [`PostCSS`](postcss-link), however, first of all, why do I need CSS preprocessor?

## Key use cases

In my own scenario, the key use cases are:

* Externalise the common values using _Variables_, such as the _sizes_ and _colours_.
* Externalise the common logic using _Mixins_, along with _Loops_ and _Conditional Statements_ to implement some complicated logic.
* _Nested Rules_, for myself, is mainly to reduce typing and keep the module organised.

Hence the following features are used mostly:

* Variables & Variable Interpolation
* Mixins (including Extend) & Loops & Conditions
* Nested Rules & Parent Reference

__Bibliography__

1. [CSS PREprocessors - Compare](1)

<!-- references -->

[1]: https://csspre.com/compare/ "CSS PREprocessors - Compare"

<!-- links -->

[less-link]: http://lesscss.org/ "Less Home"
[sass-link]: http://sass-lang.com/ "Sass Home"
[stylus-link]: http://stylus-lang.com/ "Stylus Home"
[postcss-link]: http://postcss.org/ "PostCSS Home"