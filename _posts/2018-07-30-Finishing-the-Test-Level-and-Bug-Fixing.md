---
layout: post
title: "Finishing the Test Level and Bug Fixing"
date: "2018-07-30"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Reflections, Quaternions, Light Mass, Design, Level Design, Thief, Stealth]
excerpt: "Today's work involved trying to get the test level finished and fleshed out to test gameplay."
images: [[2018-07-30 Camera Rotation Bug Fixed.png],[2018-07-30 Test Level Overview.png]]
---

Today's work involved trying to get the test level finished and fleshed out to test gameplay. I was able to fix reflections, get security cameras in there, light mass importance volume, and some other things like trees. When I was testing the level, I noticed a security camera bug where it won't rotate correctly because of how Unreal Engine works. The coordinate system uses a -180 to 180 instead of 0 to 360 system. So I had to code around it. I had to force it where it would do if statements to check if the player is pressing a certain key like "A" which is -1.0 in input so it would check if the input axis is == to -1.0 and if the position of the camera is = to, stop it. It worked. 

{% include image.html filename="2018-07-30 Camera Rotation Bug Fixed.png" description="Camera Rotation Bug Fixed" %}

{% include image.html filename="2018-07-30 Test Level Overview.png" description="Test Level Overview" %}