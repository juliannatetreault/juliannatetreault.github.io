---
layout: post
title:      "Tackling Flatiron's CLI Data Gem Assessment "
date:       2018-10-25 20:20:41 +0000
permalink:  tackling_flatirons_cli_data_gem_assessment
---


If you’ve gone through Flatiron School’s software engineering course, then you’ve had to tackle their CLI Data Gem Assessment head-on. Being the first of many important portfolio projects, the CLI Data Gem Assessment is a mixture of both creative fun and hard work. The assessment has four parts: the project itself, a video walk-through of the finalized project, a blog post about the project (like this one), and a code review with Flatiron staff. As of writing this, I have finished the project portion of the assessment, and the blog post that goes along with it.

### My CLI Data Gem Project

After much deliberation, I chose to scrape the “Technology” section of the New York Times and built a CLI that lists the latest tech news. 

My CLI works as follows:

After being greeted, the user is given some initial instructions on how to navigate the CLI and is then prompted to make a selection from a list of the latest tech news. From there, the user is able to type ‘menu’ into the CLI to return to the main menu, from where they can select another article to read, or ‘exit,’ which will send the user off with a goodbye message, and exit the program. Furthermore, I took into consideration edge cases when building my CLI—if a user inputs an invalid number, the program will alert the user, display the tech news menu for them again, and suggest that they enter a valid number (1-10) into the terminal. 

### Inside My CLI Toolbox

There are three essential scraping tools that students are advised to use (read: *must use*) when building out their project. The first of the three tools is **open-uri**, which is used to open and read URLs. The second crucial tool is **Nokogiri**, which is a gem that parses through web pages and ultimately allows the user to scrape said web page. Using both open-uri and Nokogiri will get you through all of your scraping needs. The last of the three gems is **pry**. While pry is not necessarily required, I would say that it is just as essential to getting through the CLI project as open-uri and Nokogiri are. 

The final tool in my CLI toolbox was the **colorize gem**. While this gem is not required or necessary to complete the CLI assessment, I highly recommend using it. The addition of color to my CLI was a huge coup—not only did it add a fun twist to what would have been a standard CLI, but it also aided in the separation of key sections in my CLI, making it easier for the user to discern what they must do when interacting with the program.

### Takeaways From the Project 

The lessons I’ve learned after tackling my first portfolio project are invaluable. Completing this assessment has taught me two crucial things:

1. ***Build projects that you are passionate about.***
2.	***Ask for help when you are stuck.*** 

When I first began scraping websites and building out my CLI, I struggled…a lot. I had a difficult time figuring out what I wanted to use my scraped data for and I struggled with envisioning what I wanted my project to ultimately look like. It wasn’t until I entirely scrapped my first CLI project and began building out something I was passionate about – reading and technology – that I was able to conquer this hurdle.

The next hurdle I had to jump was getting over my fear of reaching out for help when I am stuck (read: *imposter syndrome*). While completely irrational, I struggle with asking for help when necessary out of fear that I am in way over my head. Getting past this roadblock is challenging, but every time that I reached out for help, I was always supported. The help I received throughout the project ultimately led me to completing the assessment.

