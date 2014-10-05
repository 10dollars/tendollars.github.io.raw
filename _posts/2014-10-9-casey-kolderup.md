---
layout: interview
slug: casey.kolderup
title: Casey Kolderup - Lonecraft
summary: A persistent Minecraft world. You get one life!
categories: [games, minecraft]
---

#### Who are you and what do you do for a living

I'm [Casey Kolderup](http://twitter.com/ckolderup), a 30-year-old software developer from Indiana living on the east coast of the U.S. I work at [Vox Media](http://www.voxmedia.com/) on the awesome [Vox Product](http://product.voxmedia.com/) Team, which builds the software that powers the hundreds of blogs and news sites we own and operate.

#### You've got a lot of interesting choices that I could have chosen from. Most notably, the currently-down-soon-to-be-resurrected [Narratron](http://narratron.com), [PutHTML](http://puthtml.com), and [Backtracks](http://backtracks.co/). I chose Lonecraft because I think the core concept is interesting in its own right, but it's also a great example of someone picking up someone else's idea (in this case, [Chain World](http://en.wikipedia.org/wiki/Chain_World)) and running with it.

#### Can you describe basics of Chain World and the features you built to make it your own?

Chain World was an idea that indie game designer [Jason Rohrer](https://twitter.com/jasonrohrer) brought to a game design competition at the Game Developers Conference in 2011. GDC is one of the biggest industry shows in gaming, and I find Rohrer's work really fascinating because I think he's really good at taking what's on his mind and turning it into a game in a really unfiltered way that makes you react pretty strongly to it whether you like it or not. The full story of Chain World is [outlined here](http://www.wired.com/2011/07/mf_chainworld/all/); the short version is that he set up a system of loose rules around a USB thumb drive containing a licensed copy of Minecraft that at the surface level played with themes of religion (the theme of the competition he debuted it at), civilization, oral tradition, and death. In the process of getting the community involved in the experiment he also managed to create an interesting situation in the community involving themes of privilege, celebrity, social cliques, money, and general internet drama.

At the time that all of this was happening, I was also pretty into Minecraft and was thinking a lot about my own relationship with the game. I had [written an essay](http://warpskip.com/post/1648277202) the previous winter about what I wanted to get out of the game and that spring had started to explore the unofficial Minecraft modding scene to see if I could make the game play in a way that fulfilled some of what I was looking for out of it. When Chain World came out, I was stunned and I wanted to play it so badly, but I knew that there was no chance I'd ever get my hands on it. Distressed at the idea that Chain World was bound and made inaccessible to regular folk by social politics and physical limitations, I realized that the Internet was the perfect tool to launch a subversion of Chain World that put an infinite number of Chain Worlds into the hands of the people.

I found a Minecraft plugin that could whitelist specific usernames on a server while keeping everyone else out, then wrote my own plugin that could send HTTP requests from the Minecraft server to another web server when certain in-game events happened. Next, I wrote a web application you could log into and associate your Minecraft account username with an email address. Then I set things up so that when a player died in Minecraft, it immediately banned them from the server, then notified the web app that they had died. It emailed a token -- sort of like a gift card code -- to that person, and they could forward it on to someone else. Anyone could come to the website with that code and sign up with their Minecraft username; the first person to do so would be white listed on the Minecraft server and given the login details so they could play until they died.

In doing all this I think I created a pretty reasonable facsimile of the Chain World idea that could be set up by anyone with a free Heroku account and a fairly cheap Amazon EC2 instance.

#### As someone who is pretty terrible at Minecraft and dies frequently, I don't really have  a great concept of how long someone's life is. When I read the description of Lonecraft, I imagine a lone figure stumbling upon both crumbling monuments and small encampments in a world "haunted" by those who have come before. For example, maybe you find a really sophisticated home or rail system, but you might also just be walking by a hill and see that some random blocks have been dug out and wonder why someone would have done that.

#### Do you have a sense of how long any one person got to spend in that world? Would there have been enough time to build really big structures?

There were only ever two Lonecraft worlds created but peoples' playing styles were definitely very different. Some people wanted to make a splash and set up all kinds of explicit messaging with signs full of text, self-referential jokes and such. Other people played like they may have played a normal offline game, building structures for survival purposes.

The shortest game was under an hour long (me, being stupid). The longest was over a week although I'm not sure how many play sessions happened during that time. Some people have played enough Minecraft that they're pretty good at staying alive! I never got amazing at it, so I don't think the controls ever felt quite as natural as I think they have to a lot of the game's players.

#### Were these lives long enough to impact the journaling process once they died? Like, would they forget things? Did you consider having them do chat in-game and logging all that text?

Logging game chat never occurred to me! The journaling only really came later (like, I rushed to add the feature during the second playthrough) because once people were outside the world they wanted to share what they had seen but some of them seemed to have mixed reactions about the idea that they might spoil something for someone who might play later. The idea with journaling on the web app was that I could create a safe space where a player could record their experiences immediately without fear of spoiling for anyone-- I could limit the exposure of journal posts only to users of the web app who had already played and died as well, and then once the world had "ended", we could open up the journal to the public while also offering the "completed" world maps for download (a feature I never actually finished because the logistics of uploading that all to S3 or similar kinda bored me).

#### In order to facilitate the archiving, you put a 10 game cap on the world by default. I'm curious how that went. Were you happy with that time horizon / number of players? Were there any really big games that you're aware of?

I mostly scrambled to add the hard user limit to the game during the first playthrough when people were staying "alive" for 4-5 days at a time, which might only be one or two actual play sessions but I wanted to keep things moving and give people the chance to play more than once since they were also immediately clamoring for that (a really obvious drawback of a single persistent world that I somehow hadn't anticipated while first setting things up!)

The 10 round limit seemed to work okay as far as the timing of shutting down the first game and starting up the second-- I also intentionally ran the two tests with different social groups, although I would sometimes put people in touch with others who had been playing so they could get looped in since I was mostly trying to make sure the token didn't get stuck waiting for a player at any point during those early tests.

#### In your blog post, you mentioned that this was your ideal way to play the game. What did you personally get out of playing in a Lonecraft server that wasn't there in a regular solo experience?

For me, a really big part of the experience of Minecraft was the mystery of what was possible, so my most intense experiences were early on in playing the game when I didn't know all the rules of that universe and I was discovering what could be built, and what could be... out there. During my first days with Minecraft I didn't really know if I traveled far enough if I'd find evidence of civilization or what.

Once the game became much more about the online community, obsessing over patch notes, watching YouTube Let's Play series, and so forth I found myself enjoying the game in a different way but it was never the same as when I was trying to figure out things like how switches worked without looking at FAQs on how to do it.

#### Are there any surviving journals?

I have three journal entries from the last three people who played (basically after I finally got the prototype of the journal feature working) but there's a lot of weird in-jokes and I'm not sure it even makes sense to me anymore. I lost the game world files shortly after shutting the site down (which is what convinced me to finally sign up for offsite backup on my personal computer!)

#### How long did Lonecraft run? Is it something you have any interest in resurrecting?

It was basically running for a month in mid-2011. I got busy with some life/career stuff and unfortunately the tricky part ended up being maintaining a Minecraft server running a number of unofficial plugins during one of the fastest development periods Minecraft had-- the API was constantly changing, breaking plugins, and I had to go in and upgrade mine, then either wait for the plugins I relied on to update or try to modify them myself. It was hard to keep up!

I think it'd be cool to go back and finish up some of the journaling stuff (get the world download bits finished, fix bugs in the journal reading stuff, and figure out how to make it easy to share screenshots in your journal posts)... I've also learned a lot as a developer since then so I feel like I could probably rewrite the web app part from scratch and it'd be more stable, more secure, etc in a much shorter time than trying to work with code I wrote almost 4 years ago.

That said, I have no idea what the Minecraft plugin scene looks like at this point, and I also feel like maybe Minecraft proved itself to be this thing totally different from the austere mysterious thing I wanted it to be. And that's great! I'm amazed to see what people who really love Minecraft have done and continue to do with it and fully admit to having watched probably a hundred hours of Youtube videos of people playing through really creative story maps or various challenge maps; it brings back a lot of the feelings I have about some of the game creation systems like [ZZT](http://en.wikipedia.org/wiki/ZZT) and [Megazeux](http://vault.digitalmzx.net/index.php) that were so important to me as a young person, and I don't want to fight against what is obviously an awesome thing.
