---
layout: post
title: "At Velocity"
date: 2012-06-25 18:51
comments: true
categories: 
- Conferences
- DevOps
- Puppet
---

So, I'm at the [O'Reilly Velocity](http://velocityconf.com/velocity2012) conference this week, followed by [DevOpsDays Mountain View](http://www.devopsdays.org/events/2012-mountainview/).  I'm not going to lie and say this will interrupt my regular posting schedule :)

However, this means I'll have some technical stuff to talk about!  Unfortunately day one was a bit of a wash.  Here's what I did so far:

<!--more-->

## [Understanding and Optimizing Web Performance Metrics](http://velocityconf.com/velocity2012/public/schedule/detail/23857)

Good little DevOpsy operations guy that I am, I had to come to this talk.  Bryan clearly knows a lot about the field and gave explicit examples of things you can do to make your site suck less.  Unlike a good deal of similar talks I've been to this had concrete examples of what to do and not do, including those places where there's no hard and fast rule and testing is needed. (Hint, if you're making these kind of changes, make sure you can tell if they work)

Bonus points for having the slides be HTML5 and online (can be seen at [https://perf-metrics-velocity2012.appspot.com/](https://perf-metrics-velocity2012.appspot.com/)).  Even better, the numbers being collected in the first part are embedded, in Javascript, in the slides, so you can see examples of the numbers.

I have a few nitpicks in there (when talking about OSes and browsers, version numbers are super important!  Windows XP and Windows 7 have, I understand, different TCP stacks by a lot, so quirks of one may not be in the other), but it was a solid start to the day.

Even better, I have a concrete thing to check when I get back to the office: where is our GZIP compression (if any) happening?  If it's in the application, well, we're running Java 6, which means that (according to [slide #11](https://perf-metrics-velocity2012.appspot.com/#11) GZIP is blocking until the stream finishes).  Could matter!

The speaker did mention, a couple of times, a packet loss rate of 1%.  I'm curious, and have asked on Twitter, if that's a number for demonstration or a common number from experience.  Being from Google I wouldn't be surprised if it's the latter, but if so, man, y'all have some crappy network connections :)

## [A Web Perf Dashboard: Up & Running in 90 Minutes](http://velocityconf.com/velocity2012/public/schedule/detail/24825)

I was really looking forward to this.  So, imagine my surprise when instead I spent the time in the hallway VPNed into work.  Hmf.  I'll hopefully read through these later.

## [11 Ways to Hack Puppet For Fun and Productivity](http://velocityconf.com/velocity2012/public/schedule/detail/23639)

I loves me some Puppet, so I had to go to this.  Honestly, it wasn't awesome.  The talk was maybe 30% ways to hack on Puppet and 70% "hey, Puppet is pretty awesome, check this out".  I agree with the latter, but I was hoping for more technical hands-on material out of a "Tutorials" session.

That being said, though code in a slide is rarely awesome, it did inspire me to write a few custom facts for our Puppet environment.  I suppose that means it did the job?  I suspect I'm relying on custom facts instead of getting Hiera working; we'll have to do that soon as well.

## That's it.

After some more work email, I decided to leave early and get some coffee and laptop time in.  I could have done the latter at the con (though, Velocity, why would you put the coffee away after noon?!  Some of us caffeinate early **and** often), but, eh.  It's looking like I might have to take tomorrow morning off to do work stuff as well.  I hope not (not a great use of my employer's $1500 of registration), but, that's the life of the IT guy.

