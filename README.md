# KN6Q.org Theme
Ghost Theme for KN6Q.org (forked from Odin and Casper)
![Ghost version](https://img.shields.io/badge/Ghost-3.x-brightgreen.svg?style=flat-square)

**KN6Q.org Theme** is a fork of the Ghost theme [Odin](https://github.com/h4t0n/odin), which itself was a fork from the old version of [Casper](https://github.com/TryGhost/Casper/) (before Casper 2.0).

## Intro
This fork was orginally to fix the Odin theme to run clean (no errors) in the theme activation of Ghost 1.0+. (Version 1.4.x), because the author wasn't actively supporting it.  While Odin has now been updated to be compatable with Ghost 2.0 (including some fixes from me), my theme still has some differences.

I depricated the Odin favicons in favor of using the favicons now built into the Ghost platform in 1.x, and merged in some things from the latest 1.4 version of "old" Casper, as well as implemented features from Ghost 2.0 like multiple author support.

Version 1.6.x fixes the theme to work with Ghost 3.0+. Version 1.5.x fixes the theme to work with Ghost 2.0+.  Version 1.4.x is compatable with Ghost 1.0+.

![gscan results](https://github.com/twkisner/KN6Q.org/blob/master/gscan.JPG)

### Features
* Old Casper (1.5 and below) minimalistic and clean style (without right side menu)
* Works with Ghost 3.0, 2.0 and 1.0
* Fully responsive (for mobiles and tablets)
* Home Page Navigation Menu Buttons
* Uses the built-in Ghost favicon function (Publication Icon in General Settings) rather the generating manually.
* Google Analytics (easily configurable by code injection in the admin area)
* [Disqus](https://disqus.com) comments (easily configurable by code injection in the admin area)
* [Prism](http://prismjs.com/) Syntax Highlight (all languages supported)
* [RRSSB](https://github.com/kni-labs/rrssb) Extraordinary Social Sharing Buttons
* [Font Awesome](http://fontawesome.io) home page Social Link Icons (easily configurable by code injection in the admin area)

## Configuration
No need to configure ***Prism*** or ***RRSSB*** buttons.

To add Homepage Navigation Menu Buttons simply add the links in your Navigation Admin Area. They may be useful for static pages (*AboutMe* for example) or for shortcut to your (best) post tags.  

***Disqus*** comments, ***Google Analytics***  and ***Font Awesome Home Page Social Link Icons*** are disabled by default, but they are easily configurable with *Blog Header Code Injection* inside your Ghost Admin Area.

```html
<script>
// to enable Google Analytics
var ga_id = 'YOUR-UA-ID_HERE';

// to enable Disqus
var disqus_shortname = 'YOUR_DISQUS_SHORTNAME'


// to enable Social Link Icons add the social_link object
// with the pair key/value -> social_network/link
// NB: the key is used to include the right icon from Font Awesome
// (you can include any Font Awesome icon)

// Example1: default social network icons
var social_link = {
    'twitter': 'https://twitter.com/twkisner',
    'linkedin': 'https://www.linkedin.com/in/kisner/',
    'github': 'https://github.com/twkisner',
    'rss':'https://kn6q.org/rss/'
    // you can add more icons
}

// Example2: squared social network icons
var social_link = {
    'twitter-square': 'https://twitter.com/twkisner',
    'linkedin-square': 'https://www.linkedin.com/in/kisner/',
    'github-square': 'https://github.com/twkisner',
    'rss':'https://kn6q.org/rss/'
    // you can add more icons
}

</script>


```


## Copyright & License

Released under the MIT License. 

Copyright (c) 2017-2020 [Thomas Kisner](https://www.linkedin.com/in/kisner/) 

Copyright (c) 2016 [Andrea Tarquini](https://blog.h4t0n.com) aka [@h4ton](https://twitter.com/h4t0n)  (for Odin theme portions of code)

Copyright (c) 2013-2015 Ghost Foundation (for Casper theme substantial portions of code)


