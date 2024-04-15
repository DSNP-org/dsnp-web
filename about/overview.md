---
layout: default
title: DSNP Overview
---
## Overview

DSNP stands for Decentralized Social Networking Protocol, which is an open protocol and potential standard for social networking and social media. It is not owned or controlled by any one person or company, allowing anyone to build on it or use it.

## 10 High-Level DSNP Concepts

1. Users are given a numeric ID known as their DSNP User Id which may or may not be linked to or associated with their real-world identity.
2. User data is managed and secured via a set of control keys typically connected in a public/private key pair.  The control keys are owned and managed solely by the user.
3. DSNP is designed to run on a consensus-based system such as a blockchain. This allows the system to be truly decentralized—meaning that users, not system operators, have control and agency over their data, and changes to the state of the system are public and immutable. 
4. DSNP users can delegate tasks such as managing social connections or submitting posts and content to the applications they use. This means that tasks that require specialized technical knowledge or have associated costs can be performed by service providers acting under the user's explicit agreement (which the user may revoke at any time).
5. User-generated content is handled via Announcements–public or private declarations or directions published to the system.
6. Updates or changes to the system are expressed as State Change Records–the observable output of a DSNP system.
7. Part of the data stored by each user is their social graph, which contains information about all the public and private relationships between the user and others in the system.
8. DSNP is designed to allow users to easily and seamlessly access their social graph and other user-centric data with any compatible application—user data and content is not just portable between applications, but fully interoperable.
9. Applications and service providers (those to whom tasks are delegated) compete in an open marketplace for users.  This allows users to choose the applications and providers who best serve their needs, and grant or revoke delegations at any time.
10. Applications and service providers collect and send Announcements in batches, reducing operational cost and enhancing scalability.

## What is a DSNP System?

A DSNP system is a (1) state machine that generates an (2) ongoing, (3) publicly observable and (4) verifiable (5) stream of state change records in response to (6) authenticated public input.  To take each of these terms one by one:



1. State Machine: The system maintains a consistent, deterministic set of data (state) in response to protocol communications.
2. Ongoing: The system runs continually.
3. Publicly Observable: System activities are transparent and may be openly viewed by developers, creators and users.
4. Verifiable: The authenticity of those sending messages is recorded and can be verified.   While these identities may remain pseudonymous, and the real world identity of the user may not be revealed, each account’s activity can be verified to come only from that account.
5. Stream of State Change Records: The system produces a continuous log of all changes that occur, such as account Id creation, messages sent, delegation, and so forth.
6. Authenticated Public Input: Refers to the open, decentralized nature of DSNP applications, which ensures that users have control and agency over their data.

In social networking terms, one can think of a DSNP system as one that continuously records everything that happens, including the identities of the participants (identity), the relationships they declare to other participants, the messages they send, when they are sent, and who they are for. This is true whether or not that participant is sending data themselves or delegating that task to someone else to do it on their behalf.  A DSNP system does its recordkeeping in public, even if some of the data it manages may be private (encrypted).


## DSNP Operations

Required DSNP Operations include Create Identifier, Retire Identifier, Define Delegation, Revoke Delegation, Add Control Key, Remove Control Key, Publish Announcement, Publish Batch, Get User Data and Replace User Data.

In order to be compliant, DSNP systems MUST:



1. **Make available all the operations defined by the DSNP specification.**
2. **Comply with DSNP dictates for operations**.  These include the data structures that will be provided as input, generated as output and saved as a state change record.
3. **Verify approval of the Acting Principal**. This means the user, provider or application requesting an action must be verified via a Control Key Ownership Proof as authorized to perform that action.
4. **Maintain unique Transaction Identifiers**. DSNP operations may be asynchronous, meaning that the system may not immediately generate output for a transaction. In fact, a state change record can appear any time after the operation occurs, and many transactions may be processed in parallel. Thus, each invocation of a DSNP Operation should have an associated unique Transaction Identifier that can be serialized as part of a string and correlated with the output of the system.
5. **Be publicly visible.** In order to know that the system is processing data as requested by users at all times, it must do this work in the open. In practical terms, this means that all DSNP users can exist (at least conceptually) within a shared social graph and all users have the ability to see and participate in public social discourse.  
6. **Ensure decentralization**. DSNP systems must have multiple nodes (i.e. servers) and not allow any single entity (like a popular social media service) to concentrate power or override its consensus mechanisms.  Thus a DSNP system must be run on top of a consensus system (like a blockchain).
7. **Specify implementation details.** DSNP systems must specify how applications interact with them across each possible Operation and State Change Record. This includes how the operations may be discovered, authenticated and executed, and how inputs and outputs will be serialized.


## What are the three main models within a DSNP system?

The three models within a DSNP system are the identity model (which records who is participating), the content model (which manages how the participants are communicating with one another) and graph (which stores all the relationships among the participants).


### The Identity Model

DSNP implementations must allow users to have a pseudonymous yet verifiable social identity.  Control over this identity means that a user may create, update or delete content associated with their identifier, delegate certain activities to be done on their behalf, manage the keys associated with their identifier, and, if they so choose, retire the identifier.  These identifiers must be unique and must have distinct control keys. 


### The Content Model

Social media within a DSNP system is sent as Announcements which link to content made available to the network.  Each announcement is associated with an identifier which can be validated to prove who created the Announcement.  These Announcements are typically included in Batch Publication Files.

### The Graph Model

DSNP enables a social graph, meaning a graph that represents social relationships among all the involved entities.  Users are represented within the graph by nodes uniquely identified by their DSNP User Ids.  The relationships between users are called graph edges.  The graph edges that originate from a user are stored as DSNP User Data.  This data captures three distinct sets of relationships: public follows (a one-way relationship where one user follows the public speech of another user), private follows (the same as a public follow except that this relationship is not visible to the one being followed or anyone else that doesn’t have the decryption key) and private connections (half of a two-way relationship between DSNP users that is visible only to the two parties in the relationship). To facilitate data privacy, DSNP lets user share public keys that can be used to securely store data and communicate with each other.
