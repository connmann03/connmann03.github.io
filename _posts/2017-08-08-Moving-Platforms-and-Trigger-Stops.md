---
layout: post
title: "Moving Platforms and Trigger Stops"
date: "2017-08-08 20:38:32"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Super Mario 3D World, Level Design, Mechanics, Platformer, Splines, Sequences]
excerpt: "Today's work involved making a moving platform like in Mario."
images: [[splinemovement.png],[stop.png]]
---

Today's work involved making a moving platform like in Mario. The way I did it is use a spline and a static mesh component inside the same blueprint. I then did a timeline of 0-1 in a 5 second interval and then looped it with a sequence on completed. It would move end to end in 10 seconds total.

{% include image.html filename="splinemovement.png" description="Moving Platforms Using Splines" %}

Then I made trigger boxes it stops in for a second then starts back up. My problem is that on reverse it reverses back to the recent spot instead of continuing the path which I have an idea how to fix.

{% include image.html filename="stop.png" description="Trigger box for stop" %}