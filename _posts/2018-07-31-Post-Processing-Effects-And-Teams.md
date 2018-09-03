---
layout: post
title: "Post Processing Effects And Teams"
date: "2018-07-31"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Design, Level Design, Thief, Stealth, Post-Processing, Teams]
excerpt: "Today's work involved working on the level to make it more immersive so it looks like you're actually trying to pull a prank at night."
images: [[2018-07-31 Nightsky in Skybox.png]]
---

Today's work involved working on the level to make it more "immersive" so it looks like you're actually trying to pull a prank at night. I made the sky dark and have the stars show and it looks really cool. I had to watch a video on post processing settings to change and play with to get the scene to look realistic and neat. I then was able to get it to look really good but I can still play with some exposure values and sky tints.

{% include image.html filename="2018-07-31 Nightsky in Skybox.png" description="Nightsky in Skybox" %}

After that I was getting different teams setup and (right now) through a widget blueprint you select a team and that spawns you in a certain spot, in the house or outside. It took some work getting it to replicate. It was me and Adam just testing out what was wrong. We narrowed it down to the point when the reason it was wrong was because of references and how my code was setup.

{% include image.html filename="2018-07-31 Team Spawners.png" description="Team Spawners" %}

{% include image.html filename="2018-07-31 Team Select.png" description="Team Select" %}

{% include image.html filename="2018-07-31 One Player Spawning in Each Spawner on Two Clients.png" description="One Player Spawning in Each Spawner on Two Clients" %}
