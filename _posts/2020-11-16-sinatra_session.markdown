---
layout: post
title:      "Sinatra Sessions"
date:       2020-11-16 01:47:55 -0500
permalink:  sinatra_session
---


I don’t know what it is about project time, but so much always happens simultaneously during this already STRESSful time. It fell during the week of a historic election, for one! 

![](https://media.giphy.com/media/d1JfgvIoEsy4dtZK/giphy.gif)

I was still in the midst of completing the Fwitter Lab, and put it on the back burner because I was so distracted with election updates. As most of you may know, it took about four days for our NEW President to be officially announced, and between that time, my MacBook decided it didn’t want to turn on. What excellent timing! In addition to that, the lack of sleep and stress led me to catch a cold. I also had a very important check-up scheduled. I wasn’t exactly on my A game, which gave me flashbacks of my experience during project 1 (Ruby CLI). De javu, all over again. I had to use my Windows laptop that didn’t have a local environment set up, and regressed to using a buggy IDE to complete my Fwitter Lab. Good times. 

![](https://media.giphy.com/media/QwrTpd2uFPeaA/giphy.gif)

Thankfully, I was able to fix my laptop within a day (I am $150 poorer), and I was able to complete my Fwitter Lab on the afternoon of that momentous Saturday itself. That night I was able to set up my project, with surprisingly minimal issues! I had created a new repo in my Github, and cloned that to install the [Corneal](http://thebrianemory.github.io/corneal/) gem. I ended up having to delete my `LICENSE` file and moving the `README.md` under my main app folder, because it was created with them outside of my main app folder *shrug*. Corneal is amazing - thank you to former student of Flatiron School: Brian Emory, for creating it! 

![](https://media.giphy.com/media/LtcuAIzPqlTnW/giphy.gif)

Guess what I decided my project would be on? Voter registration! My sources of guidance for initially setting up my Sinatra project was this very helpful [blog post](https://flatironschool.com/blog/how-to-build-a-sinatra-web-app-in-10-steps) by @aprietof that was shared by my fellow cohort Christie. I also watched Avi’s "[Building Authentication in Sinatra](https://www.youtube.com/watch?v=_S1s6R-_wYc&t=484s)" video a few times. Here are more helpful [tutorials](https://www.youtube.com/playlist?list=PLNUiyK37z4zHyIuQjCJt-gPjBzbMb5k1Q) that may come in handy. 

![](https://media.giphy.com/media/THHHNksRyvBK1zGHjO/giphy.gif)

For useful resources on authentication and `Bcrypt`, check [this](https://github.com/codahale/bcrypt-ruby) out.

These sites helped with creating my Views. There really is no limit to what you can do and add to your form if you had the time. 

* [PHP Form](http://www.phpform.org/download_html?id=og8d38bv2b54kfq80fg0e11466)
* [HTML Goodies](http://www.phpform.org/download_html?id=og8d38bv2b54kfq80fg0e11466)
* [MDN Webdocs Mozilla: form](http://www.phpform.org/download_html?id=og8d38bv2b54kfq80fg0e11466)
* [MDN Webdocs Mozilla: button](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)
* [Nu HTML Checker](https://validator.w3.org/nu/#textarea)
* [erb Extension for VSCode](https://marketplace.visualstudio.com/items?itemName=CraigMaslowski.erb)

I faced this very unique error` Errno::EIO at /registries Input/output error @ io_writev - <STDERR>` that I couldn't figure out for the life of me. It took me almost a couple of days, and thankfully my cohort mate, Chaim, managed to help me resolve it! We had to kill a server listening on another port. [Here](https://github.com/sshingler/capistrano-resque/issues/81) are a [couple](https://stevenwilliamalexander.wordpress.com/2013/02/04/ruby-sinatra-unicorn-errnoeio-inputoutput-err/) links that may help you resolve it, just in case you face the same issue. 

Resolve: 
Key in `lsof -i tcp:9393` (port number) in your terminal 
Then `kill -9 67619` (5-digit number that is shown in terminal) 

I wanted to thank all my cohort mates who took their time to help me out on this project! Check out my repo here: [VOTEworks](https://github.com/yani82/VOTEworks). Till next time, "swing easy"! 

![](https://media.giphy.com/media/28mkBBJuyIEPVRbypT/giphy.gif)





 




