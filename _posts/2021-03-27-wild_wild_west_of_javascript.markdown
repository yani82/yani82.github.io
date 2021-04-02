---
layout: post
title:      "Wild Wild West of JavaScript"
date:       2021-03-27 02:36:45 -0400
permalink:  wild_wild_west_of_javascript
---


![](https://media.giphy.com/media/4TcR3qT0oEbyVkyDEV/giphy.gif)

Amazingly I had an easier time comprehending JavaScript compared to Ruby. I think it was heavily due to the fact that I had done some previous prep work on it, and I was also trying to balance another course when I was trying to learn Ruby. Even with some internal adjustments within our cohort, as well as trying to get the hang of Canvas, surprisingly I was able to grasp the concepts slightly easier. There are some similarities in Ruby too, which may be another factor as to why everything came together more fluidly. 

![](https://media.giphy.com/media/3o7aD3fWu2sAz9dAM8/giphy.gif)

Similarities in Ruby && JavaScript languages:
- They are both object oriented 
- Dynamic 
- General purpose
- Scripting 

As for my project, *Love Wins*, I decided on a blog concept app that allows users to share with one another their volunteering experiences, to inspire more people to volunteer to a good cause. I was inspired witnessing how everybody came together during the toughest of times last year to help each other out. This moved me to volunteer in many different community based causes, and motivated me to spearhead a few food drives for first responders. *Love Wins* is a very simple two model app. 

![](https://media.giphy.com/media/pHXhn8Ee6lRO0KZtM1/giphy.gif)

Some of the very useful resources I referred to when building my JavaScript project were [Ayana Zaire’s 7-parter project build](https://www.youtube.com/watch?v=Q5R7HSqdGFk&t=8s), you can also refer to her *GitHub* repos, and notes [here](https://github.com/learn-co-curriculum/mod3-project-week-setup-example) and [here](https://github.com/AyanaZaire/javascript-project-resources/blob/master/js-project-ooo.md). 


The first obstacle I came across was, I had failed to do something as simple as creating a new directory for my [frontend](https://github.com/yani82/love_wins_fe) from my [backend](https://github.com/yani82/love_wins_be) text editor terminal. It didn’t  show in my file tree. These are the steps I took to rectify it: 
- Open computer terminal 
- Type `code .`
- All files will open in text editor
- Go into frontend/intended directory
- Type `code .` again 
- Your text editor will open only that directory 

![](https://media.giphy.com/media/Y0PMqgFAccyahnWN3V/giphy.gif)

I learned a couple of best practices along the way. Firstly, the reason why there was a need to make two separate directories for our backend and frontend is that if you want to deploy your backend to a host like *Heroku*, or your frontend to a host like *Netifly*, it would be easier. Also, in a real world scenario it’s easier for the backend and frontend developer to focus on what needs to be done in their respective departments. 

![](https://media.giphy.com/media/MqxZxTlvcY5BS/giphy.gif)

Secondly, albeit annoying to get used to, but I totally understand why it’s best practice - is making each file separately in their own branch. This enables you to ensure that it’s working correctly before pushing it to your main/master branch. If anything were to break in your app, it’d be easier to locate and fix, instead of having your whole app break, and having to start all over again. 

#### *Git* commands and how to merge in *GitHub*:
- `git co -b user_model `
- `rails g model User name image_url email `
- `git add .` > `git commit -m “user model”` > `git push` 
- If merging on *GitHub*: Compare & Pull request > Create pull request > Merge pull request is green > Confirm merge > Delete branch 
- Back in terminal: `git co master`
- `git pull` 

Oddly enough, after watching Ayana’s Refactoring OOJS [video](https://youtu.be/EleImMG_8Ck), everything just started falling apart as an app usually does. A few other issues I had faced were: 

- Not able to display my `create` function on the browser without refreshing it, but it’s parsing data according to the `Console` (resolution: I had to double check on whether I was passing the right arguement in the last line of my fetch) 
- Not able to reset form to empty after posting data (resolution: added `titleInput = ""` on the last line of my `createFormHandler`)
- App totally did not respond to anything I was trying to communicate to server?! (truly these are the moments when you doubt ALL of your abilities in trying to pursue software engineering! Resolution: I didn't complete my *Git* merge onto *GitHub*) 
- I wasn't able to `git pull` new code from a separate branch onto my local text editor after attempting to use `git stash` which saves my code locally in a different file, saves it for later, making it retrievable, and avoids switch branch errors, then I `git pull`'ed and that didn’t work, so I used `git fetch`, and then `git pull`’ed again and that didn’t work, so with the help of my cohort mate Jordan, we looked up `git reflog` to see the log history, and I thought since my new branch had successfully merged on the main/master branch on *GitHub*, I could just clone that repo. So, I took out my existing frontend folder in my computer first, then cloned it - so that worked!!!

![](https://media.giphy.com/media/X9dpsHE4VPMWY/giphy.gif)

Along my arduous journey of debugging, at least I was able to learn many new *Git* commands I would have never known, as well as learned how useful it is to download the *GitHub* desktop app to make stuff like that easier, and I didn’t know that I had to `npm install` before starting anything, which is equivalent to `bundle install`. It checks on your app's dependencies, and is also used when doing *React* labs.  I also downloaded a new extension for my *VSCode* text editor called `Live Server`, which is awesome! You don’t have to reload your server all the time, it does it for you. Unfortunately, I wasn’t able to debug my `addEventListener` for a new `delete` fetch I was trying to create, it didn’t even hit my `console.log` and returned as `null`. Currently, this is also causing my `create` function to break! So, I'm pretty dumbfounded at the moment, and just trudging through to finally get everything running. 

**Update**: I was able to get past my last bug, by combing through my `index.html` after using *Bootstrap*, and got my `delete` function working, BUT I have to click on the `Create Post` button first, and then click on the `Delete` button under a post for it to actually `delete` a post. Currently, I'm still trying to figure out what is causing this. If anyone has ever experienced this before, do let me know how you managed to debug it. '

![](https://media.giphy.com/media/26Ff2l7ENOhVCJpLy/giphy.gif)

#### Extra Resources: *Ayana's Part 2-7 JS Project Build*

- [PART 2](https://youtu.be/ZJdfWBVFWAI) — Routes, Controllers, Serializers


- [PART 3](https://youtu.be/goYf_xQiGyE) — Events, Fetch, and DOM Manipulation using a Rails API


- [PART 4](https://youtu.be/EleImMG_8Ck) — OOJS Refactor


- [PART 5](https://youtu.be/u_Zrd8LvS7A) — Complex Database Relationships


- [PART 6](https://youtu.be/18L_LRxMeIw) — Intro to Implementing Bootstrap


- [PART 7](https://youtu.be/YIGbMX49vcE) — Implementing Auth in JS Project using JWT



May the odds be ever in your favor! 

![](https://media.giphy.com/media/edLKLYMlNFPJC/giphy.gif)


