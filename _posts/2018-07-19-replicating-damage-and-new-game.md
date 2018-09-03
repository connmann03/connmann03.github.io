---
layout: post
title: "Replicating Damage and New Game!"
date: "2018-07-19"
projects: [Mowing Game, Sneaking Game]
tags: [Mowing Game, Sneaking Game, UE4, Multiplayer, Playtesting, Replication, Bugs, Programming, Thief, Cameras]
excerpt: "I first started play testing myself and seeing what's wrong with the damage from fences, trees, etc."
images: [[2018-07-19 CamView Object Overlaying Screen.png]]
---

I first started play testing myself and seeing what's wrong with the damage from fences, trees, etc. I then realized it was the functions not replicating to the server at all and not running on the server, messing it up. I fixed it for all items and it works seamlessly. 

After that, I started on writing down ideas for a new game. It was going to be a platformer and it would be a puzzle game. I wrote down a lot of stuff and (insert picture) after a while of talking to Austin and Adam we finally came to a true concept. The game is a sort of Thief style first person game where you're trying to break into a building and steal stuff and not get caught, but the other player(s) are the security guards that patrol the area and have security cameras. I have made a prototype camera view that gets all the cameras in the world and adds a new "CamView" widget dynamically. But I can't get it to put the right texture on.

{% include image.html filename="2018-07-19 CamView Object Overlaying Screen.png" description="CamView Object Overlaying Screen" %}