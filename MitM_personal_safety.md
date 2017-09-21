
# Personal Safety in a p2p Social Network

I believe in a free and open web.
Over the past 3 years, friends and I have been growing and shaping an ecosystem for that purpose — for many, it’s now our primary way of communicating.
It’s built with cryptography and is p2p.
The result is a system with fundamentally different behaviours than the old web.
This is part of a series exploring the sociological and technological ramifications.
I call it “The Medium is the Message: Cypherspace Edition”.

![](https://cdn-images-1.medium.com/max/2000/1*XfNTaNuXnD6DNtDFhM_m8g.jpeg)

Speaking at a recent [re:publica](https://re-publica.com/) conference, my friend [Rich Bartlett](http://www.richdecibels.com/) voiced his lack of faith in blockchain as a solution for all that ails us.
Specifically, he threw this challenge:
> “If you’re going to claim that your project is decentralising power, please explain it in terms of justice, rather than just efficiency and disintermediation.”

This got me wondering how our project [Scuttlebutt](https://www.scuttlebutt.nz), a decentralised social network, is any different from other hype.
Most pressing was the question, “Can we guarantee that people will be safe from bullying and abuse?”
If we can’t build a community which is free and open for everyone to participate in — if it’s a space where some people are sexually harassed, or receive threats of violence — then we’re wasting our time.

Our decentralised architecture certainly makes global spamming attacks hard, and data only flows along lines of trust.
But it’s still technically possible for people to abuse others within our community, particularly if they have a lot of friends in common.
In our history to date, we’ve only had a few incidents of behaviour and communication that run strongly against the community culture I want to support.

So how have we dealt with abuse?

## Just kick them out

On corporate platforms like Twitter, Youtube, or Facebook, there’s a single central organisation with (essentially) a single data storage system.
In that context, it’s easy for the owners of the system to delete content or users — in fact it’s their prerogative and, some would say, responsibility to do so.
Most platforms have a “report” or “flag” feature which marks content or users for review/exclusion.
This can be good, but also results in endless arguments about these rulings, since policing and judging fairly is expensive and difficult.

Companies like Reddit get around some of this overhead by being a platform for community-moderated ‘subreddits’ (channels for specific topics).
Sometimes Reddit admins will still step in and ‘moderate’ user content, like when [their CEO messed with Trump posts](https://www.washingtonpost.com/news/the-switch/wp/2016/11/26/reddits-ceo-regrets-trolling-trump-supporters-by-secretly-editing-their-posts/) , which was simultaneously funny and pretty troubling.

As a federated network, [Mastodon](https://mastodon.social/about) takes this a step further — communities self-host their own ‘instances’ of the platform, meaning there are many self-governing fiefdoms.
Each sets their own rules and can kick content and people off their instance. It’s great because there’s no corporation shaping your experience, and you don’t need one policy to cover all the people in the world.
The challenge is you have to be fairly organised as a group to set up and pay for the infrastructure, and to actively govern your space.

Scuttlebutt goes even further: it’s fully decentralised, with no single central organisation or federation of fiefs. There are only fully autonomous peers, each running the software on their local computer and making their own choices about how they want to interact.
> # **There is no owner of any shared physical space or hardware from which you can kick a person**.

This is the double edged sword of p2p social networks — it’s a space safe from authoritarian interference *and* it’s harder to assert boundaries.

## Have a strong culture

As described above, this decentralisation might sound like total anarchy.
It is, but maybe preconceptions have coloured your expectation of how this might pan out.
In practice, what emerges is not that different to other networks — people migrate toward and away from conversations and people they want to interact with.
We see ‘islands’ or ‘domains’ of community, which might be distinct, overlapping, or totally disconnected.
It’s similar to the dynamics of Twitter, but while Twitter’s global space leaves it open for witch hunts and hashtag storms, Scuttlebutt is more localised and stable.
> # What is culture in such a fragmented space?

I can only talk about the parts of the Scuttleverse I interact with.
It’s filled with open-source programmers, communists, vegans, feminists, sailors, and mycologists — and not capitalism or trolls.

The community space around me has something like emergent governance.
When someone presents rough behaviour, it’s common for one or more people to intercede and apply some combination of:
- polite inquiry and clarifying questions
- assertion of what sort of interaction they’d prefer

This costs time and energy, and it’s totally worth it.


As individuals and as a group, we get the opportunity to:
- check our assumptions, and (maybe) build connections with new cultures
- clarify our beliefs and who we are
- role model what respectful conversation and good boundary setting looks like

Our conflicts have advanced us individually, and as group we have built stronger relationships and are more skilled and articulate.
I absolutely believe this is the fundamental and unavoidable work of community, and that community is integral to any human ecosystem.
> # This is all really cool and cerebral, but does this stop rape threats?

(Hasn’t happened yet to my knowledge, but it’s a decent question.)

![information flows in a peer network](https://cdn-images-1.medium.com/max/2800/1*zMLo7Bf96WzKHTBKs2ZTnw.jpeg)*information flows in a peer network*

## Block them

This is the feature I’ve just finished building.
Applying culture only gets you so far — it can’t necessarily protect you from a malicious actor.

In an extreme situation, the things I want you to be able to avoid are:
1. being contacted by someone
2. being stalked by someone

The first one is easy to implement — you can just tell the interface to not show anything new from that person.
What I’ve built actually goes further, by ceasing propagation of that person’s data to friends of yours not already connected with this person.

The second part is harder.
We’re a p2p network, where messages are [gossiped ](https://medium.com/enspiral-tales/gossiping-securely-is-the-new-email-6d706d4cd435)— how do you say things publicly and have them not get to that person?
You tell your friends that’s what you want, and they respect your decision!

In programmatic terms, a ‘block’ is just another type of message which is gossiped.
As soon as a peer receives it, their local setup effects the change and tops passing information about you to the person you’re blocking.

In a p2p context, being blocked means you have fewer connected peers, because the number of people gossiping your messages is reduced.
Highly abusive characters might find themselves enjoying just the freedom of their own speech, alone.

## **The Medium is the Message**

Marshal McLuhan coined this [iconic phrase](https://en.wikipedia.org/wiki/The_medium_is_the_message), and I’d summarise it roughly as, “The physics of your medium determine what is possible in that medium, and so ultimately the message.”

Given Scuttlebutt is a cypherspace (a space whose foundational physics is cryptography), what is the nature of the medium that is different here, and *what is that message?*

The underlying cryptography is what makes it possible for people to be totally autonomous agents in this social network.
It affords a level of freedom from coercion that is probably unprecedented in a digital space. 
It also removes all responsibility for governance or custodianship of a space from any particular entity and devolves it to the level of individuals making choices.
So far in the Scuttleverse, I’ve seen this lead to a lot of personal responsibility and growth.

It’s also fascinating to watch how the lack of dependence on shared hosting infrastructure means that we can have a multiplicity of overlapping communities.
A recent example was when I found a user, who calls themselves Johnny Null, in the *#dads* channel (which I started because I’m going to be a dad soon, and wanted to talk about that with other crypto-dads).
I was surprised, because I had experienced a lot of antagonistic threads with this person, leading to some of my friends blocking him, but I hadn’t yet.

In this new context, I wasn’t seeing unproductive abuse from him. We found another way to connect on a really human topic.
I was surprised to learn he was a dad, and to receive encouragement and offers of support from him. It was such a sharp contrast from previous interactions.
The diversity of approaches available made it possible for some people to block him, but he wasn’t banned from the network, leaving open new possibilities. I don’t know where that will go … but perhaps we could still have a chance at understanding each other.

I see alignment of the physics of p2p space and the physics of everyday in-person space.
It feels poetic that the way we’ve implemented a block in Scuttlebutt is through communicating boundaries and asking our peers to respect them.
That’s how it works in offline spaces, too.
I see this pattern a lot in what we’re building — p2p interactions mirroring human interaction — and it’s the heart of what I want to communicate by invoking The Medium is the Message.

Building systems with peers means the tools we build might be just a little more human, and make space for adaptive communities.
My hope is that this space will help us re-learn some of what we’ve forgotten in society, and that maybe this will make a difference in the rising challenges we have to face.

![](https://cdn-images-1.medium.com/max/2000/1*Jwt-nzhL8oAsLg7QGnpWFA.png)

*If you’re an excellent human with a rad project you’d like to collaborate on, our little tech coop would love to hear from you. I’m at [mix@protozoa.nz](mailto:mix@protozoa.nz), or you can join the Scuttleverse from [scuttlebutt.nz](https://www.scuttlebutt.nz)*


