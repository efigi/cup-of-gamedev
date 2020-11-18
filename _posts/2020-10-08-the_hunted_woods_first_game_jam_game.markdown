---
layout: post
title:  "Lessons Learned From My First Game Jam Game With A Team"
description:  "Working with a team for the first time can be daunting! But with patience and some leadership you can get everyone to make a great game!"
author: remtaine
categories: ["Game Jam"]
image: assets/images/the_hunted_woods_v1.jpg

tags: games showoff gamejam postmortem horror 2D Godot
---

So I entered the Weekly Game Jam Week 147. This was my 2nd game jam, but my first one using Godot. My first one was made in Gamemaker, and while I think it was pretty decent, it's a pretty small game. I liked the mechanics, but there were only a few levels, and most were pretty easy.

## Engine of choice

As for the engine, Gamemaker has the ability to prototype rapidly, which I think makes it a great choice for game jams. I managed to create the mechanics fairly quickly then proceeded to add on from there. With Godot, I was hoping to replicate the same fast prototyping of Gamemaker and more.

## Forming The Dream Team

I formed a team through the Discord channel, getting two sounds people to work with me. No graphics guy, but I wasn't worried since I was sure we could find the proper assets. With the theme of "Invisible", we went with the natural "invisible monster route" (like legit, I saw sooo many games submitted for this jam related to an invisible monstrosity).

## Music = Horror?

Due to our team having two sound guys, we were amenable to the idea of a horror game. The genre is really music and sound-dependent, so we would be playing to our strengths. We went for the core mechanic of things being invisible until you flash light on them, which seemed to fit in a horror game. It'd also work with the idea of an invisible monster.

## Godot's Pretty Intuitive

For the implementation, what I like about Godot is due to its scene and nodes system, it's actually pretty intuitive and fast to create prototypes for games. Not only that, polishing graphics or improving movement can usually be solved through adding a node.

## Godot vs Gamemaker

One advantage of Godot over Gamemaker is the AnimationPlayer node. It's so useful! It makes making animations a breeze, and really adds to the polish in movement. (Update: the recent build of Gamemaker finally has animations, but it's been a while since I've used Gamemaker)

## Lighting Makes Things Scarier!

I also have to say that I love the lighting in this engine! It made my light mechanics relatively simple to implement. Using the Light Mode of "Light Only" in a CanvasItemMaterial easily made our core mechanic of needing a flashlight to see things. Unlike in Gamemaker where I have to make a light system from scratch, this came out of the box and worked for my purposes.

## On Schedule!

We managed to finish in time, and we added a lot of stuff to the game. That's all thanks to Godot's fast and intuitive way of handling things.

## HTML5 Build Fail

The only part that made me a bit sad was the HTML5 build of the game. It was smooth on Windows, but really laggy on HTML5. I've seen multiple posts regarding SCons for removing unneeded features in the final build to improve performance, but since I was in a game jam I didn't want to spend extra hours on this when I could be improving game features. I've read that Godot will be moving to Vulkan soon though, so I'm not worried.

## The Game Itself

Here's my game if you want to try it. You can find it on the <a href="https://remtaine.itch.io/the-hunted-woods">Itch.io website</a >.
