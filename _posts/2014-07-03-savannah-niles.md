---
layout: interview
slug: savannah.niles
title: Savannah Niles - Tether
summary: A Meditation on Space
categories: [geolocation, status]
---

#### Who are you and what do you do?

I’m [Savannah Niles](http://www.savannahniles.com/), and I’m an artist and a researcher based in Cambridge, Mass. I build systems designed to operate where digital information and physical environments make exchanges. I’m a graduate student at the [Media Lab at MIT](http://www.media.mit.edu/), working with the Viral Spaces group.

#### What is Tether?

[Tether](http://www.tether.cc/) is a site allows anyone to memorialize a moment or a loss that is tied to a specific location by pinning a white X and an associated <1200 characters of text to a specific location on a simple, web-based map. Anyone can browse the map and its submitted X's.

Over time, the map decays. X's on the map tend to slowly drift away from their origin point. When an X is clicked, the distance in miles the X has traveled to arrive at its current location is displayed under its text. A button available in the clicked-on X allows the viewer to choose to re-tether the X to its origin point, or let it continue drifting on.

The site was developed for the 50th anniversary of JFK’s assassination, and shown at an accompanying exhibition, [*The Artists’ Commission*](http://blog.savannahniles.com/post/67368033700/gray-matters-gallery-invites-you-to-the-opening), at Gray Matters in Dallas, TX, curated by Sally Warren. At the site of JFK’s assassination on Elm Street in Dallas, there’s a [white X](https://www.google.com/search?q=jfk+elm+street+x&espv=2&source=lnms&tbm=isch&sa=X&ei=hl60U4WsGMqrsASdi4CYBQ&ved=0CAYQ_AUoAQ&biw=1419&bih=695) painted on the pavement. Tether references and extends that image.

#### How did you build it?

Tether is built in Ruby on Rails and the Google Maps API. It’s a super simple site. You can check the [repo](https://github.com/savannahniles/JFK) out on GitHub if you want to examine, extend, or otherwise dismantle the project.

Probably the most notable feature of Tether is that the notes left by participants "drift" away from their point of origin over time and visitors can decide whether or not to return them to where they started. How did you hope this would change the user's relationship with the notes? Did you have a chance to find out what people thought of that aspect of Tether?

Well the notes seem sort of autonomous, right?, drifting through a virtual world on their own. So when building this, I thought the defining characteristic of the X’s was impermanence: they’re always wandering off. I predicted that people’s responses to this would fall somewhere along a range of whimsy/anxiety.
In some ways that played out: from team whimsy, I got an email from someone who excitedly reported that her first kiss had entered the Pacific; on team anxiety, Michael Corris [wrote](http://glasstire.com/2013/12/12/the-artists-commission-at-gray-matters/) that Tether reveals that “we are unwilling to allow this particular memory to drift, either into a sea of forgetfulness or to be gathered up and molded by others into some unrecognizable or irrelevant avatar of the past.”

But by the care and attention evidently given to the text of many of the notes left on the site, it appears that many people see in the X’s opportunities for preservation, or permanence, albeit windswept. When you log on, the site loads the X’s in your current location, and to my surprise, some people seem to respond with greater interest to the shifting region of discoverability of an X, regardless of its origin point.

#### This project makes me think of [memori.al](http://www.savannahniles.com/memori-al) a bit. Possibly because a lot of the x's on Tether seem sort of sad to me, but also because there's an aspect of impermanence or fuzziness. Memories shared on Tether became less and less accurately linked to the place the occurred over time and memories on memori.al are literally forgotten by the system once they're read.

#### What do you find most interesting about the space where artificial and human memory intersect? What's your opinion on the crop of ephemeral sharing apps we've seen recently?

Alternative memorials are a deep interest of mine, so I also see Tether and Memori.al as engaging a shared set of ideas. We use the rhetoric of memory to describe data storage, but memory as we experience it cognitively is a kind of anti-data: unreliable, unresolvable, and irreproducible, always of seemingly higher-bandwidth than our expressive transmission capacities. But yeah, there is an apparently crucial, or at least unshakable, analogy between human and computer memory—and it’s further complicated by the extent to which we depend on computer memory to externalize our human memory, with our images, social lives, economic transactions, and biometric data all critically synced to the cloud. And I think this analogy extends questions that we already have around our own memory— What if we forget? What if our memories are wrong? Is this really the most reliable mechanism for holding on to the things we’ve lost? Our digital systems—like memory-prostheses—are now subject to the same unease.

But I really love SnapChat. So many interesting hardware and software development happens in response to the ephemera of just being alive. SnapChat, Slingshot, etc. are significant in what they discard, and this orchestrates certain kinds of social interactions. (Have you downloaded Yo? I love Yo. Yo’s are just so powerfully inscrutable.) Then at the other extreme, Quantified Self apps, [Narrative](http://getnarrative.com/), and so on, remember everything—and is that overdoing it? Or deeply satisfying? Idk. But (a line from Funes the Memorious might apply here:) there’s “a certain stammering greatness” to the recollection-capacity of modern computing, and noticing this likely inflects our experiences with software, with memory, and with day-to-day i/o.
