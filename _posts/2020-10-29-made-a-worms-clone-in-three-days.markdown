---
layout: post
title:  "Making A Worms Clone in Three Days"
description:  "Worms is a turn-based tactical artillary game loved by millions around the world. Let's see how to make one!"
author: remtaine
categories: ["Game Jam"]
image: images/worms_clone_bombs_equals_magic_v1.png

tags: gamedev worms postmortem clone game jam 2D Godot featured
---

Hi guys! So I made a tactical artillery game like Worms/ Gunbound/ Arcanists. It was for a game jam that lasted 7 days but I joined late, so I just made this game in 3 days. It was still pretty fun though! I learned a lot from making this, so I want you to see how it was made as well.

## Breaking It Down

When you break down Worms, Gunbound, Arcanists, or any turn-based artillery game, you essentially get: a turn-based platformer with a destructible environment and varying weapons.

## A Rudimentary Platformer

For the platformer part of worms, I would say that it’s rudimentary compared to pure platformer-based games as they tend to remove the mechanics that make platformer movement more crisp. Things like coyote jumps, jump buffering, acceleration on movement, air control, and such are removed. This basic movement is done on purpose to make positioning harder, and makes the player more reliant on proper weapon throwing mechanics.

## Turn-Based Mayhem

The turn-based part was theoretically pretty simple, though I did have some trip ups over here. I personally think that it’d be best to do the real-time version of the game, then implement turns afterwards. It’s essentially only allowing one person at a time to move, and having a signal sent when the turn is done to make the next character move. I mainly had trouble with handling turn order once someone would die, but that was fixed soon enough.

## Destructible Environments

The hardest part to implement the destructible environment. I’ve read up on several ways to handle it (Bitmasks, marching squares, etc.) though in the end I just went for the geometric method mentioned by Mitch Makes Things in his <a href="https://www.youtube.com/watch?v=q9SV4o7ZZNk">Youtube Channel</a>. Essentially he just created a custom collision polygon from the image, then whenever there was an explosion he would remove the endpoints of the collisions from the polygon. It’s pretty neat, you guys should check out that link. He can explain it way better than I can.

## Weapons That Shock And Awe

The weapons were important to make. Ideally I would have huge weapon variety to allow interesting gameplay, but for the game jam I wanted to implement the basics, so I started with a grenade. I started it as a Kinematicbody2D, but after trying to implementing proper bouncing for a while, I realized that making it a Rigidbody2D would make things way easier.

## AI Mishaps

One thing that I knew would be hard but got me stumped as to how hard was the AI! Calculating how to properly lob grenades was more difficult than I imagined. In the end I just made the enemy AI use a completely different weapon, an orb that deals low damage and small knockback/explosion, but can go through obstacles. I’d just like to say that this weapon is still hard to use for a human due to its launch mechanics (still have to estimate distance from enemy). Ideally I would learn to properly calculate this using physics, but I had to rush due to being in a jam. I’ll probably do proper calculations in the future.

## Building For The Web

As for the builds, one thing that made me sad was that the destructible tiles didn’t work in the HTML5 version of the game, probably due to the geometric functions. It made me sad since I usually have more people play my game in the HTML5 build, but I’m still happy that I got to make the game.

## Plans For The Future

In the future, I plan to add lobby-based multiplayer, more weapons, larger and more varied maps, and probably some more juice. I’d also see about exporting this to mobile. Please tell me your thoughts on what I have so far as well as these plans :)

You can check out the game at the <a href="https://remtaine.itch.io/bombs-equals-magic">Itch.io</a> website.

PS. the title is “Bombs = Magic” since you’re going against magical mushrooms using only bombs, and you’re there to show them who’s boss!
