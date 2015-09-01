# PUBLICATION SYSTEM X
*Rasmus Svensson & Hanna Nilsson (PWR studio)*

## Introduction

*”We need a way of consistently and accurately naming every piece of human knowledge, in such a way that their name arises out of the knowledge itself, out of its textual, visual, or aural representation, where the name is inextricably coupled to what it actually is. If we have that name, and if we use that name to refer to some information, and someone tries to change the contents, then it is either impossible or completely detectable by anyone using the name.”*

— Julian Assange. Hans Ulrich Obrist: In Conversation with Julian Assange, Part I, e-flux journal #25 . 05/2011. http://www.e-flux.com/journal/in-conversation-with-julian-assange-part-i/

Adding Petabytes of data to the global library everyday.

Google rebranding as Alphabet, proposing to organize the information of the world. All the information.
privatization of words



## Background

What does it mean to publish in a time of xxxxxx? According to the dictionary it is either the business of producing books and magazines or – more broadly – the act of making something public and drawing attention to it. Whereas in the not so distant past publishing was a major enterprise requiring considerable resources it has for the last decade become an increasingly everyday activity. The technology needed for making something public is now omnipresent and the line between private and public is effectively blurred. While the action of having printed, bound and distributed a book, for instance, is an unmistakeable step from the private to the public sphere. In contrast many current publishing tools exist in a grey zone in-between.

There is additionally the problem of conservation and ownership of the published information. Stored by a few major players, to be analysed and mined for commercial value. authority names

Address might change, servers go down, companies go out of business.

Adddressed by schemes such as DOI (Digital Object Identifier) or PURL (Persistent uniform resource locator), centralized system governance and management, payment, institutional backing, high barrier to entry, Registration Authority

ot reliant on any organization

published as an ISO standard where the actual document is not available without payment.

The criteria we set up for a publication are:

- publicly available
- uniquely referable


## Proposal

We propose a decentralised system for publishing and distribution of digital text – a sort of ISBN for digital publications. 

open standards

The system consists of three parts

1. A decentralised index
2. A decentralised file sharing system
3. A client application


### Decentralised index

persistent identification
first class entity
digital robustness
trustless

The core of the system, a sort of ISBN for digital publications.  

Notary function

smart contract

ethereum/blockchain
mechanism for trust


— tamperproof & censorship proof 
Whereas a ISBN number has no connection to the actual information contained in the book.

by using a SHA3 hashing function
fingerprint that will change if a single letter is replaced.

connecting the content to its reference.

For example:

    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb

With the additional prossibility of refering to parts of the document with a notation such as: 

    3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb:5f8743

— timestamped

Proving when something was published. Similar to for example Origincoin, that is built onto of the bitcoin blockchain.

small transaction fee (a one-time payment for the computing power needed to add the entry to the database.)

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

more popular files will be more widely 

But we might also 

### client

cross-platform: web, phone.

unified reading experience.

similar to medium, filling a empty space in the ebook reader market

clear line between private and public (encrypted and stored locally until published)

open to alternative clients…

### Additional considerations
— anonymity

publicly authored?


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