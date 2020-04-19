---
layout: post
title:      "Building a Content Management System with Rails"
date:       2020-04-19 16:43:31 -0400
permalink:  building_a_content_management_system_with_rails
---


The goal of this project is to build a Rails app that manages related data through complex forms and RESTful routes. In this particular project, we are managing data by utilizing the Rails web framework in conjunction with ActiveRecord and SQLite 3.

P.S. No scaffolding was used to build this project.


## Basic App Flow
*For my ArtMake app, I wanted to make a platform designed to encourage artist collaboration and creativity through artistic challenges. I created my own authentication and authorization methods without gems. I included a third party login for Facebook, to make things easier for users. 
*

My app is pretty straightforward. Users are able to browse through existing challenges, in hopes of finding a prompt or submission that will inspire them to make art of their own.

## Authorizations
Users have the authorization to join/submit to challenges ONLY IF they are registered users. Users can comment on other user submissions. However, they can only delete their own comments or comments directly related to their submissions. If a user wants to see all of their submissions, they would just need to navigate to the “My Submissions” tab in the navbar.


## Hot Tips 🔥🔥🔥
**PLAN OUT YOUR ASSOCIATIONS!**

The toughest part about this project was really taking the time to understand associations and how each model relates to the next. Because I did this in the beginning, it saved me a lot of headaches.

A very helpful source:
https://www.theodinproject.com/courses/ruby-on-rails/lessons/active-record-associations


**User Protection is Key**

Most of the work that went into this project was making sure that users had the proper authentication and validations set up. I would say your most important job is protecting the user throughout your app.

Double check if:
* User Passwords are being stored properly
* Proper checks are being made throughout your app, especially for edit/delete functions.

Important questions:
* Is the user logged in?
* Is the current user equal to the user of what we’re trying to access? (Ex: Is the current user equal to the @user that made this artwork? If they are, they have access to edit functions.)

**Errors Are Your Friends**

I’m going to tell you right now, you WILL run into errors, your app WILL probably break at some point. Don’t freak out. If I’ve learned anything through this project, it’s that errors are definitely our friends.

Take it as a learning opportunity for you to learn something new. Come up with your own process for handling errors. Maybe step one is referring to Google, step 2 is testing in console, maybe step 6 is a sanity walk and more caffeine...the point is: you got this. Don’t give up, push through and learn as much as you can from the errors.

<br>

**End Notes**

I hope this information was helpful and slightly entertaining. Feel free to reach out with insight, comments, and questions.

Happy Coding!





