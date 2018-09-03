---
layout: post
title: "Getting The Cameras To Work"
date: "2018-07-20"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Thief, Cameras, Design]
excerpt: "Today's work involved getting the cameras to work and display correctly on the screen."
images: [[2018-07-20 Security Desk.png],[2018-07-20 Possessing Desk Screens.png],[2018-07-20 Pan Tilt Zoom Control of Screen on Camera.png]]
---

Today's work involved getting the cameras to work and display correctly on the screen. Shortly after explaining my work to Austin and problems, I tried something inside the camera blueprint. It creates a new texture on beginplay. And that worked somehow. I then made a desk that you can view 6 cameras from. It gets the cameras in the world and then when the player collides with the desk(for now) it takes input from the character and he/she controls the desk. After that, the player can select a screen with WASD and press TAB to take control of it. Then WASD to move the camera around, and QE to zoom in and out. Each of those inputs is clamped. 

{% include image.html filename="2018-07-20 Security Desk.png" description="Security Desk" %}

{% include image.html filename="2018-07-20 Possessing Desk Screens.png" description="Possessing Desk Screens" %}

{% include image.html filename="2018-07-20 Pan Tilt Zoom Control of Screen on Camera.png" description="Pan Tilt Zoom Control of Screen on Camera" %}