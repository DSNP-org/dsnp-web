---
layout: post
title: Tiers of Data
author: Wil Wade
tags: design
blurb: Different classes of data are part of what make DSNP both possible and flexible.
---

DSNP makes use of a three tier data storage architecture.
While implementations may slightly differ on how or why data is stored at a different tier, the general structure is still the same.
As we go through each tier, levels of security, availability, and cost change.

#### Tier 0: The Consensus System

At the consensus system level we have the highest security and availability levels for data.
Data is replicated and stored on each node of the network, meaning that as long as the system as a whole remains uncompromised and sufficiently decentralized, strong consistency and durability guarantees apply.
The trade-off is that the cost to store data at this layer is the highest as well.
At this tier, we place items that have the greatest consequences if lost: Identifiers, permissions, the social graph to be shared among applications, and references to the next tier of data.

#### Tier 1: Batch Publications

[Batch files](https://forums.projectliberty.io/t/04-batching-source-dependent-messages-with-delegation/216) form the next tier of data. While the data is stored outside the consensus system itself, the integrity of Batch files is ensured by using Tier 0 metadata.
We can connect the contents of the Batch file back to the consensus system.
A hash of the file allows users to know if the Batch file they retrieve is authentic, no matter the source.
The consensus system also records who announced the new Batch.
While the announcer could be unknown to the consuming application, [delegation](https://forums.projectliberty.io/t/03-wherefore-art-thou-delegation/213) allows some level of user-enforced reputation.
Users are remarkably good at avoiding unreliable services.

Reputation alone may be enough to maintain batch file availability, but availability is also incentivized through diversity.
Batch files are expected to usually contain references to content from a mixture of users (at least for higher volume services).
As each individual user shares the desire (and perhaps contractual obligation from the provider) that the content remains available, the service provider publishing the Batch file has a good reason to keep the file available, even if some portion of those users leave the service.
A final availability safeguard is the use of a content-addressable file system like [IPFS](https://ipfs.io/) for Batch files. IPFS is a distributed file store and allows anyone to persist data that can be retrieved from anywhere in the network.
DSNP requires IPFS or other distributed file stores to be used for batch files.

Even with all of these various safeguards, if a batch were to fall through the cracks, the system as a whole would continue functioning.
Applications using DSNP would know that data is missing (and which provider failed their responsibility to maintain availability), but it would at least have a limited impact on the future.
Implementing systems may also investigate ways to incentivise long-term storage replication or archiving of batches.

#### Tier 2: External Content References

While Batches are stored outside the consensus system itself, they contain some level of network information that is needed for the network to function fully.
The final tier of data consists of content like posts, replies, and user profiles, and is found using the URL or URI (Uniform Resource Identifier, of which URLs are a subset) along with a verifiable hash of the content.
While we often have a chain of hashes that secure the authenticity of the retrieved information, data _availability_ is the responsibility of the user that desires others to access it.
A user typically outsources the responsibility for data availability to a service provider, which often will be the same as the provider that announces the Batch referencing the content.

DSNP can assist in communicating the intent to delete ([tombstone](https://spec.dsnp.org/DSNP/Types/Tombstone)) or notify others that the storage location or content is [updated](https://spec.dsnp.org/DSNP/Types/Update), but responsibility and control over storage is ultimately in the hands of the announcing user and their agents.

#### Mix and Match

In several places above you can see how DSNP divides data and metadata between several tiers.
This is an intentional pattern.
Metadata falls into three categories: who is trying to send the messages, how to know it is authentic, and where to find it.
By securing the more important information at a more secure tier, information stored at lower tiers with lower cost can still have a high level of authenticity: the chain of metadata provides a proof of (former) existence even if that data is not currently retrievable.

In the end, the goal is transparency and authenticity with options for cost and storage.
Different types of data have different needs, and DSNP is designed to flexibly meet those different needs.
As technologies grow and change, DSNP systems should be able to grow and change with it.
