---
layout: post
title:  "Is Coding Bootcamp Right for You? Week 13 in The Life of a Coding Bootcamper. Finale"
date:   2016-12-04
categories: [coding-bootcamp]
tags: [angular, express, node, mongoose, project-week]
description: "Hey you! You made it. You made the journey with me to the last final week of class and the big Project 4 finale. It's been a long road and now it's almost time to say goodbye. This week, our instructors provided two elective classes, an Instructor AMA (Ask Me Anything, famous from Reddit) and Project 4 Presentations were due. On the very last day of class, we reflected with our classmates, pop champagne and discussed life after WDI with the Outcomes team. Let's go!"
fullview: true
comments: true
image: /img/bad-class-pic.JPG
---

Hey you! You made it. You made the journey with me to the last final week of class and the big Project 4 finale. It's been a long road and now it's almost time to say goodbye. This week, our instructors provided two elective classes, an Instructor AMA (Ask Me Anything, famous from Reddit) and Project 4 Presentations were due. On the very last day of class, we reflected with our classmates, pop champagne and discussed life after WDI with the Outcomes team. Let's go!

# Day 1: One on Ones and Independent Project Work

Today, we didn't have anything else to do but work, work, work, work, work. An instructor was available to answer any questions from 1:30pm - 2:30pm, exactly one hour of the day. Otherwise, all questions were to be submitted as Github Issues on the general project repo.

# Day 2: Project Work and Intro to React Native

Again, an instructor was available for one hour of the day. All issues or questions were to be submitted through Github as an issue. Luckily, the instructors were very quick to respond to issues and provide help online. Also, as a class, we helped each other a lot through difficult bugs. It's really impressive to see how far everyone has come in their journey of learning to programming. I was truly lucky to have such an amazing cohort, full of bright, helpful and eager individuals.

Okay, enough of the sappy talk.

## Intro to React Native: 2.5 Hours

![React Native]({{ site.baseurl }}/img/react-native.png)

React Native is a framework for building cross-platform apps. React Native is like React, but it uses native components instead of web components as building blocks. This lesson only covered iOS development, that once learned, can be ported into creating an Android app very quickly.

Unfortunately, I did not attend this elective. I didn't think my brain could handle any more new information and I was too focused on my project to even get up and take a bathroom break. But I'll share with you the learning objectives.

## Learning Objectives:

* Explain the problem React Native solves and its approach to solving it
* Build an iOS app with React Native
* Utilize ```Text```, ```View```, ```ListView```, ```Image``` and ```TextInput``` components to construct native screens
* Explain how to style components in a React Native application

# Day 3: Project Work and Custom Deployment

All morning was all work and barely any play. In the afternoon, our official last class was available as an elective: Custom Deployment.

## Custom Deployment: 2.5 Hours

Today, I was feeling good about the progress I've made in my project so I decided to give myself a break and learn about custom deployments! So far in class, we've deployed our apps using Heroku, Github Pages and Firebase. Today, we learned how to deploy our apps using Digital Ocean.

![Digital Ocean Picture]({{ site.baseurl }}/img/IMG_20161130_144513.jpg)

## Learning Objectives:

* Create a Digital Ocean droplet
* Log into a server via SSH
* Install dependencies on a server
* Install a webserver
* Clone an application to a Virtual Private Server (VPS)
* Set up a domain and proxy server
* Configure a reverse proxy

So, if you're like me, you might be asking yourself, "Heroku worked just fine... why learn something new?". With Heroku, deploying to Heroku requires a very specific configuration and customization is very limited.  With Digital Ocean, you have customization, you can install whatever dependencies you want - whether it's gems, npm modules, etc. So, it's worth getting an understanding for when we start building bigger apps, with more dependencies and need the flexibility.

So as a class, we registered for a Digital Ocean account and walked through the learning objectives together.

One notable thing, it was my first time actually using ```nginx```. I've seen that word before but today I found out it's a web server. Most popular for being fast with low memory usage and that it can act as a reverse proxy server. You can easily install it using the command line:

```$ sudo apt-get install nginx```

You'll know nginx is up and running if you see something like this...

![nginx]({{ site.baseurl }}/img/nginx.png)

Cool.

# Day 4: Instructors AMA

So it's the last day before graduation and yes there's still work to be done! However, there was no way I was missing an instructor AMA, aka, ASK ME ANYTHING! Made famous from Reddit, AMA is when famous people or someone with an interesting role or story opens up a forum and you can ask them anything. Literally, anything you want!

This was a lot of fun because we really got to know our instructors more... questions ranged from "How hard is it to code in real life with real humans?" to "What do you think is the meaning of life?"

![Shot of AMA]({{ site.baseurl }}/img/AMA.JPG)
<center>How amazing is this shot? Looks like an album cover. Kudos to my classmate Mike Rubin for the pic!</center>

# Day 5: Presentations, Graduation and Reflections

It's the BIG day, folks! Time to talk about the project.

## Project Overview

We’ve come a long way, and it's time to show it. This will be the most advanced project to date, and if you put creativity into it, it'll hopefully be the thing you want to show off most prominently in your portfolio.

We get to call the shots and invent our own idea, choosing a framework & tools that are appropriate for what we want to build. Pull from everything we've learned so far, and tackle something that'll push us a little outside of our comfort zone.

Make sure to review the project proposal with an instructor so we can make sure it's something that can be accomplish in the limited time we have, and make sure it's something that'll be impressive visually. Sometimes people do judge a book by its cover – or an app by its design.

## Technical Suggestions

### Your app must:

- Be a complete product, which most likely means multiple relationships and CRUD functionality for at least a couple models
- Implement thoughtful user stories that are significant enough to help you know which features to build and which to scrap
- Be deployed online so it's publicly accessible

## What Did I Do?

## Background Story

Going out on a budget is hard. After spending 14 weeks unemployed while attending General Assembly, going out is almost impossible without busting your budget for the week.

Every night, my friends and I researched bars with the best drink specials. The number one question in mind... where are all of the drink specials? And **$ip** was born.

**$ip** will only show you bottomless drink specials that are under $15. In most cases, the drink special is FREE!

![$ip Screenshot]({{ site.baseurl }}/img/$ip.png)
<center>Screenshot of main page for $ip</center>

<br />

![$ip Collage]({{ site.baseurl }}/img/collage-sip.jpg)
<center>Collage of screenshots</center>

## Technologies Used

$ip is a full CRUD, MEAN Application with a Google Maps API. It's built with:

- AngualarJS
- MongoDB
- Mongoose
- Express
- Nodejs
- Google Maps API for Plotting Data on the Map

I created my own API that you can [view/use here](https://sip-dc.herokuapp.com/api/drinks)

## Live Demo

So you can check out my app, $ip, right now by visiting it's [live demo link](https://sip-dc.herokuapp.com/)

If interested, you can check out [my Github](https://github.com/LWatsonlm/Sip)

Here's how to run the app from Github:

```$ npm install```

```$ mongod```

```$ nodemon index.js```

## Upcoming Features

1. Remove the show view and corresponding show router and use modals instead, making it a true SPA.
2. When you click on a marker on the map, details appear regarding the location.
3. Adding Google Places API, so users can search inside the Google Map for locations.

## Presentations

We had presentations in the same style of project one... science fair style. Remember that? It's when everyone stands up at their individual spots in the room and show off your project to anyone who walks to you. Definitely much more preferred than standing up in front of the room and presenting.

One of the best feelings in the world is watching people light up when their interacting with something you built. I loved being able to be proud of my work and show off it's beauty. It helps that it's an app focusing on drinking deals because who doesn't love a good deal on alcohol?!

![classmates viewing my app]({{ site.baseurl }}/img/classmates.jpg)
<br />
![classmates viewing my app2]({{ site.baseurl }}/img/classmates2.jpg)
<center>Classmates interacting with $ip! Love it!</center>

# Day 5: Graduation and Reflections

After everyone had a chance to present their project, it was time to reflect on everything we've learned and how much we've grown.

We were told to grab a piece of paper and a piece of tape and turn to the left and tape that paper on our neighbor's back. Remember those days in grade school where you would wear a white shirt and let people write notes with markers on it? Or how our year books had blank pages towards the end so your friends could write messages saying "stay true"... "never change!" ... this was that type of party.

Since I actually like these people, today wasn't as painful as middle school.

![reflecting]({{ site.baseurl }}/img/reflections.jpg)
<br />
![reflecting]({{ site.baseurl }}/img/refelections2.jpg)
<br />
![reflecting]({{ site.baseurl }}/img/reflections3.jpg)
<center>You write on my back, I'll write on yours!</center>

<br />

Here's what I got back from ... my back:
![What my classmates think about me]({{ site.baseurl }}/img/my-back.jpg)

After this, we popped champagne (no really! We had 6 bottles of champagne!) and cheers to our victory. Then we took a super awkward group picture haha.

![Group Picture]({{ site.baseurl }}/img/bad-class-pic.JPG)
<center>lol</center>

<br />

And that was that. Another chapter closed in my life.

Next post I'll chat about what's been up since ending this journey into coding. Spoiler alert: It has been a lot of networking, public speaking, and just getting my face out there!

Until next time, friends.
