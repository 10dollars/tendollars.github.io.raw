---
layout: interview
slug: aanand.prasad
title: Aanand Prasad - Slit-Scanner
summary: A bot that morphs your gifs
categories: [bots, gifs, twitter]
---

<blockquote class="twitter-tweet" data-conversation="none" data-lang="en"><p lang="und" dir="ltr"><a href="https://twitter.com/zavtracast">@zavtracast</a> <a href="https://t.co/AVHwNVOnch">pic.twitter.com/AVHwNVOnch</a></p>&mdash; Slit-Scanner (@slitscanner) <a href="https://twitter.com/slitscanner/status/725034258495115264">April 26, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

#### Who are you and what do you do (for a living)?

I’m [Aanand Prasad](https://twitter.com/aanand) and I make software for a living. I work at [Docker](http://www.docker.com/), on [Compose](https://docs.docker.com/compose/). Because it’s important for a growing boy to have a diversity of interests, I also make software in my free time.

#### What is Slit-Scanner?

It’s a [Twitter bot](https://twitter.com/slitscanner) which applies a particular visual effect to any animated GIF you send to it. The effect is known variously as “slit-scan” and “rolling shutter” – essentially, you displace each row of a video progressively further forwards or backwards in time:

Frame 1 becomes (row 1 from frame 1) + (row 2 from frame 2) + (row 3 from frame 3) + …
Frame 2 becomes (row 1 from frame 2) + (row 2 from frame 3) + (row 3 from frame 4) + …
...and so on.

This leads to bizarre and quite varied effects, depending on the type of motion in the video. If people or things are moving left and right, they become transverse waves. If they’re moving up and down, they become rippling longitudinal waves, as if they’re underwater. If they’re rotating around a vertical axis, they become twisted, which is the weirdest effect of all.


#### Where did the idea come from?

I’d been fascinated by slit-scanning for ages, because I’m extremely cool. I think the earliest form I saw it in was the [Scanner Photography Project](http://golembewski.awardspace.com/) ([this image of a moving car is one of my favourite examples ever](http://golembewski.awardspace.com/photographyGallery/vehicles/images/4.jpg)). I’d long been a fan of the “[rolling](https://www.youtube.com/watch?v=eTW0rNgMcKk) [shutter](https://www.youtube.com/watch?v=LVwmtwZLG88) [propeller](https://www.youtube.com/watch?v=y_tm6ECxPmc)” effect – the first time I saw one of those videos, it messed with my sense of reality in a way I’ve rarely felt. [Sha Hwang](https://twitter.com/shashashasha) had already created a bookmarklet for [slit-scanning videos in the browser](http://shahwang.tumblr.com/post/40481891091/the-fight-scene-from-oldboy) using the “static slit” effect to create a still image, and [this short film](https://vimeo.com/7878518) introduced me to the idea of using the “moving slit” effect to create a moving image. Finally, I’d also [experimented](https://www.instagram.com/p/mduZoDR1tY/) a little myself with a slit-scan iPhone app I found on the store.

Anyhow, the idea came to me about half an hour after getting into bed one night, ensuring I’d be incapable of sleep until I’d at least knocked together a basic implementation of the effect.


#### How did you build it?

The same way I build all my bots: copy and paste a load of Python from my other bots into a giant hacky mess. I used thricedotted’s [twitterbot](https://github.com/thricedotted/twitterbot) framework, ffmpeg for extracting frames from videos, Pillow for applying the actual effect and ImageMagick for re-assembling the GIF.

I also used [butterflow](https://github.com/dthpham/butterflow) for smoothing the video beforehand. Most GIFs have a very low temporal resolution (i.e. number of frames), and that results in big chunky rows rather than smooth ripples, so in the majority of cases I double the frame rate before processing it. This is extremely computationally intensive, and makes the bot very slow, but the quality is worth it.


#### What was the biggest challenge making it?

Keeping it running – smoothing the video needs a lot of memory and it’s running on a pretty small VM, resulting in crashes, prolonged downtime and repeated replies. It’s all part of the bot’s “quirky charm”, much like my own.


#### What was the "easiest" part?

Implementing the actual slit-scanning – it worked almost the first time I ran it, and I was back in bed in no time.


#### What was the most surprising thing you learned?

The sheer variety of ways that slit-scanning can make a moving image weird was a big surprise. I was prepared for some cool rotational GIFs and a few interesting wobbles, but it’s come out with so much more. For example, because the time displacement wraps around, the output is always a looping gif, even if the input isn’t. Slow movement becomes [gentle ripples](https://twitter.com/slitscanner/status/723460616116154368); slow zooms [become](https://twitter.com/slitscanner/status/724394120140173312) [optical](https://twitter.com/slitscanner/status/724908713102958592) [illusions](https://twitter.com/slitscanner/status/723575690273153024).

I also love that, with zero knowledge of what’s in the picture, a ridiculously simple 2D transformation can warp 3D objects in a way that feels very convincing, preserving shading and reflections across a virtual surface. Rotational GIFs demonstrate that very well, as do the propeller videos I mentioned before.

#### You've made a number of bots now, and I was wondering what do you look for in a bot idea/project?

Firstly, I’ve never had an attention span (I don’t even know what that is), so every creative project is a race against time: I need to be able to implement it before I get bored. I have a sad graveyard of projects that took just a bit too long and got abandoned.

Bot people, at least the ones I associate with, have strong feelings about bot ethics and etiquette. I’ve thrown away a lot of ideas because they’d be potentially rude/invasive, or because there was a high danger that they’d inadvertently generate upsetting content. It is absolutely the responsibility of the creator to guard against this: our software is infused with our cultural norms, and if you care about changing those for the better, you have to care about your software too.

It’s hard to know ahead of time what will take off and what won’t, but that’s definitely a factor too. I really can’t be bothered making something if I think only three people are ever going to look at it. (It feels good to admit this.)

Finally, a project is especially exciting if I think I might learn something along the way. The ideal difficulty level is “just outside my comfort zone”.


#### Do you have a favorite slit-scan?

[Princess Leia turning her head](https://twitter.com/slitscanner/status/722768869979484160), the image I used for the bot’s avatar. As well as being hypnotically weird and hilarious, I’ve found it to be the best demonstration of what the bot does – people immediately get that time is delayed between the top and bottom of the image.


#### What are some of your favorite bots from other people?

Goodness. I’ll strive to highlight lesser-known works where I can. I’m going to leave out a lot – sorry, everyone.

[George Buckenham](https://twitter.com/v21)’s [manygradients](https://twitter.com/manygradients/status/727456443776024576), [Casey Kolderup](https://twitter.com/ckolderup)’s [wow rude](https://twitter.com/wowwwrude), [Inky](https://twitter.com/inky)’s [botechre](botechre), [Thrice](http://twitter.com/thricedotted)’s [nice tips bot](https://twitter.com/nice_tips_bot/status/576330525016743936), [Darius](https://twitter.com/tinysubversions)’ [Brand New Aesthetics](https://twitter.com/neweraesthetics/status/671673654917361664), [Katie Rose Pipkin](https://twitter.com/katierosepipkin)’s [moth generator](https://twitter.com/mothgenerator/status/622723717865451520), [David Lublin](https://twitter.com/DavidLublin)’s [TV Comment Bot](https://twitter.com/TVCommentBot/status/696193576921866245/photo/1), [Allison Parrish](https://twitter.com/aparrish)’s [Deep Question Bot](https://twitter.com/deepquestionbot/status/577764567343837184), [Nora Reed](https://twitter.com/NoraReed)’s [hydratebot](https://twitter.com/hydratebot).

Finally, I want to do a special shout out to [GameNames](https://twitter.com/GameNames). Very few other people seem to care about it, but I find it debilitatingly hilarious, and have wanted for a long time to make a game based on one of its tweets.

[You can read my interviews with [Casey Kolderup](http://ihadtendollars.com/interviews/casey-kolderup.html), [Katie Rose Pipkin](http://ihadtendollars.com/interviews/katie-rose-pipkin-and-loren-schmidt.html), and [thricedotted](http://ihadtendollars.com/interviews/thricedotted) too :)]

<blockquote class="twitter-tweet" data-conversation="none" data-lang="en"><p lang="und" dir="ltr"><a href="https://twitter.com/shashashasha">@shashashasha</a> <a href="https://t.co/69TvF2KNi5">pic.twitter.com/69TvF2KNi5</a></p>&mdash; Slit-Scanner (@slitscanner) <a href="https://twitter.com/slitscanner/status/725442822493601795">April 27, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
