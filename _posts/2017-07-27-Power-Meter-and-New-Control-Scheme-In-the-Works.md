---
layout: post
title: "Power Meter and New Control Scheme In the Works"
date: "2017-07-27T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Hyrule Warriors, Controls, Attack Design, Meters, Programming Fundamentals]
excerpt: "Today's work involved making a power meter for the ultimate attack or third level attack so the game isn't so slow."
images: [[powermeter.png],[pressedboth.png],[bool.png],[print.png],[endpart.png]]
---

Today's work involved making a power meter for the ultimate attack or third level attack so the game isn't so slow. We came up with this idea and we made it work by pressing the left and right click at the same time. The way it works is with booleans so if one is pressed, not released, it assigns the boolean to true then on release it makes it false. So I did that for both button actions but they're two different booleans so if left click is detected click first then it will work since it sometimes has to be one before the other. 

{% include image.html filename="powermeter.png" description="Power Meter" %}
{% include image.html filename="pressedboth.png" description="Pressed Both" %}
{% include image.html filename="bool.png" description="Boolean Logic" %}
{% include image.html filename="print.png" description="Print Logic" %}
{% include image.html filename="endpart.png" description="Set Charge to 0" %}

When you kill an enemy you gain one point out of a variable I created that you can change. Right now it's ten for max. And when you kill a spawner it gives you three points but you can change it since it's a variable.