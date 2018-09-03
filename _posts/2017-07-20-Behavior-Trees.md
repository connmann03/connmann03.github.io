---
layout: post
title: "Behavior Trees"
date: "2017-07-20T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Level Design, Programming Fundamentals, Controls, Lord of the Rings, Behavior Trees]
excerpt: "Today's work involved researching behavior trees and implementing/trying one in the game."
images: [[moveto.png],[getloc.png]]
---

Today's work involved researching behavior trees and implementing/trying one in the game. I first looked for documentation of a brief rundown of behavior trees but there was nothing. Just super complicated stuff that didn't make any sense, but would for people with prior knowledge (it even said this in the only post). Next I moved on to YouTube videos and tutorials. I found some videos that demonstrated some stuff but were super long videos just showing it off. So, I dug deeper and found a 10 minute long video just explaining some of the elements to the behavior trees. Not all of them since those are separate, longer videos. Then I found two videos that were roughly 20 minutes long that explained the aspects of the behavior tree while doing it step-by-step. It helped a lot.

I learned that a behavior tree holds the actions/tasks and runs through them in certain ways you choose. In this example we did a Sequence. A Sequence runs through the tasks you make from left to right and if one fails the entire thing fails and if one succeeds the entire thing stops, succeeding. We made one that got the player location and set it to the Blackboard. This Blackboard holds variables that are accessible throughout the behavior trees by making variables inside tasks, Blackboard Keys.

{% include image.html filename="moveto.png" description="Move To Location Behavior Tree Logic" %}

{% include image.html filename="getloc.png" description="Set Location Behavior Tree Logic" %}