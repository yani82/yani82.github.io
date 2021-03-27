---
layout: post
title:      "Wild Wild West of JavaScript"
date:       2021-03-27 02:36:45 -0400
permalink:  wild_wild_west_of_javascript
---


![](https://media.giphy.com/media/4TcR3qT0oEbyVkyDEV/giphy.gif)

Amazingly I had an easier time comprehending JavaScript compared to Ruby. I think it was heavily due to the fact that I had done some previous prep work on it, and I was also trying to balance another course when I was trying to learn Ruby. Even with with some internal adjustments within our cohort, as well as trying to get the hang of Canvas, surprisingly I was able to grasp the concepts easier. You will be able to see some similarities in Ruby too, which may be another factor as to why everything came together more fluidly. 

![](https://media.giphy.com/media/3o7aD3fWu2sAz9dAM8/giphy.gif)

Similarities in Ruby && JavaScript languages:
- They are both object oriented 
- Dynamic 
- General purpose
- Scripting 

As for my project, I decided on a blog concept app that allows users to share with one another their volunteering experiences, to inspire more people to volunteer to a good cause. It’s a very simple two model app. 

![](https://media.giphy.com/media/pHXhn8Ee6lRO0KZtM1/giphy.gif)

Some of the very useful resources I referred to when building my JavaScript project were [Ayana Zaire’s 7-parter project build](https://www.youtube.com/watch?v=Q5R7HSqdGFk&t=8s) and you also refer to her GitHub repos, and notes [here](https://github.com/learn-co-curriculum/mod3-project-week-setup-example) and [here](https://github.com/AyanaZaire/javascript-project-resources/blob/master/js-project-ooo.md). 


The first obstacle I came across was, I had failed to do something as simple as creating a new directory for my front end from my back end VSCode terminal. It didn’t  show in my file tree. These are the steps I took to rectify it: 
- Open computer terminal 
- Type `code .`
- All files will open in text editor
- Go into front end directory
- Type `code .` again 
- VSCode will open only that directory 

![](https://media.giphy.com/media/Y0PMqgFAccyahnWN3V/giphy.gif)

I learned a couple of best practices along the way. Firstly, the reason why there was a need to make two separate directories for our backend and front end is that if you want to deploy your backend to a host like *Heroku*, or your front end to a host like *Netifly*, it would be easier. Also, in a real world scenario it’s easier for the back end and front end developer to focus on what needs to be done in their respective departments. 

![](https://media.giphy.com/media/MqxZxTlvcY5BS/giphy.gif)

Secondly, albeit annoying to get used to, but I totally understand why it’s best practice - is making each file separately in their own branch. This enables you to ensure that it’s working correctly before pushing it to your main/master branch. If anything were to break in your app, it’d be easier to locate and fix, instead of having your whole app break and having to start all over again. 

#### Git commands and how to merge in GitHub:
- Git co -b user_model 
- Rails g model User name image_url email 
- Git add . > git commit -m “user model” > git push 
- If merging on Github: Compare & Pull request > Create pull request > Merge pull request is green > Confirm merge > Delete branch 
- Back in terminal: Git co master
- Git pull 

Oddly enough, after watching Ayana’s Refactoring OOJS [video](https://youtu.be/EleImMG_8Ck), everything just started falling apart as an app usually does when you’re building it. So a few other issues I had faced were: 

- Not able to display create function on browser without refreshing it and it’s parsing data according to Console
- Not able to reset form to empty after posting data
- App totally did not respond to anything I was trying to communicate to server?! (truly the moments when you doubt ALL of your abilities in trying to pursue software engineering!) 

![](https://media.giphy.com/media/26Ff2l7ENOhVCJpLy/giphy.gif)

This is when I knew I had to reset my brain, and start fresh the next day. 

![](https://media.giphy.com/media/A7XIKk7dBwSZQ7oFku/giphy.gif)

#### Extra Resources: *Ayana's Part 2-7 JS Project Build*

- [PART 2](https://youtu.be/ZJdfWBVFWAI) — Routes, Controllers, Serializers


- [PART 3](https://youtu.be/goYf_xQiGyE) — Events, Fetch, and DOM Manipulation using a Rails API


- [PART 4](https://youtu.be/EleImMG_8Ck) — OOJS Refactor


- [PART 5](https://youtu.be/u_Zrd8LvS7A) — Complex Database Relationships


- [PART 6](https://youtu.be/18L_LRxMeIw) — Intro to Implementing Bootstrap


- [PART 7](https://youtu.be/YIGbMX49vcE) — Implementing Auth in JS Project using JWT


