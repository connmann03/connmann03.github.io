---
layout: post
title: "Rewiring Attacking and Quake"
date: "2017-07-21T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Level Design, Programming Fundamentals, Controls, Quake, Behavior Trees, Service, Decorator, Collisions]
excerpt: "Today's work involved getting a character to attack through the behavior tree we created yesterday."
images: [[suttgf.png]]
---

Today's work involved getting a character to attack through the behavior tree we created yesterday. It took awhile of understanding but I had to rewire the behavior tree with some more complicated stuff.	I had to add a Service which is basically a condition that runs every tick interval you set. This service finds the player and the AI and sets these variables in it to the ones in the Blackboard. And then I needed a linetrace for collision with the player. Next we had to add a selector that if the target is set then run a "decorator" which is another custom event and then run MoveToPlayer. It's easier to understand visually. Next, we got if the AI is at the TargetLocation and set it to true then move to player. We also had to set the TargetToFollow to "is set to" (aborts both) which makes it run through both selections. 

{% include image.html filename="suttgf.png" description="Rewired Behavior Tree" %}

The video shows what this does. Ignore the buggy animations. That's because of the animation blend being messed up.

{% include youtubePlayer.html id="RBpq-XwY1kU" %}
