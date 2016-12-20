# Tech Eats: Stories of Tech and Food
## Built with Jekyll and hosted on Github Pages
<hr>

# About Tech Eats:

Tech Eats is my blog recapping stories of food, travel, and tech. Featuring my series documenting my journey through a full-time coding bootcamp in Washington, D.C, entitled: "Is Coding Bootcamp Right for You? A Week in The Life of a Coding Bootcamper"

# "Is Coding Bootcamp Right for You? A Week in The Life of a Coding Bootcamper"

In September, I embarked on a new journey to become a web developer through a full-time coding bootcamp. It took me a long time to decide if a coding bootcamp was right for me. I had a hard time finding resources from first-hand experiences from students, and there’s definitely not a lot of week-to-week recaps of what exactly goes on at these camps.

So, I started a weekly recap of my experiences with General Assembly for anyone and everyone who is thinking of joining a coding bootcamp. I hope it helps someone out there.

# Important Things I Learned While Building a Site Using Jekyll

## Front Matter, Matters.

Every single post needs to have a Front Matter or else it just won't work. Front Matters come with all types of options, and example of my Front Matter for my posts:

```md
---
layout: post
title:  "Is Coding Bootcamp Right for You? Week 8 in The Life of a Coding Bootcamper"
date:   2016-11-06
description: "Last week was Project 2 week... this week, we talk APIs, AJAX, Building our own API, Firebase and the introduction to Project 3. Let's go!"
categories: [coding-bootcamp]
tags: [API, AJAX, angular]
---
```

Important to note: How the markdown files get served also varies depending on the ```_config.yml``` file.

## _site folder

Do NOT modify or add anything to the ```_site``` folder! This is the rendering folder for Jekyll and any modification will be eliminated without warning. I spent my entire first day using Jekyll wondering why none of my styles were rendering! 😅

## Localhost vs. Live on Github Pages

This has been my biggest lesson for sure. GitHub Pages is deeply integrated with Jekyll, but for some reason, Jekyll's relative paths don’t work on GitHub Pages.

 Meaning, once you deploy, **all** the image links and styling will not work. You need to update all the relative paths and images paths for everything to render properly on GH-Pages.

The problem is that Jekyll assumes that your site lives at the root URL ```(i.e. username.github.io)```, when it is in fact in ```username.github.io/project-name```.

The solution is well documented by [Matt Swensen](https://github.com/jekyll/jekyll/issues/332#issuecomment-18952908):

<quote>
In ```_config.yml```, set the baseurl option to ```/project-name``` -- note the leading slash and the absence of a trailing slash.

Now you'll need to change the way you do links in your templates and posts, in the following two ways:

When referencing JS or CSS files, do it like this:
```{{ site.baseurl }}/path/to/css.css```
-- note the slash immediately following the variable (just before "path").

When doing permalinks or internal links, do it like this:
```{{ site.baseurl }}{{ post.url }}```
-- note that there is no slash between the two variables.

Finally, if you'd like to preview your site before committing/deploying using ```jekyll serve```, be sure to pass an empty string to the ```--baseurl``` option, so that you can view everything at ```localhost:4000``` normally (without /project-name getting in there to muck everything up):
```jekyll serve --baseurl ''```

This way you can preview your site locally from the site root on localhost, but when GitHub generates your pages from the gh-pages branch all the URLs will start with /project-name and resolve properly.
</quote>

I'd like to note that I found my pictures inside my posts were coming back with 404, so I needed to update my post's links to use Liquid markup language:

```md
![welcome]({{ site.baseurl }}/img/IMG_20160906_131357.jpg)
```

 ## Contact Information
 You can always find me on [Twitter](https://twitter.com/lmwatsonn), [LinkedIn](https://www.linkedin.com/in/watsonlm) or shoot me an email at latoyamwatson@gmail.com

 Enjoy reading!
