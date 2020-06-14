---
layout: post
title:      "Building a browser-based game with a Rails API"
date:       2020-06-14 10:21:01 -0400
permalink:  building_a_broser-based_game_with_a_rails_api
---

Using a Rails API basically means:
Rails communicates with my database, passing JSON formatted data to my frontend for game manipulation. For this project, I used Fast JSON as a serializer, even though it didn’t feel necessary, I wanted to get practice with this serializer!

The main components of my game include:
* a PostgreSQL database
* a Rails API
* main HTML document

To bring this all together I used Javascript in my frontend for logic/functionality.

### Model-based programming (OOJS)
Using Object-Oriented programming to organize and build my game logic was definitely the best decision. Once I started to get halfway through this project, I realized just how crazy my files could have gotten without some organization in place.

**Components**
* **game.js** my main game class, which starts up my game, and calls on other functions/classes
* **doctor.js** a game piece that avoids obstacles
* **input.js** the input handler for my Doctor class (movement/keystrokes)
* **pathogen.js** the obstacles in my game, RED
* **index.js** calls my main game class, starting the game

**Adapters**
My adapter files basically handle all my fetch calls to the database. They are instantiated at the beginning of the game so that I’m able to use them throughout the file.

### Things to Familiarize yourself with, when you’re just starting
* [HTML5 Canvas](https://www.w3schools.com/html/html5_canvas.asp): handles rendering for our game
* [Game States](https://codeincomplete.com/articles/javascript-game-foundations-state-management/): monitoring and managing data/the main game screen
* [The Game Loop](https://developer.mozilla.org/en-US/docs/Games/Anatomy): renders animations/games with changing state over time


### Stretch Goals
For stretch goals, I’d like to add more complexity to my game by adding different types of game pieces. Right now I just have obstacles that the doctor is trying to avoid, but I would want to add in “good” pieces that, if eaten, give the doctor extra points. 

I would also like to do a bit more styling and switch out my game pieces, which are currently just cubes, for sprites or png images. 


