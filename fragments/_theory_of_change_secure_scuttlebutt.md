This is a workshop I ran with the Secure Scuttlebutt team who all happened to be in San Fransisco recently. Here's what the top of our theory of change diagram looked like :

![](../images/TOS_2.jpg)

Some important things we agreed we need to achieve were :

- specialisation without inequity
- rich ecosystem (supports diverse approaches)

I'd like to explore one particular chain of states back. This format makes it hard to simultaneously discuss the branching and interconnected dependencies, so please forgive me if the analysis seems to narrow. I'm interested in this particular chain because it raised questions which provided a useful frame or lens for projects I'm working on or with. From the top it reads :

1. Galactic council
2. Large scale social harmony
3. Post scarcity
4. Distribution primarily in service of society
5. Distribution is distributed and un-ownable
6. We build our distribution on un-capturable technologies

As distribution surfaced as a theme, we tested our assumptions against real-world examples :

- distribution of food and goods: supermarkets, wal-mart
- distribution of information: email, google, facebook

We observed that **ownership** of distribution by **actors mainly interested in profit** has lead to problematic dynamics which block us from joining the Galactic Council.
See massive food waste, destruction of diversity through monopoly, development of tools which optimise addiction and consumption, development of tools which define value for us.

Some examples
-------------

Here's a breakdown of a couple of interesting cases in the context of information distribution.

**[Email]** : a super successful open protocol. Anyone can send emails to anyone. The failing of email is that it has no mechanism for dealing with un-wanted noise (see spam).
This has generated a niche for organisations to offer value (spam filtering), and capture users.
For example Gmail is popular because it does fairly reliable spam filtering. This makes email less open, because small private servers have a harder time generating a good 'not-spam' reputation.

> Distribution systems must have a solution to noise.

**[Facebook]** : built on an open protocol - http - but has centralised closed databases, and a closed (proprietary) interface.
Facebook's primary motivation is profit, which inclines it to leverage it's closed-ness (right of refusal of access) to extract value from it's user-base.

> All parts of a distribution system need to be uncapturable - open protocols are not sufficient

_[facebook ToS](https://www.facebook.com/terms.php)_

**[Google]** : the growth of the internet beyond easily navigable scales led to the birth of search engines.
The current winning solution to this problem is an algorithm which determes site value based on linkages and references.
Again, this is a niche which has been captured by a primarily profit motivated organisation.
This capture looks something like a monopoly through dependence, and is [defended by a suite of related free and powerful tools](http://techcrunch.com/2011/03/25/search-googles-castle-moat/).

> Distribution systems need to address capturable searchability


Things you should consider
--------------------------

I've named a bunch of assumptions and principles that we think need to be integrated in order to get us on the road to The Galactic Council.

What is your interaction with distribution systems, are you investing in systems that build the future you want to see?

- How do you network online, is it via an actor interested mostly in profit?
- Who holds power over the definition of value of what you're interacting with?
- Where do you publish your content?

I think it's overly idealistic to transition immediately to decentralised uncapturable solutions, but there are small choices that we can and should start making if we want to live in a thriving socirty.

Possible solutions
------------------

### Open-sourcing

![Loomio logo](https://raw.githubusercontent.com/loomio/loomio/master/app/assets/images/logo-orange.png)

With [Loomio](http://www.loomio.org/) (a collaborative decision-making platform), we've addressed some of these same problems by a steadfast commitment to being [open-source](https://github.com/loomio/loomio).
While individual instances of the platform may have closed databases, the open-sourcing of the platform code means that anyone can own and control their own instance. It also makes advertising and data-mining significantly less likely, because anyone in the community can fork the code-base and rip anything extractive out.
For Loomio this is actually a selling point - it's a clear signal that our primary value is in serving society.

With loomio, capturing ownership has also been very seriously addressed in how we've written our constitution, and our approach to investment. In short, you can't buy Loomio, and no one person can control it.

### Publish carefully

![Hypermarkdown logo](https://raw.githubusercontent.com/mixmix/hypermarkdown/master/hypermarkdown_badge_small.png)

You might notice this isn't published on medium. Honestly, this is an experiment in document splicing using a tool I made currently called [Hypermarkdown](https://github.com/mixmix/hypermarkdown). In retrospect this approach does tick some boxes.
This content is currently being hosted at [github.com](https://github.com/mixmix/blogposts/blob/master/uncapturable_distribution.md)... which sounds like my content might be captured buuuut, github is acutally built on a distributed content system called [git](https://git-scm.com/).
An exact mirror of the data lives on my computer as well, and could easily be hosted by any git based server, like a self-hosted [gitlab](https://about.gitlab.com/).

There's still the problem of how it is you've found your way to this blog.
99.9% liklihood is that in 2015 it was via facebook, or twitter (it probably wasn't via google because the way I built this accidently makes it harder to index).


### Build an open combined protocol/ databse

+[About Scuttlebutt](./_about_scuttlebutt.md)

