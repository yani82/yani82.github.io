---
layout: post
title:      "A Second Chance at JavaScript "
date:       2021-07-09 16:40:07 -0400
permalink:  a_second_chance_at_javascript
---


### Just when I thought I had a grasp of JavaScript because I saw minor similarities in Ruby - I had no idea!

![](https://media.giphy.com/media/ttylf4OADMn7YIOnbF/giphy.gif)

Due to a lot of obstacles in my then cohort, and going through a few complications during my third trimester, my first shot at JavaScript was a bust. Redoing JavaScript proved to be a blessing in disguise though. I had a more supportive instructor, and I had more time to really understand (or a least much more than I did) the inner workings of JavaScript. And so, I rebuilt my project from scratch as much as I could. 

## TravelBug 

![](https://media.giphy.com/media/vBMzK6KN6M6zK/giphy.gif)

This time I decided on creating an app that provides avid travelers a source of what the most updated travel restrictions (in app: travelbugs) are depending on which destination they select. All my data is seeded at the moment. Initially I wanted to keep it to two models - travelbugs and users, but was advised to add countries and comments as well, which took me a while to wrap my mind around the newfound associations, so I decided to take a step back and focus on the initial two models and work from there. It isn't as complicated as I had thought it would be, it's just a matter of compartmentalizing the different functionalities of your app into different models, and eventually classes in my front end. 

## Fetch to Render 
I have a slightly better understanding of the cycle from 'fetch' to 'render' to the DOM. Basically, in layman's terms you're fetching or parsing or abstracting data or information from an API, which is via an endpoint that is either created by you in a seed file in your database or from an external API in the form of a URL. With each fetch request, a 'promise' is returned. This is executed 'asynchronously', which handles multiples tasks at the same time. So for example, if there you setup a `console.log` inside a 'fetch' request and one outside of it, the one outside would execute first since it doesn't have to wait for the `console.log` in the fetch request to run. Below is one of the best images that displays [this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise):

![](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/promises.png)

I feel like learning JavaScript is a neverending journey, and I have so much more to learn! 




