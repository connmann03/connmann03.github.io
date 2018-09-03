---
layout: post
title: "Continuing the Pinball Game in UE4"
date: "2017-06-15T23:55:00-05:00"
projects: [Pinball Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Splines, UI, Widgets]
excerpt: "The part of the course I'm at is making a UI system where you can type your name and it posted your highscore on the screen and menu."
---

Things I learned today:
- Mostly refresh from yesterday
- Using splines and spline meshes

Today, I continued the Udemy course involving making a pinball game from scratch. The part of the course I'm at is making a UI system where you can type your name and it posted your highscore on the screen and menu. We first started developing a simple scoring system (again to actually keep the scores and save them). We made it so the highscores are only saved locally to your machine and it only holds four values (highscores). Next thing we did was display those values through a menu system so we had to create that. 

The way we created that menu system was creating something called a Widget Blueprint. A widget blueprint is basically a regular blueprint but has a built-in "Designer" for the UI it's called. There you can drag on items which include: buttons, text, text boxes, etc. These items can be modified and altered with the script side by adding "bindings" to the text and such. That "bind" is basically a script on that object in that widget/ui system. We did that so we can call variables from the "bind" in the MenuSystem so we can hook it up to the GameMode by initiating on GameStart and GameEnd.

Also, in the UI Designer if you add a default "Text", it's a text block but if you added text like, "Score: {Score}", you can edit that in the binding you add. And that's how we did some of the bindings.

The last thing we did was doing a thing called splining/using splines. Splines are a basically a three-dimensional line segment you can edit and add segments to it and edit the position/rotation/scale and place a mesh on top of that and the mesh will morph & replace itself to connect to each other. And if you expose those segments as a variable then you can edit them for each individual of the blueprint placed in the world and the scale. That's the ramp like thing in the middle of the video below.

The cursor disappears in the game, but we're running a virtual machine so that is my machines mouse and the VM's cursor disappeared. 

{% include youtubePlayer.html id="_Z4pkB--Ax4" %}