---
layout: post
title: "Adding a Flag and Figuring Out What We're Doing Next"
date: "2017-06-26T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Level Design, Gauntlet, Lord of the Rings, Getting Stuck]
excerpt: "Today, we continued Adam and my list of things to accomplish with this game."
images: [[OutsideCastle.png],[BacksideCastle.png],[Texture.png],[Flag.png]]
---

Today, we continued Adam and my list of things to accomplish with this game. The first item was accomplishing a bigger map with multiple zones/spawner areas where you have to destroy so it's like Gauntlet. Where the enemies infinitely spawn in until you destroy the spawner. So, I started creating a small ramp that comes off the edge of one wall of the castle. This ramp was basically a bridge that connected to an open field with a 2x3 block castle. I made the castle big enough to be able to have enemies spawn throughout it and then walk up the ramp on the back and walk around. Which is what we want so it's just a regular castle but it has a ramp to the outside. 

{% include image.html filename="OutsideCastle.png" description="Outside Castle" %}
{% include image.html filename="BacksideCastle.png" description="Castle Inside" %}

While I was doing this, Austin drew up a design for the enemy flag so I could import it as a texture and put it on the flag asset. He airdropped me the picture of the hand that was the orc flag from LOTR (you should know). I added the texture to the flag material and then I figured I need to multiply it by the other texture and it worked. But, the texture of the hand was too big and it tiled weird, so we did this:

{% include image.html filename="Texture.png" description="Code needed to place texture on top of texture" %}
- Open Image in New Tab to see ^ 

We basically appended two constants (bottom left, 0.005069 and 0) into one and then added the TexCoord to that. The TexCoord would offset the value of the scale of the X and Y of the texture to whatever number we would put in. So we made the Y tiling 0 and the scales to be 1.4.

This is what we got:

{% include image.html filename="Flag.png" description="Flag placed in world" %}

Then we started getting in a rabbit hole when I tried adding another character with a different mesh, sword, and everything so we decided to make a blueprint component that has all of our variables. Which is what we're doing tomorrow.