---
layout: post
title: "First Day Back"
date: "2018-07-09"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Optimization, 3D Modeling, Blender]
excerpt: "Today's work started off smooth, I started working on a lawn mowing game."
images: [[2018-07-09 Shader Complexity.png],[2018-07-09 Pool Model.png],[2018-07-09 Timer UI.png]]
---

Today's work started off smooth, I started working on a lawn mowing game. Basically the game consists of basic elements of actualy mowing a lawn with a pushmower. But, there is powerups and other obstacles you can dodge or accidentally run into. There will eventually be a time limit so the game is limited to like 120 seconds or so. But, today I added a timer that showed how long until you exit the pool, an obstacle that induces damage to the mower. When your mower reaches 0 durability, it destroys(at the moment). There are trees and fences you can run into. If you get a speed boost(they spawn after a certain amount of grass cut), you can break fences and lose zero durability but if you don't have a speed boost, you gain damage. Same with trees, but you can't break them with speed boost, it just breaks after a certain amount of hits. After while I ended up drawing a dog, I made the dog texture and then Austin told me I should download Blender and do this course I had from a while back. I started it and learned the basic controls to do basic models and then made a small house to put in the scene. I then started making a community of sorts with a pool with fences around it and then grass within it. After that we, Austin, Adam, and I, realized there was low performance with the grass meshes. We experimented with collision and placement of the meshes but figured out it was the transparency and the shadows. There is a mode in-game that shows good and bad shader complexity. The grass textures were red and that means bad and the other objects weren't read. So we turned off certain collision, didn't work, then turned off transparency and gained roughly 20 frames. Then Austin said turn off shadows and I did and it was a steady 60 frames, fixing the issue.

{% include image.html filename="2018-07-09 Shader Complexity.png" description="Grass Shader Complexity" %}

{% include image.html filename="2018-07-09 Pool Model.png" description="Pool and Mower Models" %}

{% include image.html filename="2018-07-09 Timer UI.png" description="Timer UI" %}