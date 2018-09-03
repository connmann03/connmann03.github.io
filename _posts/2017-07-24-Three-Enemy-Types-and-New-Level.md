---
layout: post
title: "Three Enemy Types and New Level"
date: "2017-07-24T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Enemy Design, Hexen, NavMeshes, AI, Level Design]
excerpt: "Today's work involved completing the three enemies I need to be able to have a basic demo for our game."
images: [[topview.png],[stairwell.png],[inside2.png],[insideview.png]]
---

Today's work involved completing the three enemies I need to be able to have a basic demo for our game. I finished these three types: one being the troll, ground worm, and flying worm that shoots at a distance. Right now it doesn't really float but it's collision makes it "float".

Here's the checklist I used to build the three enemies:
```
Things You Need To Create an Enemy

-Model, textures, animations
-Animation blueprint with fullbody pose, upperbody pose, animnotifys set, and locomotion
-Animation montages of the attacking(you need to add anim notify of DealDamage and called through animation blueprint), death, and flinching
-Animation blendspace of the walking
-Character blueprint(duplicating a previous one) and rewiring it to have the animation blueprint set, the mesh, texture, ai controller, and animations montages wired up to be the characters own.
-AI Controller with it only saying run the characters behavior tree.
-Copy the behavior tree default functions and edit them for the new character.
-Duplicate the behavior tree and edit it with the new functions.
-Put NAVMESH
```

Next, I created a map. This map is based off of the game Hexen where they have giant rooms and smaller rooms with passage ways.

{% include youtubePlayer.html id="tETrdn48QYE" %}

I made this giant map (isn't complete) but I need to add lighting, spawners, debris, and more to make it actually good looking and like Hexen.

{% include image.html filename="topview.png" description="Top View" %}
{% include image.html filename="stairwell.png" description="Stairwell" %}
{% include image.html filename="inside2.png" description="Inside Top" %}
{% include image.html filename="insideview.png" description="Inside Bottom" %}