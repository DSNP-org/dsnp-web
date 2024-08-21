---
layout: post
title:  "The DSNP Difference--Federated Protocols Part 1"
author: Jeanette DePatie
blurb:  "DSNP Contributor and professional \"techsplainer\" Jeanette DePatie shares her thoughts the differences developers will experience between creating on DSNP versus other federated protocols."
--- 
DSNP Contributor and professional "techsplainer" Jeanette DePatie shares her thoughts the differences developers will experience between creating on DSNP versus other federated protocols.


###### How DSNP differs from AT Protocol and ActivityPub, and how DSNP can act as a bridge to create truly decentralized social.


As developers explore different protocols to underpin their social networking application efforts, it’s useful to note how the Decentralized Social Networking Protocol (DSNP) is different from others.  Of particular note are the AT Protocol (currently utilized in the Bluesky platform) and ActivityPub (currently utilized in federated social network applications like Mastodon).


##### AT Protocol

The Bluesky platform is a microblogging social network platform with very short form content like X (formerly known as Twitter).  It originated as an initiative within Twitter designed to create a decentralized social protocol.  Bluesky Social (incorporated as a public benefit corporation in 2021) was launched by Twitter co-founder Jack Dorsey and XMPP creator Jeremie Miller. Bluesky Social created AT Protocol to underpin the Bluesky platform.


##### ActivityPub

The ActivityPub protocol, which builds upon the Activity Streams 2.0 data format, provides a client to server API for creating, updating and deleting content and a federated server to server API for delivering notifications and content.  The ActivityPub protocol was published as a Recommendation to W3C by the Social Web Working Group in 2014.  This group last published official recommendations in 2018.  Since then, the Fediverse community has collaborated on improvements, such as those submitted as Fediverse Enhancement Proposals (FEPs). The ActivityPub protocol and a suite of related protocols and conventions is used by applications like Mastodon, Medium, Mozilla.social and Meta's Threads, among others.


##### DSNP

DSNP was designed to give users agency and control over their social identities and the connections that form their social network, enabling a secure, universally accessible social graph and facilitating open and trusted communication in public forums.  To facilitate these goals, it leverages the capabilities of public permissionless consensus systems. DSNP has an open, community-driven governance model, and is stewarded by the Project Liberty Institute and advised by a group of experts (including Dave Clark, Lawrence Lessig and Wendy Seltzer) with long and deep histories in Internet protocol and governance development.


##### Comparing the Protocols

While all three of these protocols are utilized and in some ways designed for social networking applications, there are important differences developers should consider before choosing among them as building blocks for their social networking applications.

##### Economic Viability
One of the main differences between DSNP and AT Protocol/ActivityPub is in the revenue models they can support.  Currently AT Protocol earns a small amount of revenue through services sold by Bluesky–starting with custom domains.  In addition Web Monetization federation via ActivityPub has been proposed as a W3C standard.   However, Activity Pub is largely dependent on donations via grass-roots efforts in order to stay afloat and incentivize developers and server operators.  This means that these protocols are dependent on the goodwill of the community they originally attracted in order to keep donations flowing in.  This may affect developers that use certain revenue models (e.g. ads, selling data) that are unpopular with donors. While federated protocols may not prevent these developers from using these models, it may control their visibility within the federated network–essentially stranding them on an island away from the rest of the system.  Thus, a donation strategy may not only limit the decisions developers on the platform may make, but may also prove untenable as a long term strategy as interest or passion in the protocols wane. While Bluesky generates some income via custom domain services, AT Protocol is largely dependent on Bluesky Social for funding.  Thus economic viability is largely dependent on this entity remaining successful and retaining interest in the AT Protocol profile.

While DSNP is also a 501(c)3-stewarded protocol with charitable donations covering advisor meetings and community communications, DSNP can support any number of revenue models for applications and network participants.  App developers may choose any monetization strategy they see fit so long as they clearly and transparently divulge this strategy to would-be users on the platform.  At the next level, DSNP end users may choose whatever app provider meets with their personal needs.  Thus monetization strategies are both presented and selected in a free-market system which may change to accommodate different market conditions and whatever end users are currently willing to support.


##### Decentralization

Another important difference in DSNP when compared to AT Protocol/ActivityPub is the level of decentralization.  Both AT Protocol and ActivityPub are federated systems.  These systems (often described as belonging to the "Fediverse") are composed of a set of servers that may operate with some level of independence from one another, and each individually owned and controlled server may have its own policies and rules. The protocol defines the way content and connections are shared between servers (although ActivityPub can be used both for client-to-server and server-to-server interactions, Mastodon uses it primarily for the latter type). Access to a user's account, social graph, and content is controlled by the individual server they join.  While in theory, a server should treat its users well, at the end of the day, it’s the server not the end user who has final control over the account.

DSNP enables a universal decentralized data plane where accounts, social graphs, and access to content is distributed throughout the system with replication of all important data across nodes via consensus mechanisms, and thus there is no single point of control or failure. This can make the system more resilient to data loss as well as less vulnerable to censorship (see below). Because nodes in the system operate under a shared set of rules, a DSNP system allows for system-wide governance–a process where all stakeholders (including developers and users) will have access to transparent information about how the system is run as well as some say in how the system is managed.  At the protocol level, the Project Liberty Institute serves as the initial steward of the DSNP specification, with an open governance model and plans to formalize how everyone within the community can contribute to the growth and governance of the protocol. 

A bridge built between DSNP and ActivityPub and AT Protocol could result in greater decentralization for these two federated systems.  DSNP could potentially offer greater data resilience and resistance to censorship.

##### Data Persistence

One key element of user ownership and agency over their social networking data is consistent and persistent access to that data.  If users lose access to their data due to network issues, account issues or because they are blocked from using a social networking application, they may lose access to their content and their social graph (i.e. the web of social connections they may have as friends or followers online).

AT Protocol, ActivityPub and DSNP each handle data persistence in a different way.  A core idea of ActivityPub is that since neither desktop systems nor mobile devices have a permanent connection to the internet, one needs an agent that does (i.e. a Mastodon instance).  ActivityPub hosts user posts under linkable URLs and notifies interested parties (i.e. the people following the content creator or thread) when and where new posts may be found.  A potential challenge with this model is that all of this data may be hosted in different places on the Internet that may or may not be available at any given time.  So unless a user hosts all of their own content on their own server, their content may become unavailable at any time either because a server shuts down or a moderator removes the user’s access (censorship).  And even if a content creator self-hosts, there is no guarantee they will have consistent access to the full content of their replies, posts or threads.

The AT Protocol handles this storage issue somewhat differently.  All the user’s data is stored in a Personal Data Server (PDS) that hosts a Personal Data Repository (PDR) which is bound to the user’s identity and contains all the user’s content (including comments).  The user may choose to host their own PDS at any time.  One issue that remains unclear is where the indexes of User IDs are stored.  Until the issue of User Identification indexing is definitively solved, AT Protocol users may lose connections with other users in their network and unless they are self-hosted, they may lose connections to their own content.

As a decentralized platform, DSNP ensures that users can retain control over their content or their social graph.  DSNP is run on independent nodes, each of which guarantees access to all critical data such as decentralized user identifiers, public keys, and social graphs. Any data that is not replicated among the DSNP nodes (such as content or media files) can be stored on distributed file systems such as the InterPlanetary File System (IPFS), a peer-to-peer network for storing and sharing data without relying on the continued availability and goodwill of a particular content host.  It is conceivable that connections built between DSNP, AT Protocol and ActivityPub could result in a hybrid system.  This hybrid system could afford greater data persistence and resilience than is currently enjoyed by either of the federated systems.


##### Censorship

Decentralization and data persistence each feed into whether a protocol makes users more or less vulnerable to censorship.  All three of the protocols discussed in this article allow users who face censorship with one application or server to elect to move to another application or server that uses the protocol.  However in practical terms this plays out differently in each case.  For example, users of applications on the AT Protocol may choose a server that is aligned with what the user feels is important or what they wish to express.  However, Bluesky (the only platform using the AT Protocol at present) does not make it easy for users to understand what the differences among the different servers are.  Users are given little information about which server to pick initially and little information about what server might suit them better if they are kicked off a server for violating the rules and sensibilities surrounding that server.  The situation is somewhat similar on many ActivityPub applications.  What’s more, since ActivityPub and AT Protocol face challenges around data persistence, users risk losing access to their content and connections (social graph) as they move from one server or provider to another.

DSNP users are less vulnerable to censorship, as the delegation model allows them to simply elect to share access to their data with any willing application provider.  Each of these providers is expected to provide clear instructions regarding their terms of service.  And should a user choose to leave one provider or application, the process of moving to another is quite simple.  As all important information the user needs to stay connected to their DSNP identity and relationships is stored among all nodes of the system, the user can move from one application to another without fear that their essential data will be lost.

Again, one could imagine a hybrid system appending the data persistence and ease by which users may move from one provider to another to the current AT Protocol and ActivityPub applications.  Bridging between federated and decentralized systems would likely be quite challenging.  However, there is a great deal to be gained by creating connecting tools that allow the greatest possible number of users to encounter the advantages DSNP has to offer.  

##### More to Come

These are just a few of the important differences between DSNP and other protocols like AT Protocol and ActivityPub.  Stay tuned for further articles with additional details regarding the advantages offered to developers by DSNP.

_Jeanette Depatie is a DSNP contributor and technical writer. The opinions expressed in this post are solely the author's and do not necessarily express the views or opinions of Project Liberty Institute._
