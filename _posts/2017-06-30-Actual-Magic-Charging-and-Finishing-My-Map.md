---
layout: post
title: "Actual Magic Charging and Finishing My Map"
date: "2017-06-30T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Level Design, Programming Fundamentals, Controls, Lord of the Rings, Particle Systems]
excerpt: "Today's work involved changing the entire magic charging system since the way it works, it doesn't change the particle."
---

Today's work involved changing the entire magic charging system since the way it works, it doesn't change the particle. I tried the day before to change the particle to shoot on the fly by hold time of right click but was unsuccessful. Today, Austin decided to come to my desk and rework my entire charging logic for me since I probably wouldn't be able to do it. He figured out if you go in the KGCharacterBase and change the LaunchMagicProjectile event to have a variable that would be a particle system and would change by getting the player controller hold time. Next, he went to KGProjectileBase and called that variable from the character on beginplay, which is on spawn of the particle.

{% include youtubePlayer.html id="C7ObP2HG4f4" %}

In this video you can't see the text in the top left, but it displays the amount of time the player held down the right click button. The 3 different particles were because of the hold time variable and switching right before the particle is spawned.

After this, I finished my map. I added lights, made it run faster by replacing all the small blocks stacked up on top of each other with actually castle walls and kept some of the blocks for the floor. This took forever to build the lighting but was worth it since it looked epic.