---
layout: interview
slug: thricedotted
title: Thricedotted - Bots
summary: Thrice has automated everything you love, from cats to sexts
categories: [bot, twitter]
---

#### Who are you and what do you do besides make lots and lots of bots?

I go by [thricedotted](http://twitter.com/thricedotted) on the internet, and I am a 20-something kid living in Seattle going to grad school for computer science. I also have a cat that I like to spend a lot of time petting! That should cover most major axes of my identity.


#### Why do you think it's so satisfying to interact with bots? What do you think it is about Twitter's structure that makes it so appropriate for botmaking?

You're always waiting for a serendipity moment. I think most folks don't have high expectations for a bot's response, but as soon as they're able to read any meaning into it at all, it becomes a little exciting. We -- or at least I -- love pattern recognition and filling in context. When a bot is able to produce content that lets us do that, it's a very satisfying feeling.

With regards to Twitter as the social media site for bots, there are a couple things. Twitter is an easy place to put what I think of as "generator" bots, or bots that produce one certain type of content, to continually generate things forever. I've written a few generator programs in the past, but never knew what to do with them afterwards, since most people (including myself) would probably generate a dozen things and then never use it again. So there's that.

But I think this question was geared more towards chatbots, and in this case, I think it's especially interesting because of the performativity involved. You can talk to a bot, you can talk to your friends, you can talk to a bot in front of your friends. It's different than talking to Cleverbot in your bedroom by yourself. There's something a little more compelling about the interaction.


#### What got you interested in bot making?

So, because I am a hilarious human and definitely not annoying at all, one of my favorite things to do in the past was to create terrible "riddles" on the fly. Well, really what would happen is that I'd notice an overlap between two words, smash them together, and then make up a stupid question involving the definitions of both words in order to get my friends to guess the amazing pun I had just made. It occurred to me at some point that I did this so often, I might as well automate it, and I was frankly shocked to learn that nobody had yet created a portmanteau generator -- thus [@portmanteau_bot](http://twitter.com/portmanteau_bot) was born! After that, I learned more about other people's Twitter bots, and in turn started to have more and more ideas for bots myself, and...well. Here I am.

As a side note, this question made me realize that ever since I launched @portmanteau_bot and [@badjokebot](http://twitter.com/badjokebot), I've been doing the thing with the riddles less these days. Hum.


#### You made a bot for your cat and she is pretty great. Glitch is a bit different for your other bots because, while the exact implementation of your [acrostic hunter](http://twitter.com/acrostik) is still uncertain, the audience can imagine the general methodology behind it. Glitch is just all over the place. How does she work?

I'm pretty proud of glitch (I feel weird capitalizing her name? haha), she is probably a lot simpler than people imagine. I made a couple tweets that alluded to this:

<blockquote class="twitter-tweet" lang="en"><p>part of the beauty of <a href="https://twitter.com/storyofglitch">@storyofglitch</a> is realizing that all this weird shit is stuff that people tweeted about their ACTUAL CATS</p>&mdash; butt empress donkus (@thricedotted) <a href="https://twitter.com/thricedotted/statuses/476871530421702658">June 11, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet" lang="en"><p><a href="https://twitter.com/inky">@inky</a> think of her as the collective consciousness of cats as experienced through the lens of humans who talk about them on twitter :)</p>&mdash; butt empress donkus (@thricedotted) <a href="https://twitter.com/thricedotted/statuses/476872307244531714">June 11, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

Essentially, I'm mining the the Twitter gardenhose for tweets that mention cats, and parsing out actions and characteristics, and then applying a little decoration to them so they come out in glitch's voice. Everything you see glitch do is something that some person has said a real-life cat has done, which is pretty amazing given some of her tweets.


5. Also, how does @acrostik find and choose acrostics?

It's pretty basic -- I stream in tweets from the aforementioned gardenhose, split them into words, and see if the first letters match anything in a dictionary. If they do, then I run it through an entirely arbitrary scoring function that considers the length of the acrostic, the number of "real" words in the original tweet, and whether that word has been tweeted or not before. Every hour, the top scoring acrostic gets tweeted, and the bot starts from scratch yet again.


6. You don't stop answering my questions. I close my eyes and thoughtfully consider your answers. How did [wikisext](http://twitter.com/wikisext) learn to sext?

I gently explain that the idea for a sext bot originally came from my friend [@mayorhumscarrot](http://twitter.com/mayorhumscarrot), who originally proposed that it use steps from recipes. As it turned out, there wasn't a very good recipe API out there, but it occurred to me that (1) that would probably be same-y anyway, and therefore (2) why not use instructions from anything instead? It turns out that it's incredibly easy to grab a random page from wikiHow and parse out the important bits of the instructions, and thus [@wikisext](http://twitter.com/wikisext) was born.


#### How do you find people generally react to your bots when the have unexpected interactions with them?

Depending on what you mean by "unexpected", I'm not sure if I've seen this happen much, haha. I don't keep a very close eye on my bots' mentions, so most of the interactions I see are with people who I follow, who tend to be pretty "bot-articulate". Every once in a while, one of my bots will say something especially poignant/hilarious/lewd and someone will @-mention me so I can appreciate it.


#### What do you look for in a bot idea?

Has it been done before? Will it be funny or interesting or useful for a day or for a week or for a while? I typically don't decide to start working on a bot until I've identified what corpora I would need to make it work, be that tweets or a dictionary or something else entirely. At that point, I prototype and let them grow. A fun thing about my bots is that many of them do have personalities, and that's very intentional, but some things rise out on them on their own. And that's when I feel like I've really hit something.

#### This is really interesting. When you say that some of them have personalities intentionally, do you mean they have a tone for their posts or represent a point of view? I'm curious how much of a reflection of your own personality and perspective you think your bots are?

When I said that, I meant more of a tone for their posts, but some of them also represent obvious points of view: see [@notallbots](http://twitter.com/notallbots) and [@onlymanthings](http://twitter.com/onlymanthings). If anybody were to look at me next to almost any bot I've made side-by-side, I think you'd see a lot of me reflected pretty clearly. It's not especially subtle, I think. Haha.

#### What are some examples of things that have risen out of the bots on their own? That sounds like a really magical experience.

At the time when I was putting glitch together, I wasn't sure what to expect from plugging in tweets, but as I started to generate more examples, I started to hone in on a tone I wasn't expecting. And when I put her up on Twitter, people really did start to treat her like a cat and report on her bad behavior to me. A similar thing happened with @wikisext, in that through very minimal text manipulation on my part, things that ranged from silly to poignant started coming out quickly.

#### What are some of your favorite bots from other people?

So, there are a few mainstream bots that I like, but I'm going to take this opportunity to plug some lesser-known bots:

- [@feelings_js](http://twitter.com/feelings_js) by [@katierosepipkin](katierosepipkin) is a lovely simile bot exploring new emotions each day. I love trying to find ways to interpret what the feelings behind its words would actually be, and the moments when our moods collide entirely.
- [@PROGRAMR_BAT](http://twitter.com/PROGRAMR_BAT) by [@inky](http://twitter.com/inky) posts single lines of source code pulled from a few different programs (he hasn't said exactly which ones :p). I find it interesting for the ways it brings out the human side of code.
- [@libraryofemoji](http://twitter.com/libraryofemoji) by [@aparrish](http://twitter.com/aparrish) imagines surreal new emoji. Perhaps the best so far has been "PHANTASMAGORICAL SYMBOL FOR THREE DISAPPEARANCES". That's an emoji I didn't know I needed until I saw that phrase, and knew that I did.
