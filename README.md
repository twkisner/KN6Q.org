# KN6Q.org Theme
Ghost Theme for KN6Q.org (forked from Odin and Casper)
![Ghost version](https://img.shields.io/badge/Ghost-1.x.x-brightgreen.svg?style=flat-square)

**KN6Q.org Theme** is a very simple fork of the Ghost theme [Odin](https://github.com/h4t0n/odin) , which itself was a fork from the old version of Casper (pre-Casper 2.0).

## Intro
The current release version of Odin (1.3.0) is not fully compatable with Ghost 1.x.x, and I believe the author is probably no longer supporting it (and the demo webpage is down).  This fork makes the theme run clean (no errors) in the theme activation of Ghost 1.17.0+ (probably all versions of Ghost 1.x.x).  Not sure what if any problems the activations errors cause when using Odin 1.3.0, but this avoids any issues.  

Also, I depricated the Odin favicons in favor of using the favicons now built into the Ghost platform. 

### Features
* Old Casper (1.4 and below) minimalistic and clean style (without right side menu)
* Works with Ghost 1.x+
* Fully responsive (for mobiles and tablets)
* Home Page Navigation Menu Buttons
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
    'twitter-square': 'https://twitter.com/h4t0n',
    'linkedin-square': 'https://www.linkedin.com/in/kisner/',
    'github-square': 'https://github.com/twkisner',
    'rss':'https://kn6q.org/rss/'
    // you can add more icons
}

</script>


```


## Copyright & License

Released under the MIT License. 

Copyright (c) 2017 [Thomas Kisner](https://www.linkedin.com/in/kisner/) 

Copyright (c) 2016 [Andrea Tarquini](https://blog.h4t0n.com) aka [@h4ton](https://twitter.com/h4t0n)  (for Odin theme portions of code)

Copyright (c) 2013-2015 Ghost Foundation (for Casper theme substantial portions of code)


