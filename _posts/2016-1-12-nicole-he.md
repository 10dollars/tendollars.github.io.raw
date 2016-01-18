---
layout: interview
slug: nicole.he
title: Nicole He - True Love Tinder Robot
summary: Computer Mediated Love
categories: [art, tinder, robots, love, itp, disembodied hands]
---

Nicole's True Love bot has everything you could want in a project: romance, robots, suspense, the slightest feeling of helplessness, a single disembodied hand – everything! As Nicole says in her description of the robot, "This project explores the idea that the computer knows us better than we know ourselves, and therefore it has better authority on who we should date than we do. In a direct way, the True Love Tinder Robot makes the user confront what it feels like to let computers make intimate decisions for us." I think it looks like a really successful project in that regard.

After you read this, you should check out the Nicole's documentation for the project. She's set up [a page](http://nicole.pizza/true-love-tinder-robot/) answering some of the more common questions and showing off a video of the robot in action. You can also read her [process blog](http://nicole.pizza/itp/tag/tinder-robot/) to see the robot's development unfold. It has early sketches, code, and even a breakdown of all the parts and how much they cost. I kind of wish every project was this well documented, but then I probably wouldn't be able to keep this site up.

<a href="/images/posts/nicole/true-love-tinder-robot.gif"><img src="/images/posts/nicole/true-love-tinder-robot.gif"></a>

#### Who are you and what do you do for a living?

I'm a graduate student at NYU [ITP](https://tisch.nyu.edu/itp), which is like Hogwarts but with computers. I currently do nothing to make a living, which is both terrible and wonderful (mostly terrible).

#### Can you tell us a little bit about the True Love Tinder Robot? How did you make it, and how did you decide that this was what you wanted to work on for your ITP project?

[The True Love Tinder Robot](http://nicole.pizza/true-love-tinder-robot/) was a project I made for two of my classes at ITP. It's a robot that reads your feeling as you are looking at Tinder profiles, and then decides whether or not you are attracted to that person. If you are, the creepy robot hand will physically swipe right, and if you are not, it will swipe left. It also talks to you the whole time about your involuntary choices.

I woke up in the middle of the night with the idea for this robot. I decided to run with it because I thought it would make people think about how much we trust computers with intimate decisions, and also because I thought it would be a funny project.

#### How did you decide the robot should talk?

It was important to me that the robot express its personality. Doing this visually by showing another screen was out of the question, since the user should be focused on looking at the Tinder profiles. So it made sense to make the robot speak.

The way it talks to you is a big part of the experience, because it makes you feel like it's a little bit judgmental about what's going on. But it has the right to be, because it knows better than you. All of this adds to the question of how much we want to trust a computer with something so personal.

#### How does the bot decide if it's love?

It measures galvanic skin response, which is essentially how sweaty your palms get and how that changes over time. When we are excited or nervous (the familiar feelings of love!), our palms get just a little bit sweatier. Using an Arduino, the robot can then read how the electrical conductivity of your skin changes.

The True Love Tinder Robot knows better than you because it knows how you *truly* feel when you look at a person, and therefore you aren't swiping based on how you *think* you feel.

#### If it's sweaty palms, does the bot start matching you up more over time? Do we look like we're getting more desperate to the True Love Robot?

Not necessarily - it measures the *change* in how sweaty your palms get, so if you have naturally sweaty hands, it doesn't mean that you'll swipe right more. It depends on how your body reacts to each individual Tinder profile.

But yes, the robot may judge you if you're swiping right a lot.

#### How have people generally been reacting to it?

There's been a surprising flurry of response to the robot! I think it activates people's anxieties about internet dating, biometric devices, and our own intimate relationships with computers. The people that have actually gotten to try the robot find it a little sassy, I think. But of course, it's because the robot knows best.

#### What was the biggest challenge making it?

The physical fabrication was the most difficult part for me, because I have no experience in that area, and like a dumb person I did not take a class on it this semester. Drilling holes is scary for me!

#### What was the "easiest" part?

I guess since my unconscious mind came up with the idea while I was sleeping, that was the easiest part.

#### What was the most surprising thing you learned?

I was surprised at how much of a reaction there has been to this project across the web and in the news, but I think people pretty much will eat up anything based around Tinder. Also, this may be cheesy, but I learned that I could come up with an original idea for something that I find interesting, and then code it and build it myself. That was pretty nice.

#### What's the most intimate decision you've let a computer decide?

This, my friend, is a secret between me and my computer.
