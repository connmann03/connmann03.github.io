---
layout: post
title: "Different Stages of Magic Effects and Planning Spawner"
date: "2017-07-03T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Level Design, Programming Fundamentals, Controls, Lord of the Rings, UI, Widgets, Particle Systems, Materials, Brainstorming]
excerpt: "Today's work involved configuring the attack list and stages of magic effects for each type and getting particle effects made/set."
---

Today's work involved configuring the attack list and stages of magic effects for each type and getting particle effects made/set. I started out by searching "fire" in the InfinityBladeEffects folder that Epic Games gave out. I found 3 good evolutions of attacks for fire. One a simple fireball, a flamethrower like attack, and a flame wall which I thought would be a cool attack for number three. A huge fire wall. That would be awesome! So, I did what Austin set up previously and made children of the ProjectileBASE called ProjectileFIRE_01-03. I assigned the particles in those 3 blueprints respectively, made adjustments to the velocities, and bounciness if needed. I then did that for ice and electricity. But, we have a particle called "bear". We thought it would be cool to summon some sort of animal to hurt the enemy. So, I got the bear skeletal mesh and made a material that's semi-transparent and looks like a grid. This is what I got: 

{% include youtubePlayer.html id="8y-Ns_WAnXY" %}


After that, we planned out the enemy spawner. It will spawn an actor of class every couple seconds if the player gets closer to it.