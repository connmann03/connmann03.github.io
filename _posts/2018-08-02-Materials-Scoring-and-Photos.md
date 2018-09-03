---
layout: post
title: "Materials, Scoring, and Photos"
date: "2018-08-02"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Design, Thief, Stealth, HUD, 3D Modeling, Blender, Gimp, Scoring]
excerpt: "First I made a quick texture and stretched it and tiled it across my lamp's base and to make it look like light is coming out of it, I made the white spots emissive."
images: [[2018-08-02 Emissive Lamp Texture.png,Emissive Lamp Texture]]
---

Today's work involved packing up the apartment to move out...yeah sad, not really but it is kind of. But in my free time I would be watching Rush Hour 2 and working on my stealth game. The things I added were very minimal but they have slots to add some cool complex stuff. First I made a quick texture and stretched it and tiled it across my lamp's base and to make it look like light is coming out of it, I made the white spots emissive.

{% include image.html filename="2018-08-02 Emissive Lamp Texture.png" description="Emissive Lamp Texture" %}

I then added a thing where if the camera is looking directly at a player's face and the player is looking at the camera slightly, the camera user will get score. That's all the the camera thing does at the moment but what it will do in the future is copy that frame and put it onto a new texture to display at the end of the game. I also made a spot light that flashes to scare the sneaking player like a wild life camera would. I also added a score text to the hud.

{% include image.html filename="2018-08-02 Line Trace Based Score Meter.png" description="Line Trace Based Score Meter" %}

{% include image.html filename="2018-08-02 Line Tracing Face Arrow.png" description="Line Tracing Face Arrow" %}