# b10.hk

**DRAFT 2**

*Rasmus Svensson & Hanna Nilsson (PWR studio)*

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*

– [Julian Assange. Hans Ulrich Obrist In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011.]( http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/)

## Introduction

In this text we outline a decentralized platform for publication and distribution of digital text. The purpose of the system is to enable long-term persistence of sharply defined, immutable units of information. Through a cryptographic link between the identifier and the identified (a digital fingerprint) the system is made tamper-proof and resistant to censorship. We see this proposal as one small contribution to the internet renaissance. 

A smart contract, currently implemented on the [Ethereum] protocol and blockchain, acts a decentralized catalogue ( _babel_ in the local terminology of _b10.hk_) allowing publication and retrieval of units of texts (called _blocks_).

As with most catalogues, _babel_ does not contain the actual content but only a reference: a hash (called _yinn_). The _yinn_ can then be used to find the _block_ in a content-addressed, distributed, peer-to-peer file system, such as [IPFS].       

As all the specifications and code is made public, a _reader-writer_ can interact with _babel_ and the _blocks_ in whatever way they choose. One way is the typographic interface we are building at the address _b10.hk_.   

## Background

What does the verb “to publish” mean in a society where every thought, step and moment is digitized and stored? 

According to the dictionary, “publishing” is either the business of producing books and magazines or – secondarily and more broadly – the act of making something public and drawing attention to it. The first definition is archaic and we leave it behind in the age of paper, but the second seems worth considering: What does "public" mean? Again consulting the dictionary we see that it is the opposite of "private". In the past these two spheres where clearly defined and separate. Today the line is blurred. The action of printing, binding and distributing a book was an unmistakable step from the private to the public sphere. In contrast many current publishing tools work in a grey zone in-between, actively hiding where data end up and how it is exploited.

After the revelations of the last years it has become increasingly clear to many that the categories _private_ and _public_ are in need of re-definition to give the individual the choice of where on this private-public spectrum she is communicating. In addition we think there it is time to re-consider the lifespan of information: to give us, the users, the choice between a forms of communication that burn-on-read to  last-forever. 

As a step in this direction we believe there is a point in re-asserting the category of the “publication” or "the book" – meaning the creation of stable and clearly defined units of public information, something that can be uniquely referred to in public discourse independent of central authorities and big commercial interests.

We see the _block_ (the name we use for the published text unit) as existing on the extreme point of both the private/public and the temporary/permanent scale: a _block_ is public and permanent. 

## Proposal 

We propose a system consisting of three parts:

1. A decentralized catalogue
2. A decentralized file sharing system
3. A client application

Of course we do not want or need to construct the necessary foundations of the first two parts (not to mention that we would not be able to).

For the catalogue we make use of a simple _smart contract_ running on the [Ethereum] blockchain.

For the distribution of the actual content we are looking at the content-addressed, peer-to-peer file system [IPFS]. 

This allows us to focus on point three: the interface and the conceptualization and aesthetics of the _block_.   

### Decentralized catalogue

The core of the system is a decentralized catalogue preserving references to all _blocks_. Whereas previous solutions to the problem of persistent referability have relied on a central authority to issue certificates, b10.hk will use a transparent, autonomous authority system based on blockchain technology.

The specific technology that enables this is [Ethereum], a decentralized platform that runs smart contracts. Fundamentally it is a system, based on blockchain database technology, allowing agreement between nodes in a network without a central authority. The integrity of the system is maintained through the economically incentivized cryptographic labour of the participating machines. This is the operating system on top of which the core of b10.hk runs. Publishing is simply the operation of making an entry into this distributed, public database. The catalogue functions transparently, without human involvement.

In contrast to a [ISBN] or [DOI] number, a _yinn_ is directly tied to the information it identifies. By using a [cryptographic hashing function], a fingerprint of the information is created. Changing a single letter in the text will completely change the fingerprint. A modified file would therefore fail verification against the catalogue. This allows certainty that the text you are reading is indeed the exact text that was published.

### Decentralized storage

The core catalogue will only store a reference to the text. So how to get the actual text? There are a number of distributed storage systems under development. The one we are looking at using currently is [IPFS] – a file system working according similar principles as BitTorrent: by reading a file you become a point of distribution for other readers and you contribute to the preservation of the _block_.

##### Format

b10.hk is designed for publication of pure text.

Many electronic book formats (e.g. ePub) try to adapt the book/publication-concept to things that are not a good fit for it (interactivity, variable content, etc…) making it into a less good version of already existing forms (web-sites, games.) This seems pointless to us – 

We consider the 


code / literature / poetry

A connection to material metal typography – seeing the digital letters as having a certain "body"/volume, taking up a certain space.

That way we would get a strict grid where letters line up vertically allowing for a visual/aestethic pattern-making/layout. It would bring it a bit closer to code than to literature. That is something we think could be an interesting area: the meeting between code and literature/poetry.

aesthetic of the blockchain

A header containing metadata is added to the content, affecting the hash/fingerprint and therefore subject to the same tamper resistance as the main content. We will use a simple key-value system such as the one outlined in [MultiMarkdown], with a few standard (but not compulsory) keys and the possibility of adding your own.

### Client

In order for b10.hk to be useful the layer that meets the user needs to offer a unified, well-designed reading experience. It needs to bring attention to the underlying positives of the system without losing focus on the main thing: the text content. In line with the emphasis on the publication as a more self-contained unit of information, the design of the interface we envision will be distraction free – drawing on the tradition of book technology while being very aware of the context of screen based reading. Through the design of the experience we aim to draw a strong line between the private and the public – storing texts encrypted on the local device until published – making it clear to the user when this line is crossed. 

## Conclusion

With Google rebranding as Alphabet and working to organize the world from A to Z, there is an urgent need for other models of organisation of our collective memory, beyond giant data centers and walled gardens. We believe that recent developments offer opportunities for such new models. 

The current web is based on a business model of Spying on users, selling the information and advertisements.

## Terminology

Interface				---				b10.hk
Protocol				---				babel
Catalogue				---				babel 
Publication 			–––				block
Hash						---				yinn		
File						---				slab
Line						---				line
Column					---				spine 
Letter					---				grain

## References

	[DOI]: https://www.doi.org
	[Ethereum]: https://github.com/ethereum/wiki/wiki/White-Paper
	[cryptographic hashing function]: http://emn178.github.io/online-tools/sha3_256.html
	[IPFS]: http://ipfs.io/