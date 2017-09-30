---
layout: interview
slug: andrew.wong
title: Andrew Wong - Astronaut.io
summary: A peek at small moments from around the world
categories: [youtube, video, undiscovered gems]
---
[Astronaut.io](http://astronaut.io/) was made by [Andrew Wong](http://twitter.com/wongavision) and [James Thompson](https://twitter.com/astrojams1) in 2011. It crawls youtube for videos that have been uploaded in the last two weeks with generic filenames like dsc 001 and turns them into a feed of small intimate moments from around the world. Watching for just a couple of minutes, I saw multiple class presentations from around the world, an offroad expedition on ATVs, an oddly close up view of a goldfish, a volleyball game, a play, a few baby videos, someone documenting a car accident, video of foam boxes being broken down by a machine, and one guy filming his crotch in boxers.

It is mundane and amazing. The fact that the people who uploaded these files didn't name them makes me think they probably wouldn't expect anyone to see them, which does create a mild sense of voyeurism, but since the feed jumps around so quickly I don't ever feel like i'm lingering and leering.

In some ways, I feel like it is a product of its time. I'm no internet scholar, but in 2011 I feel like we were still grappling with the idea of how things that felt semi-private because of the scope of the internet were actually public and could become *very* public *very* quickly as social media got bigger. For some reference, in 2011 [Nick Douglas](http://twitter.com/toomuchnick) was posting an [open letter](http://knowyourmeme.com/memes/scumbag-steve) from the guy in the Scumbag Steve photo to the girl in the Annoying Facebook Girl meme.

RIP Slacktory.

The project instantly reminded me of this old reddit thread about being able to [search for the first image someone posted from their camera.](https://www.reddit.com/r/pics/comments/evkqo/sometimes_i_like_to_search_for_dsc00001jpg_in/) from the same year.

The current version of astronaut.io feels like it is less about the fact that we can find these videos with low view counts, and more about creating a sense of what life is like around the world by focusing on the moments we aren't trying to go [mega-vi](https://www.fastcompany.com/3056057/how-buzzfeeds-jonah-peretti-is-building-a-100-year-media-company).

#### So, the first thing I always ask people is just, "Who are you, and what do you do for a living?"

I'm Andrew Wong and I'm a data visualization engineer. I work freelance right now. Previously, for about four years, I was a logistics engineer at a startup called Postmates.

But I've done a mix of design and engineering for a while now.

#### Where did the idea for astronaut.io come from?

This is a joint project with me and my friend James.

It came out of a loose project prompt that we gave ourselves. We were always hacking on random ideas, and we started to think about, "what is television really about?" and how might we want to create a modern version of that.

We tried lots of different things to explore what that space would look like. Pretty quickly, I think, the idea of extracting content from a live stream became pretty interesting to us. We tried lots of different things. I think there was a version where we were just getting videos from Twitter as they were coming out. I tried one that would look at all of your email and actually extract all the video that was in there and generate a stream from that.

We also looked at what it should feel like when you're watching it. One of the ideas was that it should be highly synchronous. Like, when people manipulated the channel, that everybody would see it. There were all these ideas floating around and we pared it down to the the current incarnation, which is to actually use file names that normally show up in memory cards.

That would actually extract videos that had a distinct flavor to them. Very un-edited. They tend to look like videos that weren't really meant to be shared widely. Maybe they were just uploaded temporarily, or they're meant to just be like for that person. And this is very much in contrast to the videos that we were seeing when we tried to do things like Twitter. When someone tweets something, they're actively trying to get attention. Those videos tend to be more like music videos - a lot of commercial things.

This particular format of a search on YouTube, I think, yielded much more personal, more realistic content that we found very attractive.

#### In the site's description it mentions that the videos should have a low view count. Is there an actual limit? What's the most view one of those videos could have and still who up?

I don't think I'm explicitly searching for low views. It just happens to be that way. It's a function of both being recent, these are all videos that are uploaded in the last week, and also having a title that's highly unsearchable. The site just crawls through many permutations of these numbers, like IMG 313. That's like one search, and it will get all the videos it can for the week of that search term and then go to, like, 317. So, most of the videos are 0-3 views.

Occasionally you'll see something with maybe 120 or something. But I think the videos predominately have 0 views.

#### Why was it important that everything be that recent? What was attractive about that recency idea?

Because it changes. James and I would get together on an annual basis when we were away from our jobs, like winter vacation or something like that, and we were like, "Oh, maybe we should revamp the site a little bit and make it look nicer." We'd check it out and it's all Christmas dinner videos all of a sudden. A few weeks later, it's all fireworks for New Year's. So it's kind like a it's a moving window through time.

I think if you opened up the search window a little larger you'd start to lose that aspect.

#### You mentioned doing upkeep. When was the last time that you updated the site?

I did the bulk of the update in November, I think. That was after a long time of not doing anything. I think it was actually even just busted for a while because the YouTube API had changed and so the player just broken for a while.

So, in that time I did a few things. I changed the whole UI of the page and made it the way it looks now. There's a space video in the background.

#### Yeah, I was going to say it doesn't look like it was made in 2011.

I think the way it looks now is much more approachable because you're just in it. There's not much to do. I think before it felt a little bit more cerebral. Like, you read this thing first and then we also had controls.

#### It still starts with the the written lead in, right?

Yeah, the written thing originally was like the entire screen. It was like three columns. It was pretty interesting stuff, but we pared it down quite a bit. And there's some hidden features in there.

I didn't really think anyone was looking at it. I kind of forgot about it. And then one day someone put it on Hacker News. I was in Taiwan at the time, and all of a sudden it just goes down. So I made some more changes after that to try to make it a little more legit. There's a cool little feature if you press spacebar it goes into theater mode.

It's not like it goes fullscreen or anything, what happens is it wipes out the the audio and then replaces it with a soundtrack. So it's more like the whole thing is like one montage.

There's absolutely no indication on the page that you can do that. Surprisingly, people actually do find it. When I looked at the analytics, I was like, "Oh people are figuring it out."

#### One of the other interesting things is that the default time is five seconds, but you can decide to stay on the video. How did you guys settle on that kind of interaction model of a little teaser and then the option to extend it?

Yeah, I mean the origins of that was very much about how to sync up people. We had played around with the idea that it was it was like everybody was sharing one remote control. So, if you held it everybody was forced to linger. I think the idea is still kind of the same. You have a slight amount of control to linger or even go back.

#### Oh, I didn't see you can go back.

There's no indication that you can. The old version of the site actually has three buttons. There's go back, hold, or resume. But it's actually incredibly complicated to understand what that means in this context.

#### It wasn't obvious to me that it was like synchronized for everybody either.

This one is not, actually. I was just explaining where it came from. It was originally an experiment to synchronize it. Now it's just at the individual level. I just reduced it down to "hold" to keep it simple.

And the idea is that if you're doing that, the stream is actually still going by.

So you're actually missing videos. You can pull something and hold onto it, but then every five seconds another is still going by. So, when that video you're holding finishes you're thrown back into the stream. To whatever everybody else is seeing.

That underlying stream is actually shared by everybody. Everybody sees the same thing. But you can... I don't know, it's like a sushi boat or something. You can pull it and look at it more carefully, but the conveyor belt keeps going.

#### That's super cool. Is it possible to run out of content? Does that ever happen where you have to loop the feed or anything?

I mean, we probably do run out at the five second level. Like if you don't hold onto everything and you let everything play for five seconds you will loop, I think, if you watched all day.

But it's not like it's pure stream in the sense that a video will never show up again, especially because these are videos from last week so they'll stay around for at least a week. But we try to make it so that it's very unlikely that you'll feel like you're watching things again. I do some things like reshuffling the stream. I think the actual stream itself is rebuilt every day.

#### It seemed like one of the things people respond to well is how global it is and how much you jump around.

#### I was wondering if you'd done anything to ensure that or if just like the sheer volume of content makes it so that that's the case.

I think it's the unbiased-ness of the search term. Because the search term is essentially language free. A file format like MOV is universal. It's not language specific, which I think is very useful in that sense.

#### You mentioned working on that with your partner James. How do you guys divvy up the work or go about working on it together?

You know, most of those early things... it's just talking, I think. The original thing I remember was we had a pretty good chemistry and were able to work kind of off the technical side for a bit. Just, like, pure concept building. We were able to play off each other's ideas.

He's he's very strong on the product design side of things. I think, that first version, he designed the way the system would look. I think I was obsessed, for the first version, with making the videos completely seamless so that you never see a spinner.

That's actually the bulk of the engineering, and it's probably not noticeable to most people, but I think the reason why it just feels like you're watching a continuous stream is because you actually are. When the videos switch, it's not loading another video; the other video is already there. What's happening is there's actually three players on the screen.

#### Is there anything that you didn't get to talk about that you want to add?  

I think the main thing is is just that it will keep changing.

Like, the internet moves really fast. I remember very clearly, the videos were really blurry in the beginning. I don't think the high-res stuff was really that common yet. Now when we look at it it's like, "Wow, all these videos look really sharp."

I think that's kind of been the really interesting thing. It serves as a great project for James and I to come back to. Basically, every time we come back it's like, "Hey let's just change it again."

It gives us kind of an annual routine. Like an annual retreat. And at the same time, all the content has changed. It's a really nice feeling.
