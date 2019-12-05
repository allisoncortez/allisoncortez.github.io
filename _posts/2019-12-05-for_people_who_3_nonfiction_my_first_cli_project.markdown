---
layout: post
title:      "**For People who <3 Nonfiction : My First CLI Project**"
date:       2019-12-05 20:29:49 +0000
permalink:  for_people_who_3_nonfiction_my_first_cli_project
---

Our objective for this project was to build a Ruby gem that provided a Command Line Interface (CLI) to an external data source. I decided to use the New York Times API for Books.

Sidenote: I used to read a lot and it’s something I’m trying to get back into.




I’ll confess that when I first started this, it was overwhelming..to say the least. I had to really take a step back and come up with a workflow that would break down the list of requirements for this project. So that’s where I started.

1. Find an API to work with
2. Outline basic functionality (pseudo code)
3. Set up a basic environment/file structure
4. Write code, test code, break code, REPEAT.

**Surprisingly, CONNECTING MY API WAS THE EASY PART.**
The New York Times API is super helpful and user-friendly, with built-in features that allow you to refine your API link. I was able to set up my API pretty easily. 

**INITIAL SETUP**
AVI’s CLI Gem walkthrough was extremely helpful in at least getting me started with the basic setup of my classes. I was able to get my program to run within a matter of 30-ish minutes. 

**NEXT STEP, LOGIC**
Essentially, users where to be greeted with a  list of Nonfiction Bestsellers. They would then be able to pick a number from that list and get more detailed information.

To break this down:
I knew that I needed to have a list view and a detail view. I also wanted to give my users the option of circling back around to the full list again without having to start the program over. 

This is the menu I came up with:
1. Input a number from the bestseller list to view its details.
2. Type 'list' to view the full list again.
3. If you'd like to exit, type 'exit'.

**CHALLENGES**
Getting this menu method to work properly was probably what took the most of my time, for this project. I realized that this method would have to be the main method that prompted the user and also called on my other methods. This method basically gave my program it’s functionality, which at first, took me a second to wrap my head around. At one point I even made an endless loop in my program. This was due to the fact that I was calling my menu twice and needed to do some refactoring in my methods. Because of this issue, I decided to make my call method simple and straightforward. I even made the greeting have its own methods, to keep my code somewhat streamlined and easy-to-read.

**IN THE FUTURE**
In the future, I definitely want to circle back to this project and flesh it out a bit more. 
This API actually gives 4 different buying options for each book in the bestseller list. Adding the functionality to make this part of the menu would be nice. 

I would also try my program out with a more robust API link, such as the main BestSellers lists for all New York Times Bestseller Lists by Genres. That way, users could pick the Genre they want, and then be given a list, with the same options to view more details of a book from that list. 

**TAKEAWAYS**
Overall, I am happy with my project. I know it’s not the fanciest, but it’s functional and I thoroughly enjoyed working on it, even the errors. I can’t believe 2 months ago, I didn’t know the slightest thing about Ruby. I’ve learned so much in the span of a few weeks.


Here’s a link to my repo, if you want to check it out!
https://github.com/allisoncortez/nyt

One final sidenote:
Nerd is a term of endearment!! 
(you're not going to get this unless you run my program)

…..
Bye Nerd ;)

# 
