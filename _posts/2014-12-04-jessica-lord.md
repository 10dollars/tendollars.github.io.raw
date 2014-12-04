---
layout: interview
slug: jessica.lord
title: Jessica Lord - Sheetsee
summary: Visualize information from a Google Docs spreadsheet!
categories: [spreadsheets, visualization, databases, maps]
---

I met Jessica at [Taco Conf](http://tacoconf.com/) when she was at Code for America, and I remember being really inspired by her work as well as the passion she had for it. One of the things I like about Jessica's work is that you get the sense that she really cares about helping people solve problems, and goes about it in a way that gets them started on a track where they can keep improving their solutions. As you'll see, Sheetsee lowers the barrier for visualizing data using tools people are already familiar with. Her project [Git-it](https://github.com/jlord/git-it) is an application that runs in your terminal to help you learn how to use git and github.  

I think a good way to put it is that Jessica makes software that feels welcoming. I look at it and feel comfortable starting something new. 


#### Who are you and what do you do for a living?

I’m [Jessica Lord](http://twitter.com/jlord) and I’m a front-end developer and designer at [GitHub.](http://github.com/jlord)


#### Can you describe [Sheetsee](http://jlord.github.io/sheetsee.js/) really quick?

[Sheetsee.js](http://jlord.github.io/sheetsee.js/) is a client-side library designed to be connected to a Google Spreadsheet (using [Tabletop.js](https://github.com/jsoma/tabletop)) and turning that data into maps, charts and tables—and hopefully then lowering the barrier to entry for having a simple website with visualizations and a simple database.


#### Where did you get the idea for Sheetsee?

The idea for Sheetsee came [during my fellowship year at Code for America](https://www.youtube.com/watch?v=Q76bKK229aM). I was working with the area I grew up in actually, Macon, Georgia, and the budget office wanted to share how they were spending some money the city would be getting through a bond referendum.

I’d just come from 3 years in working for the City of Boston and had taken from that a desire to incorporate some of the useful web services we take for granted, like Google apps, into city government. I also believed that departments should be able to manage and update content on their websites themselves and that we could reduce the bottleneck of tasks a city IT department is asked to handle.

So with that I wanted to use a Google spreadsheet as a database. It was free, didn’t need installing and it wasn’t a new interface to learn, it was a spreadsheet and people were familiar with that. I wanted to make something that was easy to set up with minimal HTML and JS knowledge and even easier to maintain by just editing cells on a spreadsheet.


#### What are some of your favorite uses for Sheetsee? Who has done cool things with it or used to particularly good effect?

Yeah! Some libraries have used it, people have used it to crowdsource information through spreadsheets. Most of the time I don’t know when people are using Sheetsee unless they tell me. Every now and then I meet someone randomly and they say they’ve used it or even been paid to use it and that’s neat!

People have been forking some of the Sheetsee-based projects I have on GitHub and reworking them for what they want. That’s another neat thing about Sheetsee and the fact that GitHub will host website for every repository, you can fork an existing Sheetsee-based project (or any for that matter!), copy the header cells on its spreadsheet, paste them into a new spreadsheet and then edit the spreadsheet url on your fork of the project (which you can do online with GitHub, without Git or a text editor installed). Then you’ll have a website live and hosted connected to data that’s yours. I really think the fork and GitHub Pages tools combined are really powerful and put together a page, [Fork-n-go](http://jlord.us/fork-n-go/), to list some examples.


#### Is Sheetsee done? Is there anything you would like to add to it or clean up?

No way! There are lots of things I’d love to see refined or added. I try to work on it as much as I can, but I am but one person (so, pull requests welcome!). I’d like to make the sorting not just work for the alphabet, I’d like to add marker clustering to maps, it needs tests! I’d love to see more fork-n-go projects built with Sheetsee, and it needs tests! And whatever else is open in the Issues for the repository!
