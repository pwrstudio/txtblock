# PUBLICATION SYSTEM X
*Rasmus Svensson & Hanna Nilsson (PWR studio)*

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*
– [Julian Assange. Hans Ulrich Obrist In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011.]( http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/)

## Introduction

Adding Petabytes of data to the global data store every day.

Google rebranding as Alphabet, proposing to organize the information of the world. All the information.
privatization of words


## Background

What does the verb “to publish” mean in a time of hyper circulation? According to the dictionary “publishing” is either the business of producing books and magazines or – more broadly – the act of making something public and drawing attention to it. Whereas in the not so distant past this activity was a major enterprise requiring considerable resources it has for the last decade become an increasingly everyday activity. The technology needed for making something public is now omnipresent and the line between private and public is effectively blurred. While the action of printing, binding and distributing a book is an unmistakable step from the private to the public sphere. In contrast many current publishing tools exist in a grey zone in-between the two. Is “publishing” then a anachronistic term best left behind in the age of paper? We believe there is a point in re/asserting the category of the “publication” – a stable unit of information in contrast to the ephemeral flow.  

There is the problem of long-term addressability of information: Addresses change, servers fail, companies go out of business. Schemes such as [DOI] (Digital Object Identifier) or [PURL] (Persistent uniform resource locator) have been implemented to come to terms with this. Most of them have depended on central points of authority – as well as failing to provide an attractive way of conceptualizing and visualizing the core feature of permanence to the general public. 

In addition there is the problem of increasingly centralized control of the published information. Stored by a few major players, forming the core asset of their business model: A resource to be analysed and mined for commercial value.


## Proposal

We propose a decentralized platform for publishing and distribution of digital texts. Enable trustless persistent identification and digital robustness.

The criteria we set up for what constitutes a publication are:
- uniquely identifiable
- publicly available
- easily accessible  

Tp address these criteria we propose a system consisting of three parts
1. A decentralized index
2. A decentralized file sharing system
3. A client application

Where the (1) and (2) is a set of open standards (as far as possible existing such standards) and (3) is a interface for interacting (reading/publishing) with the underlying system.

X is designed for publication of pure text. This decision is made to position X in the historical lineage of the book. We believe it could in the future quite easily be extended to include other media or arbitrary data by adapting the client layer.

### Decentralized index

The core of the system is a decentralized index or catalogue preserving references to all publications. Where as previous solutions to the problem of persistent reparability have relied on a central authority to issue certificates, X will use a transparent, autonomous authority system.


##### Ethereum

The technology that enables this is [Ethereum], a decentralized platform that runs smart contracts. Fundamentally it is a system, based on blockchain database technology, enabling agreement beweeen nodes in a network without a central authority. The integrity of the system is maintained through the economically incentivized cryptographic labour of the participating machines. This is the operating system on top of which the core of X runs. The operation of publishing will require a small transaction fee (a one-time payment for the computing power needed to add the entry to the database.)


##### Tamperproof & Censorship proof 

In contrast to a ISBN or DOI identifier, a X identifier is tied to the information it indentifies. By using a [cryptographic hashing function] a fingerprint of the information is created. Changing a single letter in the information will completely change the fingerprint. A modified file would therefore fail verification against the catalogue. This allows a certainty that the text you are reading is indeed the exact text that was published – especially important as the actual file will be stored in a decentralized manner by all the participants of the network.

A X identifier could look as follows:
    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb


##### Timestamped

In addition to the identifier the catalogue will also store a timestamp of the moment of publication. In this way it can be proven that certain information was made public at a certain date, similar to how for example [OriginStamp] works on top of the bitcoin blockchain. 

##### Atomic addressability
It will also be possible to refer to parts of the document with a dot notation such as: 

    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb.5f8743
    
With the postfix being a offset from the start of the file.

Or to a range of text like so:
    
    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb.5f8743-a489b4


##### Format

As every bit of information is crucial in establishing the identity of a publication there needs to be a standardized way of formatting the text. X use the [Markdown] standard for saving information about basic formatting of the text (bold, italic, headline, block quotes, etc…) The actual visual styling of the text is left to the client software.

A header containing metadata is added to the content, affecting the hash/fingerprint and therefore subject to the same tamper resistance as the main content. We will use a simple key-value system such as the one outlined in [MultiMarkdown], with a few standard (but not obligatory) keys and the possibility of adding your own.

##### Pseudonymity

While an author can be specified in the metadata, this is not obligatory. This enables pseudonymous publication – to the extent that measures are taken to maintain this pseudonymity through all the layers of the system. On the other hand there would also be the option of connecting it to more authoritative personal identity systems by adding custom fields to the metadata header. 

### Decentralized storage

The core catalogue will only store a reference-fingerprint of the text. So how to store the actual text? Many solutions would be possible. Following the spirit of the project, a decentralized storage system would naturally be ideal. At this point there are a number of such solutions existing or under development:

- [Swarm]
- [IPFS]
- [StorJ]
- [BitTorrent]

We are looking at these strive to be compatible all of them, as well as centralized, local, storage. 

X will provide a linking schemes such as:

    X:3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb

In the end the information will need to pass verification of the catalogue, so the storage points do not have to be trusted, as long as redundancy is achived.

### Client

In order for X to be useful the layer that meets the user needs to be 

Bringin attention to the underlying positives of the system without losing focus on the main thing: the text content.
cross-platform: web, phone, and in the future deicated reader hardware.

Through the design of the experience of we aim to draw a clear line between the private and the public – storing  texts encrypted on the local device until published – making it quite clear when this line is crossed. 

Value in a unified, well designed reading experience.

With the area of dedicated digital reading being dominated by proprietery systems such as kindle and iBook.
Lack of good open alternatives with attractive implementations.

The client would just be one, holding no special authority other than being the first. The field is open to alternative clients functioning and looking in other ways.

## Conclusion

## References
[PURL]: https://sites.google.com/site/persistenturls/
[DOI]: https://www.doi.org
[Ethereum]: https://github.com/ethereum/wiki/wiki/White-Paper
[Markdown]: http://daringfireball.net/projects/markdown/
[MultiMarkdown]: http://fletcher.github.io/MultiMarkdown-4/metadata.html
[cryptographic hashing function]: http://emn178.github.io/online-tools/sha3_256.html
[IPFS]: http://ipfs.io/
[Swarm]: https://github.com/ethereum/go-ethereum/wiki/Swarm---distributed-preimage-archive
[StorJ]: http://storj.io/
[BitTorrent]: http://www.bittorrent.org/beps/bep_0005.html
[OriginStamp]: http://www.originstamp.org/