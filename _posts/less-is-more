---
layout: post
title:  "Less is More?"
date:   2015-10-12
categories: CS3216 Final Project
---

Met Gerald and Garry on Thursday. Turns out his use case for the application is much simpler than we thought. I was under the impression that he wants to be able to track all reviews for the online store as well. But it turns out that he's more concerned with being able to quickly pick out reviews to be displayed. So we are moving back to the show/do not show review paradigm instead of the good-review/bad-review/not-a-review paradigm, which is essentially how Repuso does things... So we are really building something like Repuso, just with better/nicer UI and maybe a search feature?

I like the idea of being able to sort and manage reviews but it makes the application more complicated and perhaps less intuitive for new users. Perhaps it's better that our core features are actually very simple so we can focus on getting it well polished within the short frame of time we have. 


Development is progressing slower than expected. Because of how tightly coupled Meteorjs is to MongoDB, we had to go back on the decision to change to PostgresSQL. It actually possible to switch to Postgres, just that we would have to wrap all method calls in Fibers ourselves and we would have to modify some of Meteor's libraries. Too much hassle given the short amount of time we have, what's more Meteor is currently working to integrating Postgres, so we would be duplicating work on their side.

Realistically speaking, MongoDB might not bottleneck on us so soon, given most of our queries are readonly and most of the time we are just pulling data from a single collection. But I really dislike how MongoDB is designed. No joins? Come on, you can't run away from having relational data of some sort. So you can't run away from having to pull data from 2 collections, unless you are doing something really horrible called nesting documents. 

Not sure I like Meteor though. On one hand it handles the build process for you, so I do not have to write scripts to copy files, combine and minify them. It also provides an abstraction over Node so you don't get callback hell, unless you have to write a lot of async code. But it is a little too opionated.
It's really easy to get started but if you really want to write maintainable code you need to figure out how Meteor really does things, which is where our bottleneck is. Life gets dicy when you want to do things differently from how the developers of Meteor think things should be done...