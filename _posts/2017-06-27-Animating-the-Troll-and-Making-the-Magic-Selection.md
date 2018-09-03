---
layout: post
title: "Animating the Troll and Making the Magic Selection"
date: "2017-06-27T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Animation, Montages, Locomotion, UI, Widgets, Graphic Design]
excerpt: "Today's work involved getting the troll boss to have an animation blend, montages, and an animation blueprint."
images: [[trooll.png],[ui.png]]
---

Today's work involved getting the troll boss to have an animation blend, montages, and an animation blueprint. I first started creating the animation blendspaces for the troll. I added the idle animation, turn left, turn right, move left, right, forward, and backward. Then, I moved the animations in the -200 by 200 space to match the knight's blendspace since it is a good example. But, I had to modify the turning and add more move left and right ones. This worked so I moved on to the animation blueprint which holds the blend between moving and poses for the montages. 

I made the locomotion have a movement variable called local velocity that would change based on the movement and it was hooked up to the movement blendspace for the troll. Then I added a locomotion pose called upperbody and another named full body. This would split fullbody animations (dying, taunt) from the upperbody animations (swinging sword, etc.).

After that we did an animation montage for the sword swinging (also dealing damage), victory, death, and flinching. Using Anim Notifies, I made notifies if things happened in the montage.

{% include image.html filename="trooll.png" description="Troll Blend Space" %}

Next, we, Austin and I, spent several hours solving how to put blueprint structures inside of each other, then to be able to have a UI item be interchangeable on the fly so it is better if we get more spells(later on, easier now). Our outcome was insane since we are able to scroll down now but the items get added by pressing 1.

{% include youtubePlayer.html id="srlseiytxtY" %}

{% include image.html filename="ui.png" description="Insane UI" %}
