---
layout: post
title:  "Assignment 3"
date:   2015-09-30
categories: CS3216 assignment3
---

Assignment 3 turned out to be a disaster. A number of features, such as notifications, which I think are needed for the product to make sense remain unimplemented, and as a whole the application is quite buggy.


What went wrong? A confluence of being under-manned and over ambitious for the amount of time and manpower that we had.


The motivation for the app was simple - build something that can help you find people to share a cab with you as well as get the best route given the start and end points of the people sharing the cab. This was in part inspired by one of our bad experience with the driver being unsure of the route while sharing a cab with friends. We started out being very unfocused, trying to be usable in the case of car pooling and taxi sharing. On hindsight, we could have fine tuned our UI by just focusing on taxi sharing.


Our project was behind schedule throughout the 3 weeks allocated to us. Progress in the first week was very slow as most of the team was learning the frameworks we decided on - Ionic/Angular + Laravel. On my part, I fell sick that week and was unable to do much besides pushing up some boilerplate so that the rest could get started.


Throughout the project, there was this nagging worry that I wouldn't be able to get the features needed on the backend. The person allocated to the backend was semi-responsive for the most part (I realised that the best, but not exactly fastest way to reach him was via SMS. DUDE we agreed to use Slack and you are not monitoring it.) and there was absolutely nothing on the backend until Friday of the second week. 

I was tied up on the frontend fixing weird bugs resulting from how Angular/Google was attaching things to the DOM and how we needed the components to be attached. I left styling to Justin because he was much better than me in this aspect. 

Well, our dear unresponsive-and-always-late-for-meetings friend eventually did push something up in the last week, but I was never sure what he had done or what was lacking until I started trying the integrate the backend. It was an absolute pain because there was absolutely no documentation for the backend API and absolutely no useful comments in the code. My original intention was to do the integration with him present at our daily meetings so I could get immediate answers to what each endpoint was for but he never showed up >.< Integration was a very messy business as the backend was buggy and there wasn't proper tests I could run to find out what was wrong. With the backend guy being not physically present and slow to respond, I had to result to fixing many of the issues myself. 

Our application does not work offline in part because of our heavy reliance on google maps. This was partly my fault as I wasn't tracking the milestones properly and never considered offline functionality in the initial design. I also made the mistake of choosing the wrong offline storage, IndexedDB, which was not well supported by Safari, so it doesn't work on iOS. But there wasn't time to fix it.


I'm sorry this turned out to be a really ranty post as assignment 3 was a really huge pain and colossal failure to me. From this experience, I learnt

1) **The importance of being focused**

Do not try to do too many things at once. Start by targeting a smaller use case and doing it well, rather than being general and trying to be useful for a bigger group of people. 
Also, we should have been more realistic about what was achievable given our time and manpower constrains. We should have flashed out a clearer timeline of what we had to get done.

2) **The importance of a good team**

I learnt that it was really beyond my ability to fill in the gap for the backend and work on the frontend at the same time. 
Given my lack of UI design and implementation talents, I should really team with someone who has more experience in frontend work. The good thing that arose from this random grouping is I had someone who could take care of the styling as well as do up the much needed help page.

---------------------------

With the conclusion of assignment 3, I finally get a much needed break from CS3216 work. I should really catch up on my backlog from other modules as well as my FYP (oh noes I have done absolutely nothing for it over the past 4 weeks) before I have to start working on my final project. I'll do a post about my thoughts and expectations for the final project if I have time.