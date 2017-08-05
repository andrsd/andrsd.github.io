---
layout: post
title: Laundrification
Date: 2017-08-05 15:00 -0700
tags: "DIY"
---

If you are like me and forget things, this might be useful.  When I used to do laundry,
I'd put the cloths in the washing machine, but then I would go do something else and
I'd forget about it and then missed the step of putting the cloths in the dryer.

So, I was thinking how to prevent that.  Obviously, I could buy an expensive smart
washing machine that would be connected to my WiFi, talk to some cloud service and whatnot.

Or, I could do something myself about it. And that's how laundrification came about. It is
not my idea, I found a similar approach on the internets, but the solution were not what
I wanted, so I did my own version.  The idea is simple: use photo resistor to measure light
coming from the LED that indicates the cycle finished. When the light comes on, send a
notification to my phone.

One needs a WiFi enabled circuit like Arduino MKR1000 and use IFTTT webhooks service (formely
maker channel) to trigger the notification.  Sending a http request with Arduino is trivial,
and the platform is simple to work with. That's why I chose it.  I played with other smaller
and cheaper boards, but I only managed to fry them. However, the idea should still work, if
you do not want to use Arduino which is more expensive. You can also use a different webhook
platform. I used IFTTT because I already had an account there.

The project lives on [github][1].

[1]: http://andrsd.github.io/laundrification/
