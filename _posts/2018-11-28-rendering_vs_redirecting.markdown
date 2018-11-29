---
layout: post
title:      "Rendering vs. Redirecting"
date:       2018-11-29 03:07:54 +0000
permalink:  rendering_vs_redirecting
---


I have recently completed my Sinatra Portfolio Project. Getting to this point took dedication—the lessons leading up to the Sinatra Portfolio Project are long and require learners to put in long programming hours. 

Getting through the project proved to be challenging, and had it not been for the endless study groups or litany of pair programming sessions I attended, the project could have been a lot worse.

For this blog post, I decided to take a different angle than I have previously—I have distilled my post down into some key project concepts following this introduction. In hopes to not only better my own understanding of these crucial concepts, but also help students nearing their Sinatra Portfolio Project, I have written this post. Here is one of the most important Sinatra concepts to understand:

### Rendering vs. Redirecting

I cannot stress enough the importance of understanding the difference between rendering and redirecting. Not only will you have to both render and redirect when building your project’s controllers, but you’ll also have to decide when it’s most appropriate to use which. Furthermore, you will be tested on it during your technical project review. So, without further ado, I give you the key differences between the two:

### When to render

Rendering a webpage via a method in your controller is done through the “erb: “/insert-page-here” syntax. “ERB” stands for embedded ruby and refers to the embedded ruby tags programmers use to both render pages through the use of Ruby programming, and embed the Ruby language into plain text documents. The quotes and backslash, followed by a filename, that comes after the “erb” call is the webpage that will be rendered—it takes a reference to a file. So, when and why is it considered best practice to render a page?

•	It follows the “separation of concerns” convention, meaning it ensures that every route and every controller has one job, and one job only.
•	Rendering allows for the URL to match where we want the user to be—if we want to render our “index” page for a user, we can simply match the rendering call to the location specified, i.e. “erb: “/index”.
•	It stores instance variables values.
•	Contrary to redirecting, rendering persists data. Rendering is done when a current request has data that we need.

### When to redirect 

Redirecting to a webpage via a method in your controller is done through the “redirect to “/insert-page-here” syntax. The syntax for redirecting is very straightforward—you begin the request with “redirect” or “redirect to,” followed by the file you wish to redirect the user to. So, when and why is it considered best practice to redirect a page?

•	Unlike rendering, redirecting does not persist data—it resets everything.
•	It is used best for scenarios where new knowledge comes into play, such as signing a user up for a web application.
•	Contrary to rendering, redirecting does not save instance variables.
•	It fires a new “GET” request to wherever you’d like your user to go.
•	Redirecting is used when you do not need the data from a current request.

### Takeaway 

Understanding when to render and when to redirect and the difference between the two actions should be a priority when preparing for your Sinatra Portfolio Project. Not only is it necessary knowledge, but it is crucial to getting through the project as a whole. Understanding these concepts is key to becoming a stronger programmer.

