# Embracing Subjectivity

prompts : 
  - how can people learn from this talk?
  - how is this accessible for beginners + more advanced 

---

## We've been exploring a subjective space.

What does that mean - it's a net built less on a server-client model, and more on a p2p model.

what if there isn't a node or a logical structure you have to sync up with in order to run a network...

i.e. there's no central source of truth

truth is synthesised, is subjective

We've swapped the problems of centralisation with a whole other bunch of problems.

Sounds scary, but don't worry, you're more qualified than you might think.


SOME ASSUMPTIONS - you can proveably know who said something a thing (and when they said it relative to other things they said.)


## Here's what we've discovered so far ! 

  - identity
    - any @-mention
    - any avatar
    - how: 
      - cryptography (public key = your identity. private key = the secret to your signature)
      - cypherspace

  - boundaries of community
    - there isn't a usage policy, there's just your community
      - encourages community to practice self awareness + ownership
    - example
      - unwelcome conversation

  - 'online' isn't a thing
    - in-sync, or a bit delayed
    - examples
      - at home
      - planes, islands, boats
      - space, or just isolated communities
      - hitch-hikers guides, local peer-maps

  - no ads

  - open database -> interface diversity
    - how do I want to derive meaning?
      - arrangement, filtering
      - history books vs history
    - examples:
      - patchwork
      - patchbay
        - minbay
        - sdash
      - ssb-viewer
    
  - open database -> interoperability for free
    - what if about messages could allow you to add metadata to anything
    - what if replies could be responses to anything
    - what if issues could point at anything
    - ferment
    - git-ssb in patchbay

  - app interface/ db interoperability > swappable modular
    - logic
    - views
      - css
    
  - git on scuttlebutt
    - more logically + architecturally decentralised ... an actual cloud?
    - git repos that I care about are immediately accessible
    - subjective naming

  - just like classic interpersonal meatspace
    - just people talking to each other and figuring things out



## Uncharted territory

How many degrees of gossip are too many?

Multi-device
  - merging identities vs. plugable keys vs. hyperlogs

Private groups?
  - cost of decryption
  - authorisation

How do you visualise the gossip flows

How do you do this well on mobile?

How do you describe foreign lands when there are no common words for what you've seen ?



---




Ideas I care about: 
- plurarliy of truth
  - names
  - perspectives
  - mix

- freedom to interpret
  - what is important
  - how do you engage / interface
  
- sovereignty over what I receive
  - ownership of the interface

- perks
  - freedom from advertising
  - sustainability
  - resiliance

Possible arcs:
- why i'm named mix > history books + discourse > current social media > what's needed to be more subjective > dispensing with usernames, kings > meat space

- here is scuttlebutt > gossip > opinions > subjectivity > names > identity > interface / view (patchbay, patchwork, patchwork-next: diff) > 

- problems with the internet at the moment
  - interface controlled 
    - biased algorithms you have no authorship over
    - no opertunity for diversity in interface
    - unwanted ads
    - data locked away > user lockin (how to represent this as unreasonable? hanging out at the mall?)
  - online
  - filters

- how to make facebook > make a login system > have the data > provide logins for other sources > sell the data > keep the users
- how to make a google > make a login system, proride the toolls > sell the data > provide the services > get the data 
- costs of centralisation > free services, more social, singletons, lockin, proprietary filters.
  - ludites, what are our social values
    > identity, community

- how do you socialise, does everyone carry ID, is everyone called exactly the same thing everywhere?
  - Do you need to authenticate with your government every time you want to do a thing?
    - bookmark (why?)
  - why can't people be lots of things, why do we need to have a login system?
    - authorization / authentication
    - in meat space how do we resolve these things?

Misc notes : 
- reputation / social graph
- authentication vs authorisation


Possible pre-requisites for comprehension: 
- peers
- replication via pubs
- public / private keys
- 


## quotes: 
 - non-digital concepts about how society influences technology and the other way around, borrowing a lot from Franklin's The Real World of Technology. (@keks)
 - cypherspace is the space created by crytography. Its phyics can make certain propieties conducive (such as human autonomy) although not nessicary.+  More importantly what does this enable, if anything? (@null_radix)
 - Embracing Subjectivity also means shifting from designing systems where there is always a single source of truth (say, who is what username?) to one where things can mean different things to different people. This is against the grain of most tech, but is along the grain of everyday life. (@dominic)
- A data structure is subjective if different agents within a system may have an partially overlapping view of it, each agent has a different view of it, and that is okay. (@dominic)


---

talk proposal (thread) %uYUTrSomSmIGv5JkgCqZLSkmsT6wJHh7LSGtiz5hRpY=.sha256

## rough thoughts from earlier: 

### Identity

What is it really ?
We might have got quite used to carrying ID, using our email address as a login, or building servers with usernames.

While these identifiers are quite centralised still some distribution of the work of identity in this :

- facebook trusts that gmail is reliable enough that email auth works
- OAuth / single-sign-on is about 3rd parties confirming other identities
- my power company trusts my bank statements as confirmation of id / address

So people with skin in the game of affirming identity (e.g. when there's money present) are useful and probably going to be useful sources of affirmation of identity.

But there are more people with skin in the game than those in monetary relationships - e.g. friends / family / colleagues. Any of these these can have skin in the game in there will be a negative social impact for false confirmations of id.

Strength of confirmation of id is probably proportional to the amount of damage that can be done. Whether @dominic_temp temp was really a @dominic doesn't have that high stakes when we're just doing conversation. I would probably want to do more checks on that character if he w as asking for money.

### Reputation

This is one of those rat-traps of a problem that I've seen tempt several entrepeneurs. Forcing people to change their behaviour to gather and signal reputation just doesn't work.
Well it doesn't when there's one person trying to form a single view.
When we go subjective, the problem is a lot easier - I have particular ways I value connections around me, and they're a reflection of the reputation I perceive. Friends of mine can leverage this, and /or are welcome to interpret how they see fit.

### Views / filters

ideas around how currently databases and views are welded, but explore what happens when they're not.
Feels more like a dscourse, like how there are many different history books on the same events.
