---
layout: post
title:  "The DSNP Difference--Federated Protocols Part 2"
author: Jeanette DePatie, DSNP Contributor
blurb: DSNP Contributor and professional "techsplainer" Jeanette DePatie shares her thoughts in this second in a series of articles about the differences developers will experience between creating on DSNP versus other federated protocols.
--- 
DSNP Contributor and professional "techsplainer" Jeanette DePatie shares her thoughts in this second in a series of articles about the differences developers will experience between creating on DSNP versus other federated protocols.


###### Second in a series of articles about how DSNP differs from AT Protocol and ActivityPub, and how DSNP can act as a bridge to create truly decentralized social.


In part one of this series, we discussed several of the important advantages DSNP offers over other protocols (namely AT Protocol and ActivityPub).  Some of those key advantages included greater economic viability and freedom of choice for developers on the platform, greater decentralization as opposed to a federated model, data persistence where developers and users can feel confident that data won’t be lost and less vulnerability to censorship at the protocol level.

In this article, we will discuss a few additional important differences between DSNP and other protocols like AT Protocol and ActivityPub.



##### Discoverability

One challenge for developers using ActivityPub and AT Protocol is the lack of discoverability across servers.  Since ActivityPub and AT Protocol use federated P2P technology, they don’t provide for unified public spaces with global search capabilities where users can find new apps, new content, or one another.  This can present an area of risk for developers using these protocols, as there is no guarantee that users will be able to find the applications they have built or the content posted there.  Additionally, this may open the door to developers facing gatekeepers that could restrict their development and content choices–as leaving them out of the search index would be equivalent to isolating their apps to a deserted island.

DSNP developers can rest assured that users will be able to find and access apps and their data.  All public activity is replicated in every node, thus there is no place for gatekeepers to arbitrarily lock out nodes or developers.  Building hybrid solutions with DSNP and other protocols could help improve discoverability and reduce the risk that developers will find themselves stranded outside the search index. 



##### Identity

ActivityPub handles universal identity through a decentralized social networking protocol that uses ActivityStreams vocabulary.  Each user in the ActivityPub network is represented as an "actor" with a unique profile that includes various elements like inbox, outbox, followers, following, and a unique id URL that serves as a globally unique identifier for the user within the network.  However, one challenge in user verification on ActivityPub-based platforms is the absence of a cross-server directory. This can make it difficult for users to find and follow people across different servers. Additionally, there is currently no standardized tool or mechanism in widespread use for confirming the authenticity of an account.

Alternatively, the AT Protocol uses two interrelated forms of identifiers: the handle and the DID.  AT Protocol handles are DNS names.  For DIDs, AT Protocol supports did-web and a temporary method called DID Placeholder for global identification management. While AT Protocol has committed to supporting this placeholder until a better method is found, developers will likely soon be faced with the challenge of upgrading to the new DID system.

DSNP has fully developed and detailed mechanisms for handling universal identity across DSNP applications.  DSNP applications must allow users to create pseudonymous identifiers (although users can use their real name if they wish).  Users choose a handle which is then paired with a number in the application to create the user's universal handle.  Verification of the user’s identity is managed via a cryptographic key pair–ensuring that content issued by a particular user comes from them and no-one else.  The process of tying a user handle to a real world identity is outlined via a process currently proposed for DSNP called Attributes and Attestation, which will be outlined in a future article.  With the right bridges in place, DSNP could also potentially be used in concert with other protocols like ActivityPub and AT Protocol to bring verifiable pseudonymous identity to a hybrid system.



##### Portability

The ability to move one’s identity from one application to another (as discussed above) is just one aspect of portability.  Decentralized systems also aim to allow users to move content and their social graph (the web of relationships with others on the system) from one application to another.

AT Protocol offers some ability to migrate data from one host server to another via signed data repositories and DIDs.  However, the extent to which this data is portable depends on the implementation of the AT Protocol by individual applications, and the compatibility between them.  ActivityPub offers even more constrained portability as it requires the original server to provide a redirect to the new location as well as the new server to allow the transfer.  Should an old server go down, it would be unable to offer the required redirect.  And if the account is banned or the server to which they are migrating is defederated, then migration would be impossible.  Thus the only way to truly ensure content stability is for a user to run their own server (which requires a certain degree of technical aptitude).  Other challenges to portability in ActivityPub include the lack of a standard backup format for certain types of content and the possibility of incomplete data transfer during the move from one server to another.

With DSNP all key data is stored in all nodes of the system.  Thus, there is no need to “transfer” data from one place to another and risk loss of data in the transfer.  The user may take their social graph with them from one application to another without worries about compatibility or redirects.  The user needn’t bother running their own node (although they may if they wish to) as the multi-node structure functions as a de-facto backup of their key data.  In any case, the data remains persistent without reference to a particular application or server host.  Perhaps in the future, DSNP's universal identifiers could provide risk-free mechanisms for users of other protocols to transfer their identities and social graph.



##### Privacy and Security 

Another key differentiator between DSNP and other protocols lies in data security and privacy. 
In ActivityPub, the security of the system is largely dependent on how it’s implemented by various applications.  For example, ActivityPub as experienced by Mastodon users can make no promises around system-wide privacy and thus must trust that servers are not bad actors.  This puts much of the responsibility for security on the individual server administrators.  In addition, ensuring secure communications among servers can be challenging, involving not only securing the data while in transit but also verifying the identities of the communicating parties.  While the AT Protocol specifies that digital identifiers (DIDs) may be authenticated via rotating cryptographic keys, at this time, AT Protocol as implemented in Bluesky utilizes a simple email certification to determine account authenticity.  Additionally, while AT Protocol specifies that private messages and accounts may be available in the future, its current Bluesky implementation does not allow for DMs or other private communication.

DSNP offers publicly provable data encryption to secure user data and maintain privacy (particularly via blockchain).  DSNP systems allow users to choose a pseudonymous handle, and users can decide what other information to include in their descriptive profile or via the use of verified attributes. Any private user data stored in DSNP is encrypted using cryptographically strong public/private key technology.


##### Scalability
Scalability is likely to be one of the largest issues ActivityPub will face as scaling the network requires ever-increasing computing resources to interact with fragmentation and large instances.  ActivityPub’s inherent requirement for replicated content could greatly increase the costs for running the massive servers required to meet demand.  In short, ActivityPub can be server-load intensive.  AT Protocol is less resource intensive as it splits its functions across two types of servers: Personal Data Servers (PDSs), lightweight servers which house user accounts, and crawlers, which access data from various accounts and PDSs and aggregate it for end users.  However, one significant challenge to scalability at present is that at the moment, AT Protocol is only effectively used by Bluesky, and has not had to deal with the challenges of working with a more decentralized network architecture.  The only way that the true decentralized advantages of AT Protocol can be realized is if a significant number of other applications or service providers join the AT Protocol bandwagon.

DSNP has been designed from the ground up to be massively scalable.  Firstly, DSNP allows users to delegate their tasks to providers who may in turn gather many transactions together and send them in batches.  This drastically cuts down on costs, while allowing applications to listen to announcements and implement their own strategies for replicating and indexing content.



##### Conclusions

Decentralized and federated social media protocols have attracted significant interest and rapid advancement.  While AT Protocol, ActivityPub and DSNP may be among the most popular of these formats, new ones are being developed all the time.  Each decentralized or federated social media protocol has advantages and disadvantages for hosts, developers and users.  The spirit of decentralization points to a future which doesn’t split the world into winners and losers, but rather, seeks to find common ground and opportunity in collaboration.  Thus it should be of significant interest to all stakeholders to find a way to work together and learn from one another to work towards a future that creates a better, and more empowering, social networking future for all.



##### Note from the Author
The opinions expressed in this post are solely my own and do not necessarily express the views or opinions of Project Liberty.

---

