---
title: "Ants vs. SomeBees"
date: 2019-10-18T10:07:47+06:00
draft: false

# post thumb
image: "images/ants.jpeg"

# meta description
description: "CS61A Ants Project"
summary: "Inspired by the game Plants vs. Zombies."
author: "Jeffrey Sung"

# taxonomies
categories: 
  - "Structure and Interpretation of Computer Programs"
tags:
  - "Game"
  - "Python"

# post type
type: "post"
--- 

### Summary
This plays essentially exactly the same as the original Plants vs. Zombies tower defense game. The only real differences are that I added some more complex mechanics (EX: minions that don't damage but apply certain status effects), and, of course, visuals. It was good practice using an object-oriented programming paradigm.  

What I did:  
- Designed "minion" objects (attributes include health, hunger, strength, etc.), utilizing inheritance
- Track game state (position of entities, time left, resources left, etc.)