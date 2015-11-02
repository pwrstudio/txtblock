# txtblock
_Reading in the shade of the Merkle Tree_

*Rasmus Svensson & Hanna Nilsson ([PWR])*

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*

– [Julian Assange. Hans Ulrich Obrist In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011.]( http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/)

## Introduction

In this text, we describe a decentralized tool for publishing and distribution of digital text. We propose a format called the Block: a sharply defined, eternal, immutable unit of information. The Block is the successor of the Book.

Through a cryptographic link between the identifier and the content, or even the embedding of the content within a cryptographic control structure, the system is made tamper-proof and resistant to censorship. 

We see this proposal as one small contribution to the internet renaissance. 
 
## Background

What does it mean "to publish" in a society where every thought, movement and moment is recorded and stored? Let's say that publishing is simply the act of making something public and drawing attention to it. And let's agree that the opposite of public is private. 

Public and Private. In the past, these two spheres were clearly defined and separate. Today they overlap and merge and melt together on a IKEA couch. In the context of traditional publishing, the action of printing, binding and distributing a book was an unmistakable step from the private to the public sphere. The writer in her chamber working on the manuscript, bringing it to the publishing house and so on down the production line. In contrast, current info-tools work in a grey zone in-between, obfuscating where data ends up and how it is exploited.

After the revelations of the last years it has become increasingly clear that the categories "private" and "public" need to be re-defined to give the user the choice of where on this private/public spectrum she is communicating. We also find it useful to introduce a second axis: temporary/private, to allow us to re-consider the lifespan of information: to give us, the users, the choice between forms of communication from burn-on-read to eternal-life. 

As a step in this direction we believe there is a point in re-asserting the category of "the book" – beyond – meaning the creation of stable and clearly defined units of public information, something that can be uniquely referred to in public discourse independent of central authorities and big commercial interests.

The humble aim of txtblock is to enable eternal identification of clearly defined immutable units of textual information. 

We see the Block (the name we use for the published text unit) as existing on the extreme point of both the private/public and the temporary/permanent scale: a Block is public and permanent. An inscription in stone. The block is the book is the brick.

## Proposal 

We see txtblock as consisting of three components:

1. Catalogue
2. Storage
3. Interface / Format

Point one and two, catalogue and storage, rely on the blockchain-infrastructure provided by the [Ethereum] platform. This makes them fairly uncomplicated to implement. This allows us to focus on the interface and the conceptual and aesthetic format of the Block.   

### Decentralized catalogue

The core component of txtblock is a decentralized catalogue containing cryptographic fingerprints, or hashes. These provide an absolute reference to the publications – uniquely based on the content. This catalogue is the autonomous point of authority. A smart contract, a simple program on the blockchain, allows publication and retrieval of units of texts.

The specific technology that enables this is [Ethereum], a decentralized platform that runs smart contracts. Fundamentally it is a system, based on blockchain database technology, allowing the agreement between nodes in a network without a central authority. The integrity of the system is maintained through the economically incentivized cryptographic labour of the participating machines. Publishing is simply the operation of making an entry into this distributed, public database. The catalogue functions without human involvement.

In contrast to for example an [ISBN] or [DOI] number, a _yinn_ is directly tied to the information it identifies. By using a [cryptographic hashing function], a fingerprint of the information is created. Changing a single letter in the text will completely change the fingerprint. A modified file would, therefore, fail verification against the catalogue. This allows certainty that the text you are reading is indeed the exact text that was published.

### Decentralized storage

How to store the actual texts? Two alternatives.

1. The sensible, scalable solution. Recommended best practice: The catalogue, **on** the blockchain, contains a reference to the text which is stored **off** the blockchain, on a [Content-addressed, distributed, peer-to-peer file system.](http://ipfs.io)

2. The more conceptually and aesthetically pleasing alternative: The text itself is stored directly **on** the blockchain, embedded within it. Piggybacking on the piggybank. Might be considered "bloat" or vandalism. But according to the market logics that govern To write a letter to the blockchain costs 0.00005 US dollar. Publishing the text we are reading to you right now would cost about 50 cent – paid to the nodes of the network who perform the labour of writing it to the database. 50 cent – considering that this price theoretically buys your text eternal life this is not too bad...

### Format: limits and æsthetics

_txtblock_ is designed for publication of pure text. In this sense, it exists in the lineage of the book.

Why not images, video, embedded html5? There is value in limitations. It makes the creative possibilities more apparent. To avoid the slippery slope of adding features we propose a strict, minimal framework: 

unicode symbols
displayed in a monospace font 
laid out in 64 character lines

In this way, we would get a strict grid where letters line up vertically giving the writer a rudimentary but predictable control of the layout. The Block exists somewhere in the intersection between concrete poetry and code.

The interface will be strictly typographic with all of the design encapsulated in an open-source monospace, fixed-width font, designed in collaboration with typographer and artist Raphael Bastide.

Current e-book formats (e.g. ePub) try to adapt the book/publication-concept to things that are not a good fit for it (interactivity, variable content, etc…) making it into a less good version of already existing forms (web-sites, games) 

Others are simply ways of commodifying information – Apple's iBook, Amazon's Kindle. This is worse than pointless...

We think there is a core of the Book that can serve a purpose today and in the future. This is, in contrast to many other forms of communication, as sharply defined units of information that, once published, once bound, are permanently frozen. Objects you can point to, discuss and critic.  

## Conclusion

What does the blockchain look like? A hovering, glowing network diagram? A cloud? The google-approved material-design color scheme? Is it gold, silver or the color of oil? A pile of coins? A tower of Babel built in Lego? 

Physically it is mining-units lined up in warehouses in China, or north of the polar circle in Sweden, or amateur machines spinning away in closets. 

Functionally it is block stacked on block stacked on block, each one locking the previous one in place.

*"We need to posit a collectively controlled legitimate vertical authority in addition to distributed horizontal forms of sociality, to avoid becoming the slaves of either a tyrannical totalitarian centralism or a capricious emergent order beyond our control. The command of The Plan must be married to the improvised order of The Network."*

– [Alex Williams and Nick Srnicek. #ACCELERATE MANIFESTO, 2013](http://criticallegalthinking.com/2013/05/14/accelerate-manifesto-for-an-accelerationist-politics/)

The blockchain could be the Merkle Tree that enables the Rhizome, the necessary hierarchical element providing control and coordination.

The current web is based on a business model of spying on users and selling the information. We believe we're at a very interesting point where a combination of blockchain technology with peer-to-peer file systems gives the tools for re-inventing the web, and opening possibilities to other models beyond giant data centers, Amazon Allowance and Walled Gardens. 

_txtblock_ is an experiment in this direction. 


[Ethereum]: https://github.com/ethereum/wiki/wiki/White-Paper
[cryptographic hashing function]: http://emn178.github.io/online-tools/sha3_256.html
[IPFS]: http://ipfs.io/
[PWR]: http://pwr.site 