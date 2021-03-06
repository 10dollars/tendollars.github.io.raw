---
layout: interview
slug: katie.rose.pipkin.and.loren.schmidt
title: Katie Rose Pipkin & Loren Schmidt - infloresence.city
summary: A journal about a city that changes every time you visit!
categories: [generative art, storytelling, algorithms, maps]
---

#### Who are you and what do you do for a living

k: my name is [katie rose pipkin](https://twitter.com/katierosepipkin). i string together a system of odd jobs and incidental work, including; teaching, gallery sales, slinging esoterica, taking commissioned work, web development, public art projects, small grants, murals, and a studio sublet in exchange for my curatorial role at an austin-based arts space. i am a series of symbols that looks like a field of flowers.

l: i’m [loren schmidt](https://twitter.com/lorenschmidt). i work on various digital art projects, including games. i do various odd jobs to help pay the bills, including contract art and programming for other folks’ projects. i also recently started a patreon, which will hopefully help me focus more on my own projects:
[patreon.com/vacuumflowers](patreon.com/vacuumflowers)

#### Could you briefly describe [inflorescence.city](http://inflorescence.city/)? What was the catalyst for the project?

k: infloresence.city is a small journal about a city generated anew every time it is visited.

l: we started with the idea of doing something composed of a number of fragments, and the idea of visiting a city from multiple perspectives arose from that.

<a href="/images/posts/inflorescence/inflorescence1.png"><img height="444" width="500" src="/images/posts/inflorescence/inflorescence1.png"></a>

#### How did you make it / what's it built with?

k: it is almost entirely built in javascript, with html5 canvas as platform for the illustrations. there are also a few programs in ruby (some work there done by the ever-talented [@zonodonoceros](https://twitter.com/zonodonoceros)), and a small twine game.

#### What were the biggest challenges for infloresence.city and how did you get around them?

l: we wanted to make sure the project was accessible. it can be a bit disorienting to come across a wall of generated text and not know what’s going on. i think the way this piece is broken up into diverse segments helps a lot, as does the fact that it’s so visual. it’s also important that everything in the project is coming from a very personal place: people can sense that, and it makes it easier to connect and let it in. we also knew we needed to communicate the nature of the piece to people, so we were careful to present the basics whenever talking about it.

<a href="/images/posts/inflorescence/inflorescence2.png"><img height="427" width="500" src="/images/posts/inflorescence/inflorescence2.png"></a>

#### When we talked earlier, you mentioned this started as a [nanogenmo](http://www.theverge.com/2014/11/25/7276157/nanogenmo-robot-author-novel) project. What about it made you think it was something that should be worked on outside of that event?

k: in short, we ran out of time! i don't think it is an uncommon sentiment when working on large projects within short deadlines, but the place it was by december 1st was fairly shallow of the place we hoped to leave it.

l: that and the pile of ideas we came up with for future projects...

k: bless scope creep.

#### Inflorescence.city is generated anew every time the page loads. Maybe I didn’t visit it enough times, but it seems like certain parts are always the same. Are pieces hard coded? If so, how did you decide what to compose yourself and what to have generated?

k: the pieces that are hard-coded (the news, in particular) are generated from ruby programs that "i was going to get working in the browser". at this point i think i may offer them for a download instead? or perhaps their structure will be re-used for a slightly more elegant version of the same idea. for example, the section with the war-words to flowers (the news), really should be a web portal or browser extension. it is on my vast to-do list.
note: since i wrote this, i published that chrome extension; [it is available for free here](https://chrome.google.com/webstore/detail/rose-colored-window/djlhhopgmokkhnljjlkclknddoododoc/)

<a href="/images/posts/inflorescence/inflorescence3.png"><img height="444" width="500" src="/images/posts/inflorescence/inflorescence3.png"></a>

#### What do you think the generated text adds to the experience for the reader? For instance, the name of the park with the gravestones, and even the city itself, vary, but a reader might only visit once and wouldn’t pick up on it. Does your ideal reader visit more than once? Is the interesting part for you the potential for what could happen?

l: for me, the independence of the process is important. not just knowing that it will be different each time, but having a sense of the software as a creative force with its own notions and tendencies.

k: i am very interested in making individual experiences or artworks for every person who chooses to engage. this iteration of this project used random seed variables to produce that effect- going forward, i am exploring ways to generate work uniquely, but not /randomly/- tracking mouse patterns, browser version, timestamp data, the world of silent information that is unique to each of us on the internet. perhaps this particularization isn’t evident to every visitor, but I hope that it becomes important to those who engage in that way.

l: for future work, i’m really interested in doing things which are location and time specific!

#### I feel like I see something about algorithms having a point of view quite a bit in my Twitter feed. I feel like that is easier to unpack when I’m thinking about algorithms used in products, but I was wondering if you could talk a bit about what it means to write an algorithm for artistic purposes.

l: i think ascribing intent to algorithms is shorthand, a way for humans to be loving and respectful within a human vocabulary. pure algorithms do, on some level, exist outside of human invention. but it’s difficult to draw a line and separate the shape contributed by the computer from that contributed by the human. there is so much crosstalk between humans and computers. our monitors are shaped to fit human eyes, our cultures are reflected in programming languages. 

k: writing an algorithm to produce artworks is sort of like making ten thousand individual pieces at once. the practice of defining rulesets to make the kind of work that you wish to see is similar, but not identical to, making the artwork alone would have been. it is sort of a reversed-process; it takes a broad-scope view of the /what/ those defining characteristics are, how they fit together, what makes them compelling- as opposed to the process of finding an individual feature that moves you, and later seeing that it fits in with all of these others.

#### There are quite a few striking visualizations that get generated and I'm curious what it means in the afterword when you write that these are instances where the "text takes visual form".

l: the illustrator we used for this project is an effort at translating text into a meaningful visual form. the drawings are made by doing one to one translations of parts of the text. the letter q might mean “turn left, then go forward”