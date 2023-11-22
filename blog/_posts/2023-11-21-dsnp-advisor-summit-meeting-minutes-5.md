---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2023-10-25"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
October 25, 2023<br>
Emerge212, 1185 Avenue of the America, New York</p>

**Agenda:**

1. Introductions, logistics, and updates from Project Liberty
2. Ecosystem goals and vision
3. Governance update
4. Technical scope of DSNP
5. Community-based social identity
6. Ethical framework

**Attendees:**

- Erik Suhonen (ES), Project Liberty
- Wes Biggs (WB), Project Liberty
- Jeb Bell (JB), Project Liberty
- Paul Fehlinger (PF), Project Liberty
- Harry Evans (HE), Amplica Labs
- Braxton Woodham (BW), Amplica Labs
- Denise Duncan (DD), Amplica Labs
- Dave Clark (DC), DSNP Advisor
- Deb Roy (DR), DSNP Advisor
- Wendy Seltzer (WS), DSNP Advisor
- Sara Wedeman (SW), DSNP Advisor
- Larry Lessig (LL), DSNP Advisor
- Wes Chow (WC), DSNP Advisor Team
- Maggie Little (ML), Georgetown University Ethics Lab
- Jonathan Healy (JH), Georgetown University Ethics Lab

**Meeting Summary:**

Introduction and status updates

- The meeting was called to order at 9:00am by ES followed by a round of introductions. LL was welcomed as a new DSNP Advisor.
- The group agreed that the next meeting would be held on December 8, 2023, at the MIT Media Lab. A further date was set for the subsequent meeting, to be held January 23, 2024 in the Cambridge, MA area, with Harvard suggested as a location to be confirmed.
- ES discussed recent work at Project Liberty including details of the "Building Our Digital Futures" event and workshops organized by Project Liberty being held that afternoon.
- ES noted the developing academic partnerships with MIT, Harvard, Stanford, Georgetown and Sciences Po, and that experts within these universities would be working with PL to incorporate DSNP into their research and technology R&D efforts.
- ES described proof of concept work in progress between Project Liberty and FIDE to combine DSNP and the Beckn protocol for decentralized e-commerce around an initial use case based on verified purchaser product reviews.
- With regard to standardization goals, ES shared that PL had a DSNP-based report approved by the United Nations International Telecommunication Union (ITU) Focus Group. As next steps, PL will participate in the Final Focus Group meeting before this contribution hits the Telecommunication Standardization Advisory Group (TSAG). He noted that PL was considering if and how to replicate this work with W3C and ISO.
- ES noted that PL was in the process of resourcing additional staff to work on DSNP.

Ecosystem goals and vision

- ES shared the vision statement developed for the tech ecosystem: "Give people ownership and control of their personal data while expanding their economic opportunities through Project Liberty’s tech and ecosystem," as well as long-term and short-term objectives:
  - Long term objectives
    - Move 1 billion users to DSNP, with positive impact on those users
    - Create a mission-aligned and active tech ecosystem
  - Priorities by December 2024
    - Launch real-world proof points demonstrating DSNP’s positive impact and utility
    - Announce strategic tech partnership (e.g., social commerce)
    - Showcase the identity/single sign-on use case 
    - Demonstrate the interoperability use case 
    - Expand economic opportunities for users, developers and ecosystem participants
    - Make DSNP a global standard
    - Build a healthy, vibrant tech community
    - Initiate community governance for DSNP

Governance updates and next steps

- JB was introduced as the current head of research at PL who would be taking the lead in governance facilitation. He noted an opportunity to combine an evidence-based research approach with DSNP.
- JB commented that he sees DSNP as a proof point for responsible technological innovation, and asked how he could best serve the needs of the advisor group. He shared his background and professional experience, and emphasized the importance of the user experience in expressing transparency and accountability. He noted a goal of encouraging increased data sharing in privacy-preserving ways, so that pseudonymous data from the DSNP ecosystem could be available for evaluation by third parties.
- DD noted that in its formative phase, Project Liberty had developed bedrock principles which set the atmosphere and environment for the project and company, but that these were not action-guiding in a practical sense.
- WB noted that there were potentially three areas that warranted governance structures: the advisor group itself, the DSNP technical specification, and the community of developers and ecosystem participants.
- JB noted that for the latter category, achieving scale while maintaining quality was important.
- DD relayed that defining community and cohorts was a struggle in the early stages of Project Liberty, but that there was not a governance structure to help at that point. BW commented that the focus of the initial work with Ethics Lab was to formulate ethical principles for the people building the technology, not necessarily the community using that technology.
- ML remarked that "governance of a community" was counterintuitive. DC agreed and stated that in his view, community is the governance mechanism. He relayed challenges within the IETF that led to effective lockup for a period of 5 years or more. He remarked that nimbleness and inclusivity were important to allow community-based governance to keep up with the pace of Big Tech and not be susceptible to capture. WS added that the voluntary nature of a tech governance community means that the participants must feel agency.
- PF asked how governance would apply to the application layer. DC said the important work would be to define what interfaces give you the ability to create a better web—focused on user control and agency while preserving safety—and make it manageable for users.
- LL asked what relationship the specification had to end-to-end encryption, where the network was not trusted but trust was placed in the individual participants' end nodes. DC replied that in his view E2E encryption was an orthogonal concern to the underlying question of trust between participants in a global context subject to disinformation and attempts at manipulation by actors with hidden motives.

Technical scope of DSNP

- WB presented an overview of DSNP, starting with the rationale for mandating a consensus system.
- He described DSNP's definition of a viable system as one with the following features:
  - Shared finality
    - Detection of dishonest/non-conformant nodes
  - Sufficiently decentralized
    - No single entity can directly or indirectly control the system
  - Observable
    - State changes must be visible to all participating applications
- He noted that these were specified to achieve desired attributes of the protocol; the protocol should be:
  - Discoverable
    - Shared content reality
    - Access to stable identities, attributes, and verification methods
  - Attributable
    - Traceable to user (directly or via delegation)
  - Tamper-evident
    - Cryptographic hashes to content

- WB remarked that blockchain is one of many possible implementations of those requirements, and that the DSNP spec does not dictate on- or off-chain status of data so long as the functional requirements are met. He noted that the Frequency blockchain is a specific configuration designed to optimize economics for a theory of adoption.
- WB then categorized the affordances offered in the current specification as falling into eight categories as follows:
1. Identity (authentication): enables users to create unique identifiers and associate and dissociate control keys that allow operations on those identifiers
2. Delegation (authorization): enables users to delegate the ability to perform operations on their behalf to other users
3. Social graph persistence: gives users the means to manage the state of their social graph from any compliant application and provides for uniform discovery of publicly shared graph data
4. Social graph semantics: defines how social graph data should be consumed by applications (e.g. follow/friend relationships)
5. Key management: enables identities to be associated with discoverable keys for access and verification
6. Announcements: enables users to announce publicly available tamper-evident content and attributes
7. Content data formats: incorporates W3C Activity Streams and W3C Verifiable Credentials specifications
8. Content semantics: defines how social networking applications should interpret the stream of announcements (e.g. to construct a feed)

- WB presented this in diagram form and took an action to look at reorganizing the specification website to better reflect these categories.
- A discussion followed around the core requirements of participating in a shared public space. DR raised a concern that having a single global identity was in conflict with building healthy communities at human scale. DC noted that the difficulty of allowing for a global context without sharing a single namespace. The group agreed to take an action to arrange for a more detailed discussion of this topic for interested participants following the meeting.

Community-based social identity

- Following on from an ongoing email discussion leading up to the in-person meeting, the group discussed the scope and requirements for a social identity that should be the focus of discussion. DC had outlined a number of potential use cases, noting that these were merely a subset of all possible use cases. WB categorized these and solicited group consensus as follows:
  - In scope: anonymous speech, control of abusive behavior, qualification for rights and privileges
  - Out of scope: government services, funds transfer
- The group agreed that this was a rational basis upon which to proceed.
- WB presented a set of definitions for the group to debate for social identity and contexts:
  - An entity (human, corporation, etc.) may have multiple identities, each designated with its own identifier
  - An identity may participate in multiple contexts, each with its own context identifier
  - It should be possible for an entity to authorize specific attributes (credentials, data) to be visible within a given context
- He noted that the current specification only contemplated identities and content on a single, implicit global context.
- Feedback on these raised two key questions:
  - Should it be possible for content to be visible across contexts (without manual reposting)?
  - Should contexts be hierarchical, and how do norms and moderation rules stack within a hierarchy of contexts?
- WB presented a strawman proposal for specification requirements to support context affordances. He noted that affordances for private contexts would mean addressing the complexities of group encryption key management, but that progress could be made on initial requirements by treating encryption as an orthogonal concern.
- WB suggested an approach toward a "V1" design that addressed context creation and state management, controller relationships, context identifiers, and applicability to DSNP announcements. Private groups and the ability to link identities while preserving privacy and avoiding correlatibility would be out of scope.
- DR raised a concern that excluding moderation affordances from the initial design could lead to unintended consequences from a safety perspective. The group agreed that this should be included.
- The group took an action to form a working group outside the core meeting structure to work toward a well defined proposal.

Sharing ethical frameworks

- In response to a previous action taken to describe the ethical frameworks adopted by ecosystem members in order to inform a harmonized ethical foundation for the governance materials generated by the group, DD presented Amplica Labs's ethics white paper.
- DD noted that the white paper was meant to be a living document so it could remain relevant to the ongoing work of the Labs organization. She noted the core "action guiding principles" described in the white paper:
  - User data control
  - Freedom of expression
  - Distribution of power
  - Transparency and participation
- The group thanked DD for the presentation. A link was shared for participants to review the detailed white paper.

Closing

- The meeting was brought to a close at 11:50am by ES.

_Minuted by WB_



