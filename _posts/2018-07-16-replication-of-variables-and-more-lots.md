---
layout: post
title: "Replication of Variables and More Lots"
date: "2018-07-16"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Multiplayer, Replication, Bugs, Programming, Wondering in the Woods, Reading]
excerpt: "Today's work involved reading the UE4 Network Compendium"
---

Today's work involved reading the [UE4 Network Compendium](http://cedric-neukirchen.net/Downloads/Compendium/UE4_Network_Compendium_by_Cedric_eXi_Neukirchen.pdf), a short little book about networking in Unreal Engine 4. It discusses mostly everything briefly and some main things more precisely.

After I read the 112 pages, I began finishing getting a timer to replicate onto the clients. I figured out the [Unreal Documentation had a replicating variables section](https://docs.unrealengine.com/en-us/Gameplay/HowTo/Networking/ReplicateVariable/Blueprints) and the example they used to showcase it is a timer. I replicated the example in my blueprint and fixed some things and got it working.

Then after that I had to move the durability removing/collision detection to the server by moving the durability remove code to the fences, trees, and pools.

Then added more timers and got the text in the world to be the player's color, but there were bugs we discovered while playtesting. The mouse cursor wasn't capture in fullscreen mode, the grass wasn't replicated on rejoin, the powerups weren't replicated, and the powerups made the player too big. I will fix these issues tomorrow.


