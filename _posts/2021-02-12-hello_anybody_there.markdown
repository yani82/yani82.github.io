---
layout: post
title:      "“Hello, anybody there?”"
date:       2021-02-12 01:17:17 -0500
permalink:  hello_anybody_there
---

## Part II of my Ruby on Rails Project: Taking a deeper look inside a request-response cycle.
![](https://media.giphy.com/media/l4EoT3nunImqfLTa0/giphy.gif)


Of course, in my head I called this cycle anything but “request-response”. Instead, I would refer to it as Get/Post, a stateless request or just you know, that thing that happens when you click on submit and it returns something on the browser? Clearly, I didn’t quite grasp the “request-response” cycle fully.
![](https://media.giphy.com/media/3ohhwpmXjcIot5lv68/giphy.gif)

After doing some research, I found it was extremely helpful to write this down so I’m able to articulately explain and describe what this is when asked. Especially during an assessment! What’s actually happening when you load that URL? Your browser sends a “request” for the post resource, and the web framework, Rails, has to then send back a “response” with some HTML for the browser to display.
![](https://media.giphy.com/media/dwmNhd5H7YAz6/giphy.gif)


### Just to break it down, Rails figures out which code should handle the “request”.
![](https://media.giphy.com/media/xT8qBv7JyQi32dIlEc/giphy.gif)

### The “request” then gets routed to an action method on a controller.
![](https://media.giphy.com/media/j1saJ4yHuKh015eJB2/giphy.gif)

### Then the controller will load the resource in from the database, using a model class.
![](https://media.giphy.com/media/PPThcor17aVvtW7bO1/giphy.gif)

### The controller will then render a view usually through a HTML page.
![](https://media.giphy.com/media/jHRAf2A6WuduX2raSe/giphy.gif)

### The result of rendering the HTML is then returned to the browser as a “response”.
![](https://media.giphy.com/media/lcs5BL0NIM4WMv61a9/giphy.gif)


In the case of my project, [Eco Friend](https://github.com/yani82/EcoFriend), this fires after the user logs in and is prompted to 'Recommend a Brand', and if the requested data is not received, the app will redirect the user back to the `brand_path`, which is the page the user is currently on until the app receives the requested data to proceed forward. Otherwise, if the data requested is properly filled out, which is the 'Name', 'Category', 'Info' and 'Image' (optional) is provided by the user, the app will then receive the separate request, goes through the router, gets pointed to a new controller action that will then `render` to the next page that will `show` what the user had just submitted. 

![](https://media.giphy.com/media/12NUbkX6p4xOO4/giphy.gif)

Ta-dah! That's Rails magic for ya. Sometimes just walking through the cycle one piece at a time, and explaining it in layman’s terms makes it so much easier to understand, and in turn explain what’s actually going on in this process that takes a few mere mili-seconds to happen. It really does make you stop and think about how much actually happens under the hood whenever you’re simply surfing the web. 
