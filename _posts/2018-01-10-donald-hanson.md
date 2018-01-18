---
layout: interview
slug: donald.hanson
title: Donald Hanson - Permanent Redirect
summary:
categories: [art, scarcity, the search, cool urls changing]
---
About a week ago my girlfriend watched me click on a link over and over again for several minutes. I thought I saw her re-evaluating some life decisions when I said, "I'm getting closer," despite the fact that nothing on the page seemed to change. Once I finally showed her what I'd been working towards it was unmistakable. But I was truly pleased. Seeing the trail of digital breadcrumbs leading me to Donald Hanson's [elusive art page](http://permanent-redirect.xyz) was low key exciting, and I thought the concept was really fun.

<a href="/images/posts/permanent-redirect/permanent-redirect.png"><img src="/images/posts/permanent-redirect/permanent-redirect.png"></a>

#### Who are you and what do you do for a living?

I'm a new media artist and freelance web developer in Oakland California. I spend about half my time working on client projects and the rest working on personal projects. This year I'm doing 52 weeks of media art projects, and Permanent Redirect was the first one.

#### What is [Permanent Redirect](http://permanent-redirect.xyz)?

It's a net art piece that moves to a new URL every time someone views it. But it also leaves a link to its new location, so you can follow the links to eventually arrive at the art piece. It has resulted in a very long chain of nearly identical pages. It was intended to make the artwork harder and harder to access.

#### How'd you get the idea?

I've been thinking a lot lately about how the traditional art market is different from how digital artwork is valued. There's a whole generation of digital artists who's work gets endlessly replicated, driving the value down. There's no sense of urgency in seeing a digital artwork when it's free and available to everyone all the time. I wanted to create an experiment that introduced some kind of scarcity into a digital artwork.

#### What's it built with?

Nothing special. Just PHP and a MySQL database for the hit counts on each page. I initially made the pages contain their own hit counts, and had each page modify itself when it was viewed. That didn't work out so well when multiple people were viewing pages at the same time. And yes, each redirect page is a unique file on my server.

#### Is there anything you'd like to improve or change?

I would like to find a way to prevent bots from pushing the art along. I've been blocking IPs when I see their number of requests skyrocket, but ideally this would be automated. Additionally, the final number on the art page became really inaccurate and inflated once bots started hitting the art. I would have wanted the number to reflect unique visitors to the page, rather than just the number of hits to the page.


#### What was the hardest part of the project?


Keeping the thing online when people were clicking as fast as they could. This was still in the beginning when I was using self-modifying pages, so they kept getting truncated and endless loops would emerge.

Also deciding what I wanted to be at the end. The experiment is really about the way the piece moves, and less about what is at the end.

#### What was the "easiest" part?

The promotion. I only had to make one tweet and it took off. I still don't know who from my tiny follower base initially retweeted it, but I should find them and thank them.


#### When I was clicking I started to wonder if the whole thing was an elaborate joke with nothing actually being moved. One of the things that kept me clicking was that I was able to see when it was last accessed, so I could start to see myself getting closer. It felt like a linear path.

#### It occurred to me that you could kind of skip the line if you had a link from someone who had seen it recently. I was thinking that you could have kind of social aspect with someone handing out good link position, and sharing them around Twitter or a forum. And no matter what, that link would become less valuable over time.

#### It's kind of the opposite of how finding something typically works. People usually get more recognition for handing out earlier artifacts like demos, first editions etc, but with Permanent Redirect the newest person's link would always be most useful. Was that something you thought about at all?

I didn't expect people to pay attention to this project at all, let alone share links to good shortcuts to the art. I initially had the counters max out at 9999 because I thought there was no way it would go over that.

It turned out to have all sorts of social implications that I didn't think about. For instance this point it's extremely difficult to reach the art just by manually clicking through the redirects. The people who were able to use automation to get to the art and push it along have become essentially the only people who are able to see it at this point.

#### How many people have seen the art at this point?

It's impossible to know how many "people" have seen it, but the counter on the art is over 135,000 now. Mostly due to bots.

####What have the reactions been like?

In the beginning people were really excited to reach the art after a few clicks. I saw one person hashtag #isawtheart and I thought that was great. Once it got to over a thousand clicks, people were still doing it manually and coming back disappointed at the end. I never said the "art" would be worth that much clicking, but it has been very interesting to see the range of responses and how it changed over time.

#### Has anything about the response to the project surprised you?

All of the response! It's normal to create stuff and have very few people notice. This was a crazy way to start off my 52 weeks of media art, and I can only hope I haven't peaked on the first week. Keep an eye on my twitter [@donald_hans0n](http://twitter.com/donald_hans0n) and website [https://donaldhanson.net](https://donaldhanson.net) for updates an all my new projects.

#### Notes
The tag is a reference to this article by Tim Berners-Lee - [Cool URIs don't change](https://www.w3.org/Provider/Style/URI)
