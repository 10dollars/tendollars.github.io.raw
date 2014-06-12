---
layout: interview
slug: jen.fong-adwent
title: Jen Fong-Adwent - chat.meatspac.es
summary: Chat with animated selfies. A bunch of other stuff.
categories: [chat, community, gifs]
---

#### Who are you and what do you do (for a living)

I am Jen (but people know me as [Edna Piranha](https://twitter.com/ednapiranha)) and I currently work as an Apps Engineer at [Mozilla.](http://www.mozilla.org/en-US/)


#### So, there are a bunch of Spaces. You've got [aux.meatspaces](http://aux.meatspac.es/), the kind of [tumblog project](http://ednapiranha.com/2013/meatspace/); [chat.meatspac.es](http://chat.meatspac.es), the single channel chat room; chatspaces.org, which I haven't used, but looks like group chat with identity but no memory; [facespac.es](https://facespac.es/), for creating channels for selfies; and a beta system of tv stations that I don't have access to yet. I was wondering if you could walk me through the creation timeline and explain how you see all these different outlets fitting together.

It’s pretty funny --- the meatspaces name was originally used as a naming convention for a collection of related node modules starting with decentralized microblogging.

That’s how aux was made, and some other microblog experiments. Eventually, I used the subdomain chat.meatspac.es for the GIF chat which used a module from the group that had nothing to do with decentralized microblogging but just a basic stream of public messages. Then that took over and became known as ‘Meatspaces’ to the world --- so it ended up being the direct association w/ the brand vs. the collection of node modules.


#### What makes looping gifs so ideal for chat? How did you settle on the two second record time?

I think part of it is the repetition as a form of a visual signifier --- replaying causes the viewer to remember that moment from that individual and creates an association to a certain point in time. The two second recording time was something that Sole and I decided on being ideal --- 1 second is too short and 3 seconds makes the file too large.


#### Do the different spaces tend to have the same community, or is there a distinct facespaces community with their own jokes?

I think they are inherently related because it is the same community using both. There is a smaller subset of users on facespaces from the main community and there are some new users who prefer it over chat.meatspac.es, so that may slightly change the experience but nothing drastically different.


#### Choice paralysis and complexity seem to be big themes in your talks. While you start tons of projects, the feature set contained in each one seems strictly monitored and mercilessly narrowed. Can you talk about your philosophy behind building features and breaking them out into their own products?

The tragedy of engineering and design in big business/big projects is the need for features to measure milestones of “success” and change. The problem with this mentality (especially when it is tied to shareholders) is that it actually is detrimental to the product in the long run. Humans are not machines that can memorize and effectively monitor every nook and cranny of a product --- there is so much vying for our attention from so many things that you cannot expect any primary focus to be on your particular invention.

Instead, my belief is that keeping things as simple and minimal as possible help outline the product’s personality, end goal and ultimate lifecycle. At some point all products die and one should be fully aware of this and design for the moment, not for the future.


#### Meatspaces clears all the messages after 10 minutes and chatspaces only retrieves the last 25 messages. Were these decisions made because you expected them to change behavior on the site, or more from a desire to engineer the simplest thing possible?

This was more of a desire to engineer the simplest thing possible --- pagination, archiving, sharing are all features that cause exponential complexity in design.


#### What were some choices for what to include or cut that stick out as being particularly tough call?

Originally we had implemented blacklisting on fingerprints but it proved to be ineffective --- we ended up removing it from chat.meatspac.es shortly after deploying it.


#### The meatspace community seems really close, and it seems like you put a lot of thought into when to open up different parts to new members. Besides controlling growth, how do you think you can help shape an online community like this?

I think it is important to note that it is not entirely up to me to shape this community --- the community shapes itself as it sees fit. So chat.meatspac.es has intentional limitations on growth while facespac.es has multiple channels and can allow users to participate in multiple separate experiences.

Based on observing the interactions in both sites, I can take a better guess on what makes things work and what doesn’t. Sometimes I do ask people what they think about various product directions for future projects, but I do take these with a grain of salt, since what someone states as a good feature isn’t necessarily something that *is* a good feature.
