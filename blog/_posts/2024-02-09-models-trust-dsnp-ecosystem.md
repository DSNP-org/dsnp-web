---
layout: post
title: Models of Trust in the DSNP Ecosystem
author: Wil Wade
tags: design
blurb: Society is built on trust. Each economic and social relationship forming society requires some trust to carry out the relationship, even if temporary. Sometimes this trust is simple, such as a simple interaction with a cashier in a store. Other times it is complex and multi-layered like a marriage.
---

Society is built on trust. Each economic and social relationship forming society requires some trust to carry out the relationship, even if temporary. Sometimes this trust is simple, such as a simple interaction with a cashier in a store. Other times it is complex and multi-layered like a marriage.

Social networking systems also use different forms of trust for their protocols and user interactions. Each has a set of trade-offs that lead to different social structures, benefits, and drawbacks in different situations and environments. These tradeoffs are critical for understanding the purpose and goals of each social networking system, but also the needs and priorities of those promoting or adopting the system.

#### Types of Trust

We’ll go through many of the types of trust as they apply to the technical ecosystem of a social network, but this should not be considered complete nor precise in the details. Most systems are built on a web of many different trust models, and in the best scenario that web reinforces the trust and optimization across the network.

##### Centralized Trust

The most common form of trust in social networking today is the centralized one-to-many trust relationship. This trust is one directional. Alice and Bob trust Company Z, but Company Z need not trust Alice or Bob. However, given that Alice trusts Company Z, if Company Z says something about or supposedly from Bob, Alice must trust that this statement really came from Bob (and hasn't been modified or censored). This is centralized social. Users must trust that Facebook, X/Twitter, and others faithfully represent the communication presented to them. A modified, and somewhat less adversarial, version of this trust is the trust in a centralized party that has aligned incentives, such as a community or standards organization.


##### Zero Trust

On the other end of the spectrum of trust, “Zero” Trust is the philosophy of many blockchains. Users should trust each other, and the systems that form the network, as little as possible, and each individual actor is viewed antagonistically. "Zero" trust is something of a misnomer, though — in the case of blockchain, the trust is in the consensus mechanism of the network. In Bitcoin, users trust that 50% + 1 of the miners will act honestly (and there are various ways they are encouraged to do so). This trust in a large disinterested collective comes with high cost and scale requirements.


##### Economic Trust

Commerce happens thanks to trust in exchanges of value. If two parties agree to an exchange, that exchange is likely to happen to the benefit of both parties. This is the other side of Blockchain trust. The economics of Bitcoin mean that miners are incentivized to perform actions for a user because of the fees paid. Economic Trust can be extended with details such as contracts.


##### Community Trust

Unlike the trust in a disinterested collective like “Zero” Trust, Community Trust is that of interested individuals. Trust is built on commonality of location or purpose. These are neighbors or online groups. They often can self-moderate and set their own norms. While this can and does lead to issues when the localized norms are in conflict with the norms of society, the vast majority of the time it works. This is the power of self-organizing, and relies on the work of individuals in a group to maintain this trust that otherwise degrades over time.


##### Relationship or Individual Trust

Trust between two individual parties is a trust built over time in small ways. It is slow to build and quick to be torn down. Each small step matters. This blossoms into amazing trust of friends and family. An example of translating Relationship trust into the digital world is the work of Filecoin for retrieval. Simplifying some of the details, the payment for transferring a file is confirmed incrementally as more and more of the file is transferred and confirmed to be available from a storage provider. Tracking each chunk of data allows for a slow buildup of trust while limiting financial exposure.


##### Transitive Trust

Transitive trust is perhaps the most common and hidden form of trust on the Internet. Also referred to as a web of trust, this model enables the extension of trust from an individual to a second order relationship. _A_ trusts _B_ who trusts _C_. _A_ can thus trust _C_. While not always true in personal relationships, the SSL certificate model uses this form of trust. While a user may not trust a random website for security, trust in the vetting processes and security of a set of core internet certificate signers allows a certificate chain to reach to the vast majority of the internet now.


##### Reputational Trust

While this was historically just a part of the Community Trust paradigm, the internet has enabled larger communities and connections between otherwise unconnected individuals. To enable a global online marketplace, Ebay pioneered the use of reputation to enable peer-to-peer commerce at a scale previously unimaginable. Amazon applied the same structure to product reviews. Although both of these examples have either been replaced with Centralized Trust or are under attack from false reports, the reputation tool is a way to take Relationship Trust and quantify it for digital interactions across relationships.


##### Social Trust

Social trust is sometimes referred to as blind trust, but it is really the trust that humans have with other humans within their society. This is what Ebay started with to create Reputation Trust. Society works because most individuals are trustworthy to a certain point, based on norms of behavior that have evolved over millennia. A great example of this is how trust is easier to give when the liability of a breach of a trust is low.


#### Trust Models in Social Networking Systems

Each social network system has a foundation of one or more of these forms of trust.


##### Centralized Social

As the term suggests, the primary reliance is on Centralized Trust. The current system has a flaw that the system contains a network effect lock-in. The lock-in creates a situation where the Centralized Trust is lost, but due to Social and Community Trust, the system remains in a degraded state. A single point of trust failure, but benefits from the economies of scale and cost.


##### Federated Social

Federated networks place limits on the Centralized Trust required by allowing users to choose the centralized trust of their choice without respect to the choice of other users. It increases the need for Community Trust, yet creates a larger individual point of trust failure and a [power law distribution](https://en.wikipedia.org/wiki/Power_law) of trust for each federated provider.

The application of federated ideas to individuals running pods or nodes in a federated network reduces the single point of failure for the whole, but increases the responsibility and cost for the individual user. The network may not have a single point of failure, but the individual still does.


##### Blockchain Social

Blockchain social networks use the Zero Trust model. It instead imposes a direct cost and a loss of Social Trust with the injection of monetary value or necessity of each post invoking Economic Trust. The failure shifts away from a single point of trust failure to the general erosion of social trust.


##### DSNP Social

DSNP tries to balance the two sides of the tradeoff. How can we limit the single point of failure and the impact of a breach of trust, while still maintaining social trust and the efficiencies of scale?

The DSNP model is a layered approach:



1. Lower Centralized Trust by utilizing Zero Trust for identity and graph.
2. Leverage Reputation Trust with user choice of applications that handle many of the user tasks and the availability of content.
3. Limit Economic Trust to the underlying infrastructure instead of exposing users to damage that can cause to Social Trust.
4. Leverage Community Trust to grow Social Trust by enabling the building of applications for the vast diversity of users.

This model leads to the use of blockchain or other consensus systems for identity, graph, and the announcement of content. It then enables user choice for hosting and availability of actual content, and ensures that the user has the ability to change providers at any time without losing control of their data. And it allows for applications and experiences to differentiate and compete based on their focus, functionality, and trustworthiness using a centralized model.

This blending of trust and careful choice of what trust models to leverage in each situation builds a new foundation for social networking that works for humans and society.

_Wil Wade is the director of blockchain engineering at Amplica Labs and one of the co-authors of the [DSNP Whitepaper](https://dsnp.org/dsnp_whitepaper.pdf)._
