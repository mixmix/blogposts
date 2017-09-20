# Personal Safety in a p2p Social Network

_I believe in a free and open web.
Over the past 3 years, friends and I have been growing and shaping an ecosystem for that purpose - for many, it's now our primary way of communicating.
It's built with cryptography and is p2p.
The result is a system with fundamentally different behaviours than the old web.
This is part of a series exploring the socialogical and technological ramifications - I call it "The Medium is the Message: Cypherspace Edition_

Speaking at a recent [re:publica](https://re-publica.com/) conference, my friend [Rich Bartlett](http://www.richdecibels.com/) voiced his lack of faith in blockchain as a solution for all that ails us.
Specifically, he threw this challenge:

> If you're going to claim that your project is decentralising power, please explain it in terms of justice, rather than just efficiency and disintermediation.

This got me wondeing how our project [Scuttlebutt](https://www.scuttlebutt.nz) is any different from other decent hype.
Most pressing was the question "Can we gaurentee to women or LGBTQI people that they will be safe from bullying and abuse?".

If we can't build a community which is free and open for everyone to participate in - if it's a space where some people are sexually harassed, or receive threats of violence - then we're wasting our time.


Our decentralised architecture certainly makes global spamming attacks hard, and data only flows along lines of trust.
But... it is technically possible for people to abuse others within our community, particularly if you have a lot of friends in common.
In our history to date, we've only had 3 incidents of behaviour and communication that run strongly against the community culture I want to support.

How did we deal with them?


## Just kick them out

On corporation run platforms like twitter, youtube, or facebook, there's single central organisation with (essentialy) a single data storage system.
In this context, it's easy for the owners of the system to wipe content or users - in fact it's their prerogative, and may be in the best interests of their business.
Most platforms have a "report" or "flag" featute which marks content or users for review and/ or exclussion.
This can be good, but there's also endless arguments about rulings as policing and fairly judging reports is expensive and often contentious.

Companies like Reddit get around some of this overhead by allowing communities to start 'subreddits' - channels for specific topics which are moderated by volunteer members.
Sometimes Reddit owners will still step in and 'moderate' user content, like [when their CEO messed with Trump posts](https://www.washingtonpost.com/news/the-switch/wp/2016/11/26/reddits-ceo-regrets-trolling-trump-supporters-by-secretly-editing-their-posts/) - simultaneously funny and pretty troubling.

As a federated network, [Mastodon](https://mastodon.social/about) takes this a step further - it's a community groups self-hosting their own 'instances' of a platform.
This means there are many self-governing fiefdoms.
In this context, the community hosting the instance can kick content/ people off their setup.

It's great because there's not corporation shaping your experience, you don't have to have one policy to cover all the people in the world.
The challenge is you have to be fairly organised as a group to set up and pay for the infrastructure, and to actively coordinate the governance of your space.

Scuttlebutt goes even further - it's fully decentralised, there is no single central organisation, there is no federation of fiefs, there are only fully autonomous peers with total freedom of speech, each running the software on their local computer.

That is, **there is no owner of any shared physical space/ hardware from which you can kick a person**.

This is the double edged sword of p2p social networks - it's a space safe from authoritarian institutions AND it's harder to assert boundaries.


## Have a strong culture

As described above, this decentralisation might sound like total anarchy.
It is, but maybe mainstream media has coloured your expectation of how this might pan out.
In practice, what emereges is not that different to other networks - people migrate toward and away from conversations and people that they want to interact with.
We see 'islands' or 'domains' of community which might be distinct, might overlap, or might be totally disconnected.
It's similar to the dynamics of Twitter, but while Twitters global space leaves it open for witch hunts and hashtag storms, Scuttlebutt is more localisedand stable.

> What is culture in such a fragmented space? 

I can only talk about the parts of the scuttleverse I interact with.
This looks a lot like open-source programmers, communists, vegans, feminists, sailors, and mycologists, and it doesn't look like capitalism, trolls.

The community space around me has something like an emergent governance.
When someone presents some rough appearing behaviour, it's common for one or more people to intercede and apply some combination of:
- polite inquiry/ clarifying questions
- assertion of what sort of interaction they'd prefer

This costs time and energy, and it's totally worth it.
As individuals and as a group, we get the opportunity to :
- check our assumptions, and (maybe) build connections with new cultures
- clarify it is we believe in, and who we are
- role model what respectful conversation and good boundary setting looks like

Our conflicts have advanced us individually, and as group we have stronger relationships, and are more skilled and articulate.
I absolutely believe this is the fundamental and unavoidable work of community (and community is integral to any human ecosystem).

> This is all really cool and cerebral, but does this stop rape threats?

(Hasn't happened yet to my knowledge, but it's a decent question IMO.) 


## Block them

This is the feature I've just finished building as a result of the initial challenge.
Applying culture only gets you so far - it can't necessarily protect you from a malicious actor.

In an extreme situation, the things we want you to be able to avoid are:
1. being contacted by someone
2. being stalked by someone

The first one is easy to implement - you can just tell the interface to not show anything new from that person.
What we've built actually goes further by ceasing propogation of any of that persons data - this means friends of yours not already connected with this person won't receive contact from them.

The second part is harder.
We're a p2p network, where messages are [gossiped](https://medium.com/enspiral-tales/gossiping-securely-is-the-new-email-6d706d4cd435) - how do you say things publicly and have them not get to that person?
You tell your friends, and they respect your decision!

In programmatic terms, a `block` is just another type of message which is gossiped.
As soon as a peer receives it, their local setup effects a change to which information it will pass to the person you're blocking.

In a p2p context, being blocked means you have less peers who you'll be connected to, because the number of people gossiping your messages is reduced.
Highly abusive characters might find themselves enjoying just the freedom of their own speech.


## The Medium is the Message

_["The medium is the message"](https://en.wikipedia.org/wiki/The_medium_is_the_message) - Marshal McLuhan coined this iconic phrase, and I'd summarise it to roughly mean "the physics of your medium detemine what is possible in that medium, and so ultimatley the message"._

Given Scutlebutt is a cypherspace (a space whose foundation and physics are cryptography), what is the nature of the medium that is different here, _what is that message?_

The underlying crytography is what makes it possible for people to be totally autonomous agents in this social network.
This affords a level of freedom from coercian of larger actors this affords is probably unprecedented in a digital space.

We also see that it removes all responsibility for governance or custodianship of a space from any particular entity.
So far in the Scuttleverse, I've seen this leading to a lot of personal responsibility and growth.

It's also fascinating to watch how the lack of dependence on shared hosting infrastructure means that we can have a multiplicity of overlapping communities.
A recent example was finding a user who calls themself "Johnny Null" in the `#dads` channel I'd started (I'm going to be a dad soon, and I'm talking about that with other crypto-dads).
I was surprised because there had been a lot of antagonistic threads with this person, and this led some of my friends to block him.
It seems like I simply unfollowed them.

The dynamic that emerged from that diversity of approaches was that I was seeing no more unproductive abuse, and I wasn't seeing that many posts from this person.... until we found another way to connect on a really human topic.
I was surprised to learn this human was a dad, and to receive encouragement and offers of support from them - such a sharp contrast from previous interactions.
I don't know where that will go ... but it felt like possibility, like perhaps we could still have a chance at understanding each other.


I guess my final mention would be the apparent alignment between the physics of p2p space, and the physics of everyday in person space.
It feels poetic that the way we've implemented a block in Scuttlebutt is through communicating boundaries and asking our peers to respect those. 
I see this pattern a lot in what we're building, in honesty it's the heart of what I want to communicate by invoking The Medium is the Message.

Building systems out of peers means the tools we build might be just a little more human, and make space for adaptive community.
My hope is that this space will help us re-learn some of what we've forgotten in society, and maybe, just maybe, this will make a difference in the rising challenges we have to face.

