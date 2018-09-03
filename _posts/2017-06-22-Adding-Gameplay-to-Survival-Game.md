---
layout: post
title: "Adding Gameplay to Survival Game"
date: "2017-06-22T16:11:58+05:30"
projects: [Horde Survival Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, AI, NavMeshes, Animation, Montages, Skeletons, Level Design, Particle Systems, UI, Widgets]
excerpt: "Today's work was completing the entire Udemy course which involved finishing the survival game I started."
images: [[wow.png]]
---

Things I learned today: 

- Animation Montages
- Adding sockets to skeletons
- Changing AI pathways to detect if the player is nearby
- More Particle Effects
- Exporting Particles from other systems into another system
- Adding UI Widgets above the player
- Adding a "progress bar" widget but it's basically a health bar

Today's work was completing the entire Udemy course which involved finishing the survival game I started. I first added a sword to the player which had collision to everything but the owner of it, or the controlled pawn. The way we attached the sword to the player was by attaching a socket to the skeleton of the player and making the "socket preview" be our sword and we would make the transform fit the player's hand perfectly. Next, we added so the sword applied damage to the enemy or us if we get hit by AI. Next, we made the AI attack us and pursue the player if they're in range. Then attack the player with the sword dealing the same amount of damage, 50.

Next, we made it so the player can use a magic attack with right click. We made a particle system thats a spiraling ball that is reddish and has collision. Then we did we a thing in a blueprint of the particle that basically applies velocity in a certain vector so it shoots out in that direction on play. So, we made it so when the player presses right click, it charges up with another particle system thats on the foot and on the hand for a cool effect. Then, when it finishes the hand of our player moves forwards shooting the fireball at the enemy and it deals 50 damage.

After that, we had to make the health bar. We did this by making a UI Widget which includes a "progress bar" that hooks up straight to the player health and it displays their current health with that value on the bar. And then we applied this to the character base so it's above their head. 

{% include image.html filename="wow.png" description="Wow! A Working Health Bar!" %}

We also added some animations like death animation and if the player is hit then they flinch.

{% include youtubePlayer.html id="apOD_gZZPzQ" %}