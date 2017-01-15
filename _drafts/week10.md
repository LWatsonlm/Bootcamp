---
layout: post
title:  "Is Coding Bootcamp Right for You? Week 10 in The Life of a Coding Bootcamper"
date:   2016-11-20
description: "Welcome back to week 10 out of 13. We're almost there, folks. Thanks for sticking with me. As you could imagine, I am exhausted. Maybe you feel exhausted from just READING about the bootcamp? However, we're in the last stretch and there's no time to slow down now. This week is mostly composed of Labs, Voting due to it being Election Week, and a lot of tears and hugs. What doesn't kill you, only makes you stronger, right?! So here we go!"
categories: [coding-bootcamp]
tags: [angular, express, mongoose, vote, web-sockets, node]
fullview: true
comments: true
image: /img/election-day.jpg
---

Welcome back to week 10 out of 13. We're almost there, folks. Thanks for sticking with me. As you could imagine, I am exhausted. Maybe you feel exhausted from just READING about the bootcamp? However, we're in the last stretch and there's no time to slow down now. This week is mostly composed of Labs, Voting due to it being Election Week, and a lot of tears and hugs. What doesn't kill you, only makes you stronger!! So here we go!"

# Day 1: Express && Mongoose: 2.5 Hours

So far we've learned about a number of tools: Node, Express, MongoDB and Mongoose. Developers use these tools to build server-side Javascript applications. We learn how to work each tool individually but we have not used them all together. So that's what today is about. In today's lesson, we will learn how to connect everything and create an app that can receive HTTP requests, retrieve data, make changes to a database and send information back to the end-user.

## Learning Objectives for Express and Mongoose

* Identify how an Express app fits within the MVC framework.
* Connect an Express app to a MongoDB database.
* Implement CRUD functionality in an Express app using Mongoose.

We started with a brand new application, called _When President_ (which happened to be very timely because it was election week). "When President" is a simple one page, CRUD application with hard coded dummy data. It was our job to take this application and implement Express and Mongoose.

Since Rails was fresh in our minds, as a class, we created a Rails-to-Express transition guide. For instance, in Rails, we used PostgresSQL as our database. For Express, we're going to use a MongoDB database.

We also compared Mongoose to ActiveRecord for Rails. Mongoose is an ODM (Object Data Mapping) that we're using to represent data from a Mongo database as models in a Javascript back-end.

Via the command line, we installed Mongoose, created our ```connection.js``` file, defined a schema using mongoose's ```.Schema()``` method, defined a model using ```mongoose.model()``` and lastly connected to our database using ```mongoose.connect()```.

![Mongoose]({{ site.baseurl }}/img/mongoose.png)
<center>Mongoose</center>

In those few steps, we were able to have a real connection to our Express application! Next, we seeded our database using Mongoose.

After a short break, we got back into our application and created forms using ```body-parser```. Body-parser is a parsing middleware that let's us handle form submissions.

I won't go into the rest of the lesson's play by play. But for a Monday morning, we were definitely feeling the burn of knowledge. The heat is on!

## Afternoon Lab: 3 Hours

In the afternoon, we had a lab assigned to us so we could apply what we've learned to a real life project. The lab was called _MEN Lab: URL Shortner_ ... MEN as in Mongoose, Express and Node.

The lab was due at 5pm and an instructor was available for office hours between 6pm-8pm. I stayed behind to really solidify today's lesson and get a head start on the homework due on Thursday.

# Day 2: Election Day!

To everyone's surprise and enthusiasm, our cohort was given the day off so everyone had the chance to vote in the Presidential Election of 2016.

So I took the morning to head out to the polls, sit in a 2.5-hour line, cast my vote and headed back to General Assembly to continue my homework assignments.

# Day 3: Checkpoint && MEAN Lab

It's the day after elections. Okay, I won't lie. Today was the most depressing day ever. Today was the hardest day for me because not only am I'm feeling overwhelmed with work but I'm mentally, physically, emotionally drained from the slap in my face that our Country did last night. That is all I will say about that.

## Checkpoint: 1 Hour

Checkpoints can be thought of a quiz you take to check where you are at in the material. This quiz is a timed assignment involving questions, coding exercising, and short answers. It's open book, open notebook, but you may not speak to other students.

## MEAN Lab: The Rest of The Day

Another lab! Yes, please! As you know, labs are definitely my favorite time in all of the bootcamp. It's time to play around, mess up things, break my application, cry, find that I missed a semicolon somewhere, do a dance, and reflect on all that I've learned.

Today's lab was an open-ended pair lab. It was up to the pair to come up with a project idea. However, it must fulfill the following technical requirements...

## Technical Requirements

Your application should be ME(A)N. This includes...

* Using **Express** to handle HTTP requests and serve API endpoints.
* Using **MongoDB** as the database.
* Using **Mongoose** as the ODM.
* Adding **Angular** as your front-end. Express should only handle your root view as well as your API routes. Angular should take care of the rest via ```ui.router```.
* Your app should have CRUD functionality for at least one model.

Me and my partner, Tim, teamed up and quickly found a project idea. We both share the obsession of POKEMON! So we found an awesome [Pokemon API](http://pokeapi.co/about/) and create our own lightweight, fast, Pokedex... or should I say [RAPIDEX!!!!](https://github.com/LWatsonlm/RAPIDEX). **Hint:** Click on that link to view our Github of the project.

For our project, we did a lot of **pair programming.** Pair programming is an agile software development technique in which two programmers work together on one computer. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The observer also helps with Googling any questions that arise.

Tim was an excellent partner, who geeked out over Pokemon and programming with me. I'd work again with him anytime! #Poke4Lyfe

# Day 4: WebSockets!

HTTP wasn't designed for real-time, two-way communication. Meaning, it wasn't designed for real-time data fetching, such as, let's say you want to see your stocks update in real-time on the screen. What technology would you use? AJAX uses HTTP, where you "pull" information from a server (you make a request and you get something back). So that wouldn't work for real-time data updating... Enter, WebSockets!

![web-sockets]({{ site.baseurl }}/img/websockets.png)
<center>Tweet from yours truly</center>

What is WebSockets? The official definition is:

```WebSockets provides a standardized way for the server to send content to the browser without being solicited by the client and allowing for messages to be passed back and forth while keeping the connection open. In this way, a two-way (bi-directional) ongoing conversation can take place between a browser and the server.```

By utilizing WebSockets, a client can open up a connection to a server that allows for the easy two-way transfer of data. This makes it great for real-time, event-driven web applications.

Twitch and Slack are a couple of the notable web apps out there that are powered by WebSockets.

Mozilla created a very cool game called ![BrowserQuest](http://browserquest.mozilla.org/) using HTML canvas and WebSockets. Then in class, something awesome happened. We were instructed to play the game for the next 10 minutes! It wasn't all fun and games while playing, we were asked to consider the following questions...

* What pieces of information are being relayed between the client and server?
* How often is information sent from the client to server or vice-versa?
* What are some problems the developers who created this game might have had to consider when building it?

![browser]({{ site.baseurl }}/img/browserquest.png)
<center>Browser Quest! Game made in WebSockets</center>

We spent the rest of the day doing an in class lab, using the ![Socket.io chat application](http://socket.io/get-started/chat/) tutorial. Very easy to follow guide for anyone curious about building a quick chat application! 2

## Afternoon Lab: 2.5 Hours

After lunch, we did another lab... I think the 4th lab this week? Today's lab focused on Websockets, of course. We were to team up with a partner and create a simple game for two (or more) players. I teamed up with my partner from Project 3, Liza, and we set out to create a Tic Tac Toe game using Websockets! Fun times!

# Day 5: Slips && All Day Lab

## Slips: 1 Hour
In the morning time, we did our usual stand up in front of the class and answer technical questions regarding the topics learned so far in class.

## Afternoon Lab: 5 Hours

Today is was an all-day structured exercise in developing the skill most likely used in the industry: teaching yourself something new.

We had to pick a useful library or technology stack of something we have not learned in class and build something! We could work alone or with partners.

Tim (remember him?) and I decided to team back up together and keep working on our ![RAPIDEX!!!!](https://github.com/LWatsonlm/RAPIDEX) app! And we decided to spend the day learning ![Vue.js](https://vuejs.org/), The Progressive JavaScript Framework for building user interfaces.

![vue.js]({{ site.baseurl }}/img/vue.js.png)
<center>Vue.js, The Progressive JavaScript Framework<center>

We decided to use our existing Github repo and work off a new branch called ```vuejs```.

If interested, check out our ![Vue.js Github repo!](https://github.com/LWatsonlm/RAPIDEX/tree/vuejs).

## Presentations

Each group had 10 minutes to present what they learned and demo their application.

Some questions that we answered during our presentation:

* Why does this technology exist / what problem does it solve?
* Who built it / who maintains it?
* How does this technology compare to anything we have learned in class so far?
* Where did you go to learn this technology / what are some good resources out there?
* What kind of apps are best suited for this technology?
* What application did you build?
* What do you most like about this technology / what do most not like about it?

Spending the day learning a new language, reading through the documentation and coming to that ah-ha moment, really solidify the fact learning how to code is a lifelong commitment. Technology is always involving and it's important that we learn how to keep learning. Today was an excellent day and the assignment really challenged me.

Alright, that wraps up another week! Thanks for reading! Until next time!
