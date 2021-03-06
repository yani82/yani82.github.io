---
layout: post
title:      "The Beginner's Guide to creating your first Ruby Gem CLI"
date:       2020-09-21 23:36:36 -0400
permalink:  the_beginners_guide_to_creating_your_first_ruby_gem_cli
---

**How I would have spent two week’s worth of time more productively.**

I honestly thought I hit the lowest point in my short coding life this past weekend when it occurred to me that I would never be able to figure out how to request/parse data from a *Yelp* REST API in time to make it before my project deadline. (That and also the fact that I’m typing this on my phone’s Notes📝 because my internet decided it wanted outs for the second time today.) It took me all week of looking at tutorial videos and reading different sites to find that I really could not do it. I wish I had had the decisiveness and logic to not go for an [OAuth](http://http://developer.okta.com/blog/2017/06/21/what-the-heck-is-oauth) for my very first project. Now I know the complications involved. By the way, an `OAuth` “is a delegated authorization framework for REST/APIs. It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password.” So my idea, of having an extension to my [Small Businesses NYC Facebook group](http://http://http://http://.facebook.com/groups/246948743086053?tsid=0.661418698951614&source=result) was dashed. I shall conquer you one day soon though *Yelp* REST API!


**If I could turn back time, I would do a much better job with my initial planning. A good way to start is by browsing this list list of Public APIs on @jbrooksuk’s *GitHub*:**
https://github.com/public-apis/public-apis

Alternate sites for APIs:
* https://apilist.fun/
* https://rapidapi.com/

Make sure you choose an API that does not require an api key 🔑, when you are looking under the *Auth* column, choose APIs with ‘No’ listed by it and is able to produce the data that you'd like to display to your user. 
![](img src="http://IMG_5805.html")

Not forgetting to mention, I had just switched to a local environment the previous weekend, so that was a whole new adjustment. Make sure you make room in your RAM for all the stuff you’re going to be downloading. Don’t spend too much time on adding [fun extensions](http://https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh?hl=en-US) to your *Google Chrome*! Just get cracking. 
![](https://media.giphy.com/media/xtqmnfnCkn1TNTtXzQ/giphy.gif)

Next up, was actually setting up my project on my text editor and linking it to my *GitHub* via *Git*. I had faced many *Git* errors related to this and and faced later on in the project process, below were just a few that I could remember: 

* [➜  ~ git:(master) ✗](http://https://stackoverflow.com/questions/25351213/my-shell-prompt-looks-like-this-gitmaster-how-can-i-get-my-normal-pro) 

* ["Key is invalid"](http://https://stackoverflow.com/questions/10476360/key-is-invalid-message-on-github)

* "Error - zsh: permission denied" = run: pwd > ls > cd bin/ > ls or <./project_name> 

* [require: command not found](http://https://stackoverflow.com/questions/18214409/require-command-not-found) 

* [How to rename a directory?](http://https://stackoverflow.com/questions/6738913/how-to-rename-a-directory) 

* [dquote>](http://https://stackoverflow.com/questions/15773278/dquote-result-of-a-execution-a-program-in-linux-shell) (I used an ! in my commit edit remarks) 

* The most mysterious of them all that effected my `initialize` method and my ability to retrieve data from the website: [Errno::ENOENT: No such file or directory @ rb_sysopen](http://https://stackoverflow.com/questions/43445995/errnoenoent-no-such-file-or-directory-rb-sysopen?noredirect=1&lq=1)


**So, here are some of the basic steps to follow to get you started as well as some common *Git* commands that you’ll be using often: **
![](https://media.giphy.com/media/TgV7fAvYIZMHOed0Rg/giphy.gif)

To OPEN new file in text editor: 
1. cd
2. bundle gem <project_name>
3. ls (to check new project in file directory)
4. cd <project_name> (to retreive new project)
5. [bundler](http://http://railscasts.com/episodes/201-bundler-revised) (*to help you set up all your files for you*) and also https://bundler.io/docs.html 
6. [Install gems](http://https://bundler.io/guides/git.html)


How to push changes to *GitHub* repo:
1. git status (have to be in project's Directory)
2. git add . 
3. git commit -m "added a class for business.rb" 
4. git push origin master / git push 
5. Here's a helpful [video](http://https://www.youtube.com/watch?v=SWYqp7iY_Tc&feature=youtu.be) for beginners

Misc:
* command w = close out of project
* control r = to look up past commands 
* https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet


Also, if you have a bonus lab that isn’t required - don’t do it. That time could’ve been put into your project. Make sure you are absolutely clear of the project requirements and double check with your instructor on what you don’t need to prioritize on stuff like the project diagram. That [Draw.oi](http://https://app.diagrams.net) can steal more of your time than you think.

Don’t try to switch up your routine during project time (if you have a choice that is, which I didn’t since my husband started work and I had my daughter for most of the day who was prepping for her first year of school). Opting to wake up early to code instead of staying up late is great and all (if you actually do wake up!), but there are also no cohort mates awake to bounce ideas off of and ask for help from.
![](https://media.giphy.com/media/ZLxRWG0vhzpiE/giphy.gif)

At the 11th hour, I had switched to scraping local businesses from the *Yellowpages* website, trying to stay in theme with my original idea, but found it much more time consuming than I expected, so I switched AGAIN to using a free API where I was able to instantly parse data from. Unfortunately, with changing of my project, I thought with a few edits here and there I was able to use my old project directory and files, but I couldn’t figure out how to change the main directory’s name so I wasn’t able to run my terminal. I thought by editing it through my hard drive it would solve the issue, but it didn’t. I ended up having to open a new file in hopes that it would work. It mostly did, but the Gemfile, Readme, License etc. (non .rb files) did not attach themselves to the project’s file tree. When I did finally sort that out by cloning the repo from my *GitHub* and start anew from there, and writing most of my code for the project, when it came to my API class, I realized the data that was fetched did not have anything I wanted to list for my user. (Note to those looking for an API with data on Covid-19, do not use https://covid19api.com/) So guess what? I switched YET AGAIN to scraping from *Yellowpages*. It's been such a roller coaster ride! 
![](https://media.giphy.com/media/oZwVVO5EpYImc/giphy.gif)

In the process of overloading myself with all sorts of information, I did come by a few handy add-ons I’d like to use in future projects:

* [HTTParty](http://www.rubyinside.com/httparty-web-api-rest-service-consumption-from-ruby-class-981.html#:~:text=HTTParty%20is%20a%20new%20Ruby,can%20retrieve%20data%20over%20HTTP.)

* [Colorize](http://rubygems.org/gems/colorize/versions/0.8.1)

* [Lolize](http://https://rubygems.org/gems/lolize/versions/0.0.3)

* [Postman](http://https://web.postman.co/build/workspace/e5e43c7f-24c9-4f99-8994-a3a3e72da0c2)

* [ByeBug (Pry equivalent)](http://https://rubygems.org/gems/byebug/versions/9.0.6)  

Ok then, before I continue rambling on nonsensically, I’ll leave you with a quote by *TLC*:
“Don’t go chasing waterfalls, please stick to the rivers and the lakes that you’re used to.”
![](https://media.giphy.com/media/gmxLyCyh6xrR6/giphy.gif)

Please feel free to check out my project, Mom N' Pop, [here](http://https://github.com/yani82/Mom_n_Pop). I'm open to any constructive criticism! 


Nevertheless, with all of the challenges faced, I am truly hoping that I’m able to move forward with my current cohort! A special shout out to my cohort mates Hamza, Wayne, Cinna, Joshua W., Dana, Kelin, Adeeba, Fenty, Shalom and Daniel for all your help and encouragement during this time! I'm definitely going to pay-it-forward <3 



