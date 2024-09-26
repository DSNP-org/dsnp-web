---
layout: post
title: "Announcing the release of DSNP 1.3"
author: Wes Biggs
tags: spec
blurb: DSNP 1.3 brings exciting new features and streamlined functionality for key social primitives.
---

The DSNP community has completed work on the next update to the protocol specification, and version 1.3.0 has been published to [the specification website](https://spec.dsnp.org).
This new release contains several enhancements and new features, summarized below.

#### Bringing out our best attributes

DSNP 1.3 brings the concept of verifiable [attribute sets](https://spec.dsnp.org/DSNP/AttributeSets.html) to the protocol, and defines how they can be used in a variety of different contexts. Attribute sets are structured data describing someone or something. By establishing a framework for defining and using shared data schemas for attribute sets, DSNP enables the community of applications to collaborate on building a rich language of metadata about users, posts, and more. The specification adds [three new types of announcements](https://spec.dsnp.org/DSNP/Announcements.html), allowing verifiable attributes relevant to DSNP users, DSNP content, and external content. Use cases for attribute sets include verified user badges, display of professional accreditations, content provenance, community content tagging and much more. Higher level concepts, such as application-independent content moderation systems and reputation scoring services, become possible with these foundations.

To represent the notion of attested, verifiable attribute sets, DSNP 1.3 adds a [new sub-specification](https://spec.dsnp.org/VerifiableCredentials/Overview.html) detailing interoperability with the W3C Verifiable Credentials body of standards. Attribute sets and attestation take the form of Verifiable Credentials, aligning with important work within the W3C standards process.

#### Keys are key

Public key encryption and signatures are core to DSNP's concept of user agency and data security.
Core enough, in fact, that the specification now mandates that a user's public keys must be directly retrievable as [user data](https://spec.dsnp.org/DSNP/UserData.html#user-data-types) from the consensus system, instead of being announced as part of a user's content stream. This enables [social graph](https://spec.dsnp.org/DSNP/Graph.html) encryption, [pseudonymous relationship identifier](https://spec.dsnp.org/DSNP/Graph.html#pseudonymous-relationship-identifiers) generation, and verification of credentials to occur without the need for external indexing or data caching. This also allows DSNP to specify standard [Decentralized Identifier (DID)](https://spec.dsnp.org/VerifiableCredentials/Types/DID.html) documents, enabling paradigmatic access to a user's public keys in accordance with the W3C recommendation. The "key agreement" key type is used for social graph encryption and relationship discovery, and the "assertion method" key type is used for issuers of verifiable credentials.

#### Higher-profile profiles

A great deal of community discussion went into DSNP 1.3 in Zoom meetings, github discussions, and more. An important change that emerged from that process is DSNP 1.3's concept of [profile resources](https://spec.dsnp.org/DSNP/Types/ProfileResource.html), an extensible mechanism for storing and retrieving user profile information. In previous versions, users announced new and updated profile documents through the content stream. This had the disadvantage of requiring applications to maintain an index of the full history of the profile content stream in order to locate and display a particular user's profile. The profile resource type moves the linkage to profile documents to the consensus system proper, recognizing the critical role that profile information plays in allowing users to find and discover each other. Combined with the ability to [attach attestations](https://spec.dsnp.org/DSNP/AttributeSets.html#attestation-attachments) to a user profile, this means users can display badges and other verified attributes on their profiles, and know that these can easily be discovered by ecosystem applications and services.

#### Hashing it out

Digest values from hashing algorithms secure and anchor chains of DSNP-related data, ensuring the authenticity of announced content, attribute sets, media attachments, and more. DSNP 1.3 recognizes the importance of these [hashes](https://spec.dsnp.org/DSNP/Identifiers.html#dsnp-content-hash) and aims to make development of DSNP-compliant applications and services simpler by more precisely defining the allowed algorithms (SHA-256 and Blake3), encoding (multihash), and serialization (base32 multibase strings) of hashes. By ensuring consistent usage throughout the specification, developers can focus less on transforming hashes between different representations, and leverage reusable components and libraries across a variety of DSNP-related use cases.

#### Next steps

The summaries above focus on new and updated affordances provided in the latest version of the specification. For more details and links to related discussions, see the [github release notes](https://github.com/LibertyDSNP/spec/releases/tag/DSNP-v1.3.0). In the coming weeks this blog will explore some of the possible use cases and applications of these toward building a vibrant and thriving DSNP ecosystem. Your contributions are welcome and encouraged, too, whether that means starting a discussion on the [Project Liberty forums](https://forums.projectliberty.io/), submitting your own post for this blog, or simply airing your opinion on the [monthly community call](https://vimeo.com/showcase/dsnp-public-spec-meeting).

_Wes Biggs is a principal software architect at Project Liberty Labs and a maintainer of the DSNP specification._
