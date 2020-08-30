---
layout: post
title:      "Rails API with React/Redux frontend"
date:       2020-08-16 23:59:00 -0400
permalink:  rails_api_with_react_redux_frontend
---


For my final Flatiron project, I decided to build an app that would render a list of events (art and music only) happening locally. From personal experience, I feel like any time I am looking up events or want to see what’s going on in a day, I have to spend a lot of time browsing, or checking different sources. This can be somewhat tedious at times. The way I envision this, the main list would only be responsible for displaying events happening on the exact day the user is opening up the app, reducing scroll time, and allowing for users to really just get a brief overview of what’s happening locally that day.

Working through the Redux flow was definitely a learning experience for me, but something I feel that I have a solid knowledge of, after having gone through some hiccups of my own.

Here are some things to consider, if you're working on your own project:
* props are variables that are passed down from a parent component to a child component. Use props when the data being passed down is for rendering purposes only (you're not manipulating this data, it's for read-only purposes). 

* State variables are initialized AND updated directly by the component; Used typically when you want to store data that needs to be easily updated/changed throughout the component's lifecyle(ex: event time and date, user's location)

* Redux gives us access to global state, basically it's easy access to data without having to pass things down from the parent, which can get a little messy.

*How do you access the data you're putting in the Redux global state?? Answer: mapStateToProps()


One of the biggest issues I ran into was updating my comments correctly. What this really boiled down to was how I was manipulating data in my reducer. Since the state is held within your Redux store, the DOM only updates based on whether your store state has been updated correctly. 


### Stretch Goals
I started off with a basic MVP app, but quickly realized just how much I could build this out in the future.
I'd like to implement a User model in my backend. I imagine user's being able to 'favorite' certain events they are interested in. If they're not logged in, they'd be prompted to do so via Google oath.

I would also want to incorporate the Google Calendar API, giving users the ability to add events 
to their calendar, which is always super convenient.


