# PUBLICATION SYSTEM X
*Rasmus Svensson & Hanna Nilsson (PWR studio)*

## Introduction

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*

— Julian Assange. Hans Ulrich Obrist: In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011. http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/

Adding Petabytes of data to the global library everyday.

Google rebranding as Alphabet, proposing to organize the information of the world. All the information.
privatization of words

## Background

What does the verb “to publish” mean in a time of hyper circulation? According to the dictionary “publishing” is either the business of producing books and magazines or – more broadly – the act of making something public and drawing attention to it. Whereas in the not so distant past this activity was a major enterprise requiring considerable resources it has for the last decade become an increasingly everyday activity. The technology needed for making something public is now omnipresent and the line between private and public is effectively blurred. While the action of printing, binding and distribuing a book is an unmistakeable step from the private to the public sphere. In contrast many current publishing tools exist in a grey zone in-between. Is publishing then a anachronistic term best left behind in the age of paper?

There is the problem of long-term addressability of information: Address might change, servers go down, companies go out of business. Schemes such as DOI (Digital Object Identifier) or PURL (Persistent uniform resource locator) have been implemented to come to terms with this. 

In addition there is the problem of increasingly centralized ownership of the published information. Stored by a few major players, forming the core resource of their business model. A resource to be analysed and mined for commercial value.


## Proposal

We propose a decentralised platform for publishing and distribution of digital texts.



The criteria we set up for what constitutes a publication are:
- publicly available
- uniquely referrable

The system consists of three parts

1. A decentralised index
2. A decentralised file sharing system
3. A client application

Where the (1) and (2) is a set of open standards (as far as possible existing such standards) and (3) is a interface for interacting (reading \ publishing) to the underlying system.

Enable trustless persistent identification and digital robustness.


### Decentralised index

The core of the system is a decentralized index or catalogue

Where as previous solutions to the problem of persisten referability have relied on a central authority to issue certificates, X will use a transparent, autonomous authority.

##### Ethereum

The technology that enables this is Ethereum, a decentralized platform that runs smart contracts. Fundamentally it is a system, based on blockchain technology, enabling agreement beweeen nodes in a network without a central authority. The integrity of the system is maintained through the economically incentive zed cryptographic labour of XXXXX. 

small transaction fee (a one-time payment for the computing power needed to add the entry to the database.)


##### Tamperproof & Censorship proof 

In contrast to a ISBN or DOI identifier, a X indentifier is  
Forming a very strong link connecting the content to its reference.

By using a cryptographic hashing function a fingerprint is created. Changing a single letter in the file will completely change the fingerprint. A tampered/with file would therefore fail verification against the. This allows a certainty that the text you are reading is indeed the exact text that was published. 

A X identifier could look as follows:

    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb

##### Timestamped

Proving that a certain information was published at a certain time. Similar to for example Origincoin, that is built onto of the bitcoin blockchain.



##### Atomic referability
With the additional prossibility of referring to parts of the document with a notation such as: 

    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb:5f8743



### Decentralised storage

Identifier being resolved to multiple locations

- swarm
- ipfs
- bittorrent
- storage–agnostic

text-only:
simplicity
connecting with the historical lineage of the book
pure text (unicode) with markdown formatting + meta header 

##### Formatting

X use the Markdown standard for saving information about basic formatting of the text (bold, italic, headline, block quotes, etc…)

The actual styling of the text is left to the client software.

##### Metadata

A header containing metadata is added to the content, affecting the hash/fingerprint and therefore tamperproof. Saved as a json data-structure.

##### Anonymity

While an author can be specified in the metadata, this is not obligatory.
There would also be the option of connecting it to more authoritive personal identity systems by adding custom fields to the metadata header. 


### client

cross-platform: web, phone.

unified reading experience.

Lack of good alternatives for (kindel, iBook)
open standards such as ePub lacking attractive implementations.

similar to medium, filling a empty space in the ebook reader market

clear line between private and public (encrypted and stored locally until published)

The client would just be one, holding no special authrity other than being the first. The field is open to alternative clients…

## Conclusion

XXXXX

## References

https://github.com/ethereum/wiki/wiki/White-Paper

http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/

http://www.theindexer.org/files/18-1/18-1_025.pdf

https://sites.google.com/site/persistenturls/

http://www.editeur.org/files/Collaborations/Publications/ISO%20Focus%20April%202011%20-%20Stella%20Griffiths%20-%20ISBN%20Special%20Report.pdf

http://p-dpa.net

http://www.nist.gov/customcf/get_pdf.cfm?pub_id=919061

http://emn178.github.io/online-tools/sha3_512.html

http://www.proofofexistence.com/

http://www.originstamp.org/

http://daringfireball.net/projects/markdown/