# txtblock
Reading in the shade of the Merkle Tree

*Rasmus Svensson & Hanna Nilsson ([PWR])*

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*

– [Julian Assange. Hans Ulrich Obrist In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011.]( http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/)

## Introduction

In this text, we describe a decentralized tool for publishing and distribution of digital text. We propose a format called the Block: a squarely defined, eternally immutable unit of information. The Block is the successor of the Book.

The Block is cryptographically bound. It is given a name that is directly derived from the content, so that changing a single letter will be clearly detectable. In this way it is made tamper-proof and resistant to censorship.

We see this proposal as a small contribution to the Internet Renaissance. 
 
## Background

What does the verb "to publish" mean in a society where every thought, movement and moment is recorded and stored?

Let's say that publishing is simply the act of making something public and drawing attention to it. And let's agree that the opposite of public is private. Public and private. In the past, these two spheres were clearly defined and separate. Today, they overlap and merge and melt together. In the context of traditional publishing, the acts of printing, binding and distributing a book was an unmistakable step from the private to the public sphere. The writer in her chamber, working on the manuscript, bringing it to the publishing house and so on down the production line. In contrast, many current info-tools work in a grey zone in-between, obfuscating where data ends up and how it is exploited.

After the revelations of the last years it has become increasingly clear that the categories "private" and "public" need to be re-defined to give the user the choice of where on this private/public spectrum she is communicating. Is the message meant for one special person? Or for the community of all intelligent lifeforms? Should it expire after five minutes? Or persist until the last bit of information succumb to entropy?

We see the Block as existing on the extreme point of both the private/public and the temporary/permanent scale: a Block is public and permanent. An inscription in stone. The Block is the Book is the Brick.

The humble aim of txtblock is to enable eternal identification of clearly defined, immutable units of textual information. 

## Proposal 

txtblock consists of three components:

1. Catalogue
2. Storage
3. Interface / Format

Point one and two, catalogue and storage, rely on the blockchain infrastructure provided by the [Ethereum] platform, leaving us to focus on the interface and the conceptual and aesthetic format of the Block.   

### Decentralized catalogue

The core component of txtblock is a decentralized catalogue containing cryptographic fingerprints, or hashes. These provide an absolute reference to the publications – uniquely based on the content. This catalogue is the autonomous point of authority keeping track of what has been made public and when the publication was made. A smart contract, a program on the blockchain, allows publication and retrieval of units of texts, the Blocks.

The technology that enables this is [Ethereum], a decentralized platform that runs smart contracts. Fundamentally it is a system, based on blockchain database technology, allowing the agreement between nodes in a network without a central authority. The integrity of the system is maintained through the economically incentivized cryptographic labour of the participating machines, a digital [scriptorium](http://41.media.tumblr.com/21b3c3e36c8ab901deaf0d6d32417a7f/tumblr_mvsmxuO0m11soj7s4o1_1280.jpg). Publishing is simply the operation of making an entry into this distributed, public database. The catalogue functions without human gatekeepers.

In contrast to an ISBN number, a txtblock-identifier is directly tied to the information it identifies. By using a [cryptographic hashing function], a fingerprint of the information is created. Changing a single letter in the text will completely change the identifier. A modified file would, therefore, fail verification against the catalogue. This allows certainty that the text you are reading is indeed the exact text that was published.

### Storage

How to store the actual texts? Two alternatives:

1. The sensible, scalable solution. Recommended best practice: The catalogue, on the blockchain, contains a reference to the text which is stored off the blockchain, on a [Content-addressed, distributed, peer-to-peer file system.](http://ipfs.io)

2. The more conceptually and aesthetically pleasing alternative: The text itself is stored directly on the blockchain. Merging the ledger and the book. Piggybacking on the piggybank. The text is kept safe as long as there is value stored on the chain. Some would consider this an abuse of the blockchain. We disagree. Writing to the blockchain is relatively expensive. One letter costs 0.00005 US dollar. Publishing the text you are reading right now would require a one-time payment of about 60 cent. This is too much for most applications – but txtblock is meant for the very special kind of information that you want to commit to eternity. Text is compact compared to other media so the cost, according to current market-prices on the Ethereal network, is reasonable – and even perhaps a desirable feature adding a threshold you have to cross to go from private to public.

### Format: limits and aesthetics

txtblock is designed for publishing of pure text. In this sense, it exists in the lineage of the typographic book.

Why not images, video and other richer media? There is value in limitations. It makes the creative possibilities more apparent. To avoid the slippery slope of adding features we propose a strict, minimal framework: 

    unicode symbols
    displayed in a monospace font 
    laid out in 64 character lines

In this way, we construct a strict grid where letters line up horizontally and vertically, giving the writer a rudimentary but predictable control of the layout. The Block exists at the intersection of concrete poetry and code. The interface of txtblock is strictly typographic with all of the design encapsulated in an open-source monospace, fixed-width font.

Current open ebook formats (e.g. ePub) try to adapt the book concept to things that are not a good fit for it (interactivity, variable content) making ebooks an inferior version of already existing forms (web-sites, games, apps). Other formats are simply ways of commodifying information and locking it to a proprietary platform (e.g. Apple's iBook, Amazon's Kindle).

We think there is a core of the Book that can serve a purpose today and in the future. This is, in contrast to many other forms of communication, as sharply defined units of information that, once published, once bound, are permanently frozen. Objects you can point to, discuss and criticize. This core is what we call the Block.  

## Conclusion

What does the blockchain look like? A hovering, glowing network diagram? A cloud? The google-approved material-design color scheme? Is it gold, silver or the color of oil? A pile of coins? A tower of Babel built in Lego? 

Physically it is mining-units lined up in warehouses in China, or north of the polar circle in Sweden, or amateur machines spinning away on drying racks in repurposed guest rooms. 

Functionally it is block stacked on block stacked on block, each one locking the previous one in place.

*"We need to posit a collectively controlled legitimate vertical authority in addition to distributed horizontal forms of sociality, to avoid becoming the slaves of either a tyrannical totalitarian centralism or a capricious emergent order beyond our control. The command of The Plan must be married to the improvised order of The Network."*

– [Alex Williams and Nick Srnicek. #ACCELERATE MANIFESTO, 2013](http://criticallegalthinking.com/2013/05/14/accelerate-manifesto-for-an-accelerationist-politics/)

The blockchain could be the Merkle Tree that enables the Rhizome, the necessary hierarchical element providing control and coordination.

The current web is based on a business model of spying on users and selling the information. We believe we are at a very interesting point where a combination of blockchain technology with peer-to-peer file systems gives the tools for re-inventing the web, and opening possibilities to other models beyond giant data centers, Amazon Allowance and Walled Gardens. 

txtblock is an experiment in this direction. 


[Ethereum]: https://github.com/ethereum/wiki/wiki/White-Paper
[cryptographic hashing function]: http://emn178.github.io/online-tools/sha3_256.html
[IPFS]: http://ipfs.io/
[PWR]: http://pwr.site 