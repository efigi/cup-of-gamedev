---
layout: post
title:  "The Importance of Software Accretion"
description:  "Software Accretion is an important concept in Software development! You should apply it to your workflow!"
author: remtaine
categories: ["Programming Principles"]
image: assets/images/pearl.jpg

tags: programming principles createJS Javascript HTML5 software accretion featured
---

A few years ago, when I first took a dip into game development, I got started on a game. It seemed simple enough; it was a top-down game where the player could dash around the map like lightning and zap down enemies. I have made games in this genre before and so I know what the initial steps were.  I've already imagined the flow of the game so it was all a matter of just coding it. I sat down and started, checking Google every now and then for the Javascript and CreateJS code needed (I was developing an HTML5 game) for the methods that I had forgotten the syntax of. After some time, I was done. I loaded the HTML page with the JavaScript file linked, and guess what I saw?

A white page.

Of course, I wasn’t that surprised since I wasn’t expecting to have written the code perfectly. Some bumps here and there were to be expected. I went back to my code and scanned it to see what was wrong. I was hoping it was a mere syntax error or something similar.

It wasn’t. My syntax was correct and all my code seemed to make sense to me. I checked my code several times over and I couldn’t see anything wrong. And yet, it that white page was still there, taunting me. It was telling me something was wrong, and I didn't know what.

## Building Huge Blocks

My problem was that I built it in one huge block and not haven't bothered to test it step by step. I made the entire program before even seeing if it could manage to draw anything. Once all that was done, only then did I test it out. Since I had the entire code base be a possible source of bugs, to be able to test this properly, I had to comment out large amounts of code just to check if the bare-bones product worked. Since the program isn’t that big anyway, I simply scrapped the lot and started anew.

This wouldn’t have happened if I just did software accretion.

## What is Software Accretion?

Software accretion was a concept mentioned in Code Complete as a metaphor for making a program. The book described this concept as:

> Accretion [...] means any growth or increase in size by a gradual external addition or inclusion. Accretion describes the way an oyster makes a pearl, by gradually adding small amounts of calcium carbonate.

XXX

The method of software accretion is essentiall two parts: first, building an MVP or minimum viable product, then adding more and more features.

## Minimum Viable Product

The book describes this step as:

> In [software accretion], you first make the simplest possible version of the system that will run. It doesn’t have to accept realistic input, it doesn’t have to perform realistic manipulations on data, it doesn’t have to produce realistic output—it just has to be a skeleton strong enough to hold the real system as it’s developed. It might call dummy classes for each of the basic functions you have identified. This basic beginning is like the oyster’s beginning a pearl with a small grain of sand.

XXX

## Add Bit By Bit

The book describes the second step as:

> After you’ve formed the skeleton, little by little you lay on the muscle and skin. You change each of the dummy classes to real classes. Instead of having your program pretend to accept input, you drop in code that accepts real input. Instead of having your program pretend to produce output, you drop in code that produces real output. You add a little bit of code at a time until you have a fully working system.

XXX

Software development like this, with adding each tiny feature, makes debugging way easier. It also allows us to check mainly the code added after the last debug,so debugging would be more organized due to adding code parts at a time.

This also forces the programmer to see what is core to the program, seeing what is needed and seeing what is merely an add-on. This is useful especially for those programmers with a deadline, as feature creep (adding more and more features) is a huge cause of delays. Adding it one by one will keep the important parts in the program, so if any parts are missing during launch, it won’t be that bad.

## More Necessary Than You Think

This concept is more necessary than you think, and should be applied more often. I can't mention to you the number of times I've been following a tutorial for a specific part of the game that's several pages long, but could only be compiled at the end. I understand if it was an intermediate tutorial, but beginner's tutorials have this problem as well. This problem is even worse for newcomers as once they type everything, once an error comes they will have no idea where to start tackling it.

This doesn't just apply to game development by the way, this concept applies to all facets of programming. I'm sure all developers have had a moment where they were tempted to just start the project from scratch, since they just couldn't find what part was working. They have made the code so big without checking it every step, that when a problem comes along they don't know where to look first. That's why an addendum to software accretion is that once you find a bug while programming something, tackle it right away while the codebase is minimal and it's still fresh in your mind. Trying to bury it will only give your future self a bigger headache.

## How I applied it

I forgot about applying this to my coding since it’s been a while since I programmed, but I won’t again. Doing anything else simply isn’t worth the trouble.

Once I rebuilt the code using the principle of Software accretion, things became smoother. I could easily tell when a bug showed up, and I knew immediately which lines of code were at fault. Well, most of the time anyway.

## Software Accretion Everyday

I'm glad that in the end I managed to fix it but next time, I'll build it a bit at a time, checking it every step of the way. That way, I know that something works before I go to the next part. It saves on a lot of development time, and is overall a better way of coding.