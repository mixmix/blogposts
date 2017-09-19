# Personal Safety in a p2p Social Network

_I believe in a free and open web.
Over the past 3 years, friends and I have been growing and shaping an ecosystem for that purpose.
It's built with cryptography and is fundamentally p2p.
The result is a system with fundamentally different behaviours than the old web.
This is part of a series exploring the socialogical and technological ramifications - I call it "The Medium is the Message: Cypherspace Edition_

Speaking at a recent [re:publica](https://re-publica.com/) conference, my friend [Rich Bartlett](http://www.richdecibels.com/) threw this challenge:

> If you're going to claim that your project is decentralising power, please explain it in terms of justice, rather than just efficiency and disintermediation

This got me wondeing how our project [Scuttlebutt](https://www.scuttlebutt.nz) is any different?
Most pressing for me was "Can we gaurentee to women or LGBTQI people that they will be safe from bullying and abuse?".

If we can't build a community which is free and open for everyone to participate in - if it's a space where some people are sexually harassed, or receive threats of violence - then we're wasting out time.


Our decentralised architecture certainly makes global spamming attacks hard, and data only flows along lines of trust.
But... it is technically possible for people to abuse others within our community, particularly if you have a lot of friends in common.
In our history to date, we've only had 3 incidents of behaviour and communication that run strongly against the community culture I want to support.

How did we deal with them?


## Just kick them out

On reddit / facebook / twitter / mastodon you can `report` abusive posts to the organisation or moderators.
In a fully decentralised network like Scuttlebutt, **there is no owner** (individual or group) - each user is a fully autonomous agent with total freedom of speech!
They're running on their own hardware.

**There is no physical space that you can own from which you can kick them.**

This is one of the double edged swords of a p2p social network - it's a space safe from authoritarian institutions AND it's harder to assert boundaries.
 

## Have a strong culture

Given we look like a "tech project", the fact that a bunch of the longer standing participants invest heavily in culture might surprise you.
My local Scuttlebutt community is highly self and group-aware.
(It's probably no accident that ecosystem attracts communists, vegans, feminists, sailors, and mycologists.)


When someone presents some rough appearing behaviour, it's common for one or more people to intercede and apply some combination of:
- polite inquiry/ clarifying questions
- assertion of what sort of space we're wanting to build

This costs time and energy, and it's totally worth it.
We get the opportunity to :
- check our own assumptions, and (maybe) build connections with new cultures
- clarify for ourselves what it is we believe in; who we are individually and collectively
- role model what respectful conversation and good boundary setting looks like

We've learnt so much through our conflicts, I absolutely would not take them back.
I absolutely believe this is the fundamental and unavoidable work of community (and community is integral to any human ecosystem).

**This is all really cool and cerebral, but does this stop rape threats?**

(Hasn't happened yet to my knowledge, but it's a decent question IMO.) 


## Block them

This is the feature I've just finished building as a result of the initial challenge.
Applying culture only gets you so far - it can't necessarily protect you from a malicious actor.

In an extreme situation, the things we want you to be able to avoid are:
- this person can no longer contact you
- this person can't stalk you

The first one is easy to implement - you can just tell the interface to not show anything new from that person.
We've decided to go further - you will also no longer replicate / propogate that persons data.

The second part is harder - we're a p2p network, where messages are [gossiped](https://medium.com/enspiral-tales/gossiping-securely-is-the-new-email-6d706d4cd435), how do you want to say to the public community from getting to that person?
You tell your friends, and they respect your decision!

In programmatic terms, a `block` is just another type of message which is gossiped.
As soon as a peer receives it, their local setup effects a change to which information it will pass to the person you're blocking.

In a p2p context, being blocked means you have less peers who you'll be connected to, because the number of people gossiping your messages is reduced.
Highly abusive characters might find themselves enjoying just the freedom of their own speech.


