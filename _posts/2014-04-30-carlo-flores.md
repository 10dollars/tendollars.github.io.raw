---
layout: interview
slug: carlo.flores
title: Carlo Flores - EdgeCats.net
summary: Director of Engineering EdgeCast
categories: [cats, gifs]
---

#### Who are you and what do you do?

My name is Carlo Flores and I try to do cool things with computers.  I help lead a team of Software Engineers at [EdgeCast Networks](http://edgecast.com) (now Verizon Digital Media Services) as well as co-organize [LA DevOps](http://meetup.com/ladevops) and [js.la](http://js.la), two of the best damn meetup groups in Los Angeles.  

#### What is edgecats?

[edgecats.net](htpp://edgecats.net) has cat-gifs-as-a-service, because, hey, who doesn't need more cat gifs?

It's really just a little [Node.js](http://nodejs.org) app using [Express.js](http://expressjs.org), which is a micro web framework for quickly building sites.  I had never built an Express app before but kept hearing great things about it and loved [one of the pieces of software](http://sinatrarb.com) that inspired it.  One of the best things has been that folks out there have actually forked the application and that [Matt Austin](https://github.com/matt-), an old teammate from an old shop, even showed me some bonehead mistakes that caused security on my servers to be compromised.  So I guess it's more than just a goofy service because it's also been an excuse to learn and try new things.

#### Where are all the EdgeCats gifs from? Do you have a collection of your own?

I don't keep a collection of gifs around on a harddrive, so storing them on a webserver was one of the wins of edgecats.  Gifs are contributed by the community via pull requests on github, or by excellent gifs linked to me in various chats and Reddit, of course.

#### Any normal cat loving person can land on the site and get a cat gif right away, but there's actually a surprising amount of functionality built into edgecats. You can plug edgecats.net/auto to get a new cat every 60 seconds, or use /random to get a link for a random cat gif. You can even get a list of all cat gifs, or, if you're brave, can show all the cat gifs at once. Did you set out to make a resource for people building sites to be able to use cat gifs, like [Place Kitten](http://placekitten.com/)?

Yes!  When I first started at EdgeCast we built a testing framework to ensure our software worked as expected.  The first use case for edgecats was simple: if all tests pass, our dashboard featured cat gifs.  If any test did not pass, no cat gifs.  It was an effective motivator.

#### How did you decide what features to build in? Are there any new features you want to add in the future? Anything you're dying to fix?

All the features have come in based on user need or to allow myself to use cats whenever possible on other projects.  A good one was when edgecats got quite a bit of Reddit and Twitter traffic which led to a HUGE amount of bandwidth use.  At that point I brought in edgecats.net/meow as a dirty trick to allow cached images and reduce the internet bill.

#### Where did netcat come from?

One of our former designers [Tianhe Yang](https://twitter.com/tianheyang) put it together over a day as an homage to Nyan Cat and terminal programs.  Try dragging him around the screen for a hidden feature!

netcat has been used for various parties in various places as well, since the -auto flag on a projector beats old timey hipster style black and white movies any day of the week, but twice on caturdays.

#### Is this [subreddit](http://www.reddit.com/domain/moar.edgecats.net) related to your edgecats? I've never seen a subreddit set up like that. Did it come about because of Reddit's interest in edgecats, or is that something you set up and promoted?

I think that's just a collection of Reddit posts that have used edgecats!  I do not think there is a dedicated edgecats subreddit, but you'll find the webservice makes an appearance at /cats, /catgifs, and /gifs fairly regularly.

#### Are you a domain hoarder? What's the best domain you've got sitting idle right now?

It's not totally idle, but I own http://dumbaas.com, which will probably totally be the next big Internetting as a service.  You should send me angel funding now while you still can.  Or just please don't hack it too bad.
