---
layout: post
title: "Bug Fixed And More Multiplayer"
date: "2018-07-25"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Bugs, Thief, Stealth, Research]
excerpt: "Today's work involved me waking up to start solving this bug of where the render target textures don't build after packaging the game."
images: [[2018-07-25 Screens Working in Multiplayer Build.png]]
---

Today's work involved me waking up to start solving this bug of where the render target textures don't build after packaging the game. I first downloaded the "Blueprints" content example for Unreal. The reason I downloaded this is because it has a security camera blueprint and screen I can mimic some of the elements onto my blueprint. I saw it selects cameras in the world not by "GetAllActorsOfClass" but by manually selecting them in the world by making the array Expose On Spawn. And then creating a different Texture Render Target for each one. Then, after making it work, it started glitching. I tested changing the texture size and it fixed by changing it from 256 to 512. Don't know why, but it fixed.

After that we went house hunting like the HGTV show. And then after that I was trying to make possession of the right pawn after trying to stop using the screen table. It works for the server but the client. I think is might be because they're on the same computer but it might not be.

Here's a picture of the screens working on multiplayer on builds too.

{% include image.html filename="2018-07-25 Screens Working in Multiplayer Build.png" description="Screens Working in Multiplayer Build" %}