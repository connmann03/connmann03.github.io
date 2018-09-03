---
layout: post
title: "Spawner Effects and Power Meter Fixed"
date: "2017-07-28T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Hyrule Warriors, Enemy Design, Level Design, Materials, Animation, Controls, Attack Design, Meters, Programming Fundamentals]
excerpt: "Today's work involved making cool spawner effects and fixing the power meter."
---

Today's work involved making cool spawner effects and fixing the power meter. We created a list today that included; making power move work with Level 3 attacks, make spawners fly in and drop down, move kill count function before death animation, when the death animation is called disable physics, and the switcher working on the side of the screen. The things we accomplished today were everything besides the switcher working on the side of the screen.

First thing I did was move the kill count function and disable physics to the enemies of death. I did those easily then I moved onto the spawners flying in since that one isn't that hard and I can handle it. 

After working on the flying in and getting it to work, I needed for it to materialize in to look like it's gathering some sort of energy as it's 'teleporting' in. After getting the materials made and making it work Austin had to fix the timelines for it to be smooth on the return to set the arch to be the normal material (it doesn't make sense but it will when you see it). Next, Austin said the portal needed to have camera shake, dust clouds spawn under it as it lands, and lightning bolts to 'shock' it in. I did this easily I just had to figure out the positions and values.

Next, Austin hooked up the Level 3 attacks to the Power Meter. 

This video is what I accomplished today, but I disabled enemies so you can see the major things accomplished (ignore lag).

{% include youtubePlayer.html id="P5F29Q3cZrc" %}