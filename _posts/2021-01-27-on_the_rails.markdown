---
layout: post
title:      "On the Rails"
date:       2021-01-27 07:54:47 +0000
permalink:  on_the_rails
---

I love how project time always coincides with a momentous occasion!!! Off the high of all the inauguration revelry, I finally was able to focus on my Rails project. I am also 20 weeks pregnant and it’s been a struggle being on top of my coding. After the events of the past week though, I’m feeling hopeful though! 
[](http://https://media.giphy.com/media/l3vReIZxthtDw1kVa/giphy.gif) 

I’m always guilty of taking too much time on planning, and over thinking my associations. Never thought something that the associations would end up being one of the most complicated factors in building an app.
[](http://https://media.giphy.com/media/XeLcgh8gT8o0F5SQ8i/giphy.gif)

It took me a couple days to understand how to make sense my project, [Eco Friend](http://https://github.com/yani82/EcoFriend), which helps users source out eco-friendly alternatives that are through commenting on a brand or creating a new brand recommendation, be it looking for compostable trash bags, to finding a compost bin near them. 
[](http://https://media.giphy.com/media/l1KVcrdl7rJpFnY2s/giphy.gif)

As a refresher, our sub cohort lead, Eri, passed me this video [https://www.youtube.com/watch?v=qfB1MRnzk4g
 ] to skim through and understand what a `join` model actually does. This helped tremendously. As soon as I got my associations set I made sure I started building right away since I have about a week and a day to work on my project as I type this. In hindsight, I should have made it easy for myself and followed one of the examples in the [project requirements](http://https://learn.co/tracks/online-software-engineering-structured/rails/rails-project-mode/rails-portfolio-project), which were either a recipe manager or group task manager since the associations are more direct. 
[](http://https://media.giphy.com/media/xT8qBsOjMOcdeGJIU8/giphy.gif)

I found Cohort Lead, Jennifer Hansen’s videos to be helpful, in particular this one: [Rails MyBlog Project Build - Part 1](http://https://www.youtube.com/watch?v=825w5S69J38&feature=youtu.be&t=138s), was extremely comprehensible and got me to set up almost flawlessly. I just had a minor glitch linking to my Github. 
[](http://https://media.giphy.com/media/cFkiFMDg3iFoI/giphy.gif)

I got this `error: <pathspec 'commit"' did not match any file(s) known to git`, and Eri said that whichever branch I was on would be the one pushed to GitHub, by using `git branch`. If you’re on the main branch, which I’m usually on, you would have to put `git push origin main`. 
SOLUTION:
<git remote origin>
<git remote rm origin>
<remote add origin git@github.com:yani82/EcoFriend.git>
<git remote origin>
<remote add origin git@github.com:yani82/EcoFriend.git>
<git remote origin>
<git push origin master> 

TO TEST AGAIN: <git branch>

After which point, I was feeling good about the flow of building my project up until I used `.build` in my new method, my join model. As I write this I’m still stuck on it and moved to my create method, and commented the `.build` line out, then the form page didn’t show the whole create chunk. Update: I actually managed to resolve this, but unfortunately not being able to grasp my associations entirely kept causing me to switch around my code, making things feel more confusing than they already are. Thankfully, I was able to get the support from my cohort mates and I’m hoping to be able to wrap up my project soon. Currently, I’m still feeling like I’m drowning, so I’ll be sure to update this blog when I’ve completed my project. I wish I had more resources to share, but  below are a few links that might help you along the way: 

Another helpful resource to make sense of your associations, here via [The Odin Project](http://https://theodinproject.com/courses/ruby-on-rails/lessons/active-record-associations). 

When setting up your `Omniauth`, “[Google Authentication Strategy for Rails 5 Application](http://https://medium.com/swlh/google-authentication-strategy-for-rails-5-application-cd37947d2b1b)” by Rachel Hawa, extremely helpful. 

If you’re unsure of your routes, instead of typing `rake routes` in your terminal, it may appear more cleaner if you typed this out in your browser: http://localhost:3000/rails/info/routes. 

The best of luck on your Rail project! 
