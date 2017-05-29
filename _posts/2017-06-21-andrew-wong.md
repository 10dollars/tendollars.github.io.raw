---
layout: interview
slug: andrew.wong
title: Andrew Wong - Astronaut.io
summary:
categories: [youtube, video, undiscovered gems]
---

#### So, the first thing I always ask people is just, "Who are you, and what do you do for a living?"

I'm Andrew Wong and I'm a data visualization engineer. I work freelance right now. Previously, for about four years, I was a logistics engineer at a startup called Postmates.

But I've done sort of like a mix of design and engineering for a while now.

#### Where did the idea for astronaut.io come from?

This is a joint project with me and my friend James.

I asked if he wanted to join but he's he's been traveling and so he's actually asleep right now. But he lives like a block away from me. We were actually roommates when we made this. This was made a long time ago, like 2011.

It came out a loose project prompt that we gave ourselves. We were always hacking on random ideas, and we started to think about what is television really about, and how might we want to create a modern version of that.

We tried lots of different things to explore what that space would look like. Pretty quickly, I think, the idea of extracting content from a live stream became pretty interesting to us. So we tried lots of different things. I think there was a version where we were just getting videos from Twitter as they were coming out. I tried one that would look at all of your email and actually extract all the video that was in there and generate a stream from that.

We also looked at, what it should feel like when you're watching it. One of the ideas was that it should be highly synchronous. Like, when people manipulated the channel, that everybody would see it. There were all these ideas floating around and we pared it down to the the current incarnation, which is to actually use file names that normally show up in memory cards.

That would actually extract videos that had a distinct flavor to them. Very un-edited. They tend to look like videos that weren't really meant to be shared widely. Maybe they were just uploaded temporarily, or they're meant to just be like for that person. And this is very much in contrast to the videos that we were seeing when we tried to do things like Twitter. When someone tweets something, they're actively trying to get attention. Those videos tend to be more like music videos - a lot of commercial things.

So, this particular format of a search on YouTube, I think, yielded much more personal, more realistic content that we found very attractive.

#### In the site's description it mentions that the videos should have a low view count. Is there an actual limit? What's the most view one of those videos could have and still who up?

I don't think I'm explicitly searching for low views. It just happens to be that way. It's a function of both being recent, these are all videos that are uploaded in the last week, and also having a title that's highly unsearchable. The site just crawls through many permutations of these numbers, like IMG 313. That's like one search, and it will get all the videos it can for the week of that search term and then go to, like, 317. So, most of the videos are 0-3 views.

Occasionally you'll see something with maybe 120 or something. But I think the videos predominately have 0 views.

#### Why was it important that everything be that recent? What was attractive about that recency idea.

Because it changes. You know, we would just leave this thing on. It was like a dormant site, like no one knew about it. Usually James and I, we would get together on an annual basis when we were away from our jobs, like winter vacation or something like that, and we were like, "Oh, maybe we should revamp the site a little bit and make it look nicer." We'd check it out and it's all Christmas dinner videos all of a sudden. A few weeks later, it's all fireworks for New Year's. So it's kind like a it's a moving window through time.

I think if you opened up the search window a little larger you'd start to lose that aspect.

#### You mentioned doing upkeep. When was the last time that you updated the site?

I did the bulk of the update, I think, in November. That was after a long time of not doing anything. I think it was actually even just busted for a while because the YouTube API had changed and so the player just broken for a while.

So, in that time I did a few things. I changed the whole UI of the page and made it the way it looks now. There's a space video in the background.

#### Yeah, I was going to say it doesn't look like it was made in 2011.

I think the way it looks now is much more approachable because you're just in it. There's not much to do. I think before it felt a little bit more cerebral. Like, you read this thing first and then we also had controls.

#### It still starts with the the written lead in, right?

Yeah, the written thing originally was like the entire screen. It was like three columns. It was pretty interesting stuff, but we pared it down quite a bit. And there's some hidden features in there.

I didn't really think it was looking at it. I kind of forgot about it. And then one day someone put it on Hacker News. I was in Taiwan at the time, and all of a sudden it just goes down. So I made some more changes after that to try to make it a little more legit. There's a cool little feature if you press spacebar it goes into theater mode.

It's not like it goes fullscreen or anything, what happens is it wipes out the the audio and then replaces it with a soundtrack. So it's more like the whole thing is like one montage.

There's absolutely no indication on the page that you can do that. Surprisingly, people actually do it. When I looked at the analytics, I was like, "Oh people are figuring it out."

#### One of the other interesting things is that the default time is five seconds, but you can decide to stay on the video. How did you guys settle on that kind of interaction model of a little teaser and then the option to extend it?

Yeah, I mean the origins of that was very much about how to sync up people. We had played around with the idea that it was it was like everybody was sharing one remote control. So, if you held it everybody was forced to linger. I think the idea is still kind of the same. You have a slight amount of control to linger or even go back.

#### Oh, I didn't see you can go back.

There's no indication that you can. The old version of the site actually has three buttons. There's go back, hold, or resume. But it's actually incredibly complicated to understand what that means in this context.

#### It wasn't obvious to me that it was like synchronized for everybody either.

This one is not, actually. I was just explaining where it came from. It was originally an experiment to synchronize it. Now it's just at the individual level. I just reduced it down to "hold" to keep it simple.

And yeah the idea is that if you're doing that, the stream is actually still going by.

So you're actually missing videos. You can pull something and hold onto it, but then every five seconds another is still going by. So, when that video you're holding finishes you're thrown back into the stream. To whatever everybody else is seeing.

That underlying stream is actually shared by everybody. Everybody sees the same thing. But you can... I don't know, it's like a sushi boat or something. You can pull it and look at it more carefully, but the conveyor belt keeps going.

#### That's super cool. Is it possible to run out of content? Does that ever happen where you have to loop the feed or anything?

I mean, we probably do run out at the five second level. Like if you don't hold onto everything and you let everything play for five seconds you will loop, I think, if you watched all day.

But it's not like it's pure stream in the sense that a video will never show up again, especially because these are videos from last week so they'll stay around for at least a week. But we try to make it so that it's very unlikely that you'll feel like you're watching things again. I do some things like reshuffling the stream. I think the actual stream itself is rebuilt every day.

#### It seemed like one of the things people respond to well and I was going to read some comments about it was how global it is and how will you jump around.

#### I was wondering if you'd done anything to ensure that or if just like the sheer volume of content makes it so that that's the case.

I think it's the unbiased-ness of the search term. Because the search term is essentially language free. A file format like MOV is universal. It's not language specific, which I think is very useful in that sense.

#### So you mentioned working on that with your partner James. Yeah. How do you guys divvy up the work or go about working on it together.

You know most of those early things, it's just talking, I think. The original thing I remember was we had a pretty good chemistry and were able to work kind of off the technical side for a bit. Just, like, pure concept building.

We were able to play off each other's ideas.

He's he's very strong on the on the product design side of things. And I think, that first version, he designed the way the system would look. I think I remember I was very obsessed, for the first version, to make the videos completely seamless so that you never see a spinner.

That's actually the bulk of the engineering, and it's probably not noticeable to most people, but I think the reason why it just feels like you're watching a continuous stream is because you actually are. When the videos switch, it's not loading another video; the other video is already there. So what's happening is there's actually three players on the screen. 

#### Do you have a favorite video that sticks out something that you discovered watching that you really liked?

Do you remember when the Harlem Shake was a thing? Those just started to infiltrate like crazy, but they were, like, Not. Good. They were not well done. So they're really endearing. It's kind of like you're seeing like the B-reel of this meme.

#### Is there anything that you didn't get to talk about that you want to add just like anything you think is particularly cool that people don't know or like about the process of making it.

I mean, I think the main thing is is just that it will keep changing. Like, the internet moves really fast. I remember very clearly, the videos were really blurry in the beginning.

I don't the high-res stuff it's really that common yet. Now when we look at it it's like, "Wow, all these videos look really sharp." Like really nice videos.

I think that's kind of been the really interesting thing. It serves as a great project for James and I to come back to. Basically, every time we come back it's like, "Hey let's just change it again."

It gives us kind of an annual routine. Like an annual retreat. And at the same time it's like all the content has changed. It's a really nice feeling.
