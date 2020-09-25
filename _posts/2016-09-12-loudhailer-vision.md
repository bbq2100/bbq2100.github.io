---
layout: post
title: LoudHailer – Reaching your audience!
excerpt: "Building the next fancy Goldberg machine just for learning purposes convinced myself fairly quickly.
          That said, I started this blog series to document my learn achievements during this side project..."
categories: [Loudhailer]
comments: true
---

### What's this?
Building the next fancy [Goldberg machine](https://en.wikipedia.org/wiki/Rube_Goldberg_machine) _just_ for learning purposes convinced myself fairly quickly.
With this idea in mind, I started this mini blog series to document my learn achievements during this side project.

For the curious: the illustrated `code` in the subsequent posts can be found [here](https://github.com/qabbasi/Loudhailer).
If you have any remarks or suggestions on the project don't hesitate to get in touch.

### The idea
What's LoudHailer about? Functionally it's a voice recognition app to detect emergency cases.

![Vision](http://i.imgur.com/CvWgRl0l.png) 

Technically spoken it's a stream processing application based on [Akka Streams](http://akka.io) and consists of the actual voice recording and a processing backend.
The backend automatically detects alarming words and notifies clients about an incident. For this I created a tiny Android app using [Kotlin](http://kotlinlang.org).
Also to make it super duper easy to use, I dockerized LoudHailer to run it directly on a [Raspberry](http://blog.hypriot.com/getting-started-with-docker-on-your-arm-device/). Cool, huh?

### Next
Let's get to the building blocks! The next post covers [functional stream processing]({% post_url 2016-09-15-loudhailer-stream %}) using Akka Streams.