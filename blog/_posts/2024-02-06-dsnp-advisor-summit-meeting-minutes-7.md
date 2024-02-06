---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2024-01-23"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
January 23, 2024<br>
Berkman Klein Center, Harvard University<br>
Cambridge, Massachusetts</p>

**Agenda**

1. Introductions, organizational updates and upcoming events
2. Q&A with Tomicah Tillemann
3. DSNP ethics, use cases, ecosystem and economics
4. DSNP governance update and discussion
5. "Plays well with others": Mapping DSNP's intersection with existing and emerging standards and projects
6. Technology Breakout Group A: Community and context affordances
7. Technology Breakout Group B: Hosting, access, and availability of content
8. Summary and closing

**Attendees**

- Frank McCourt (FM), McCourt Global and Founder of Project Liberty
- Tomicah Tilleman (TT), President, Project Liberty
- Erik Suhonen (ES), Project Liberty Foundation
- Wes Biggs (WB), Project Liberty Foundation
- Sarah Nicole (SN), Project Liberty Foundation
- Braxton Woodham (BW), Amplica Labs
- Dave Clark (DC), DSNP Advisor
- Deb Roy (DR), DSNP Advisor
- Wendy Seltzer (WS), DSNP Advisor
- Sara Wedeman (SW), DSNP Advisor
- Sandy Pentland (SP), DSNP Advisor
- Wes Chow (WC), DSNP Advisor Team
- Maggie Little (ML), Ethics Lab
- Jonathan Healy (JH), Ethics Lab

**Apologies**

- Harry Evans, Amplica Labs
- Larry Lessig, DSNP Advisor
- Thomas Hardjono, DSNP Advisor Team

**Meeting Summary**

_Introductions, organizational updates and upcoming events_

The meeting was called to order at 9:00am by ES.

Tomicah Tilleman was introduced to the group as the new president of Project Liberty and interim CEO of the Project Liberty Foundation 501(c)3.

ES reviewed progress since the last meeting, as well as a meeting objectives and an enhanced meeting structure.

ES discussed the goals and some initial logistics for upcoming events.

_Q&A with Tomicah Tillemann_

FM and TT presented Project Liberty's key focus areas:

- Agency and control of data
- Voice in tech platform governance
- Participation in economic value creation

A lengthy dialogue followed as advisors parsed the proposed wording of these goals and added suggestions to strengthen them.

_DSNP ethics, use cases, ecosystem and economics_

SN summarized work to develop an ethical framework for responsible innovation for the whole ecosystem. PL staff engaged in multi-stakeholder consultations throughout 5 continents between June and November 2023. She noted that DSNP is a flagship representative of this framework as it reflects this ethical approach and requires the recommended principles for successful implementation.

She noted that the draft is open for comments until February 16, and bilateral discussions are welcomed to address questions and thoughts. ML, JH, DR, and others took actions to review.

ES summarized active work with partners engaged with DSNP, including MeWe, MIT, Harvard, and the Foundation for Interoperability in Digital Economy. He noted that PL was additionally starting to engage two additional key groups, the government and investment sectors.

ES noted that work was underway building a DSNP economics working group with Erik Brynjolfsson (Stanford) and others, and that this would be a key agenda item in the next (March 2024) advisor summit.

SN announced the formation and initial structure of the DSNP Governance Working Group (G-WG). The G-WG is chaired by WS with participation from Denise Duncan (Amplica Labs), ES, HE, SW, SN, WB, and WC. This group remains open to all advisors and WS will reach out on more specific requests when needed. The G-WG will meet every other week with the next meeting to be held in person the morning after this advisor session. The group's initial goal is the publication of a first draft iteration of a governance framework document for feedback in April 2024 which will define the mechanisms by which the protocol specification is governed. A version incorporating public feedback from this review period will then be produced, targeting Q3.

SN noted the publication of the DSNP Mission & Principles document on dsnp.org and thanked the advisors for their contributions.

_"Plays well with others": Mapping DSNP's intersection with existing and emerging standards and projects_

WB posed questions on how DSNP should relate to other potentially like-minded projects in the wider decentralization technology landscape, including the Fediverse (ActivityPub-based projects including the Mastodon app as well as similar projects like Bluesky), blockchain dApps in the Ethereum, Polkadot, and other ecosystems, decentralized Semantic Web projects including Solid and protocols from the Decentralized Identity Foundation, and platform-centric and independent password/passkey management solutions. BW noted additional opportunities with values-aligned projects with peer-to-peer messaging systems and digital rights systems. WB argued that DSNP should not take an isolated approach but embrace the existing intersections with these projects and build a framework for further engagement and collaboration.

Advisors noted that these groups had wildly varying levels of user adoption. WC noted that there was a difference between market share and mindshare, and that both elements were important to consider.

BW proposed that three principles be used to determine the level of active engagement with outside projects: (1) mission and value alignment with DSNP; (2) complementary problem domain; (3) technical implementation specifics.

The group discussed and proposed a framework where projects and technologies with overlap on (1) only would interface with Project Liberty's Alliance; projects with relevance to (1) and (2) would be worth investigating and documenting solution architectures for integration, and projects overlapping all three could be candidates for direct collaboration with Project Liberty supported by resources from Amplica Labs.

_Technology Breakout Sessions_

The group divided into two breakout sessions to examine the protocol affordances required for key scenarios expected to be supported by the protocol.

_Community and context affordances_

The first group examined questions related to moderation controls, group membership models, and the expression of multiple facets of identity.

The workshop asked participants to describe a person’s experience participating as a community member within a social networking context. How do they find out about the online community? How do they join the online community? What personal data do they reveal within that context? How do they comprehend and abide by the norms set by the community?

The group discussed how users might find others with similar interests in a privacy-preserving way. For example, individuals who shared a rare disease could provide proof of their diagnosis in a way that allowed them to find private groups that catered to their needs and interests, without those groups (or membership relationships) needing to have public metadata.

The group discussed models for membership where joining a group could be attestation-based (as in the rare disease example), administrator-based, or both.

Moderation was discussed as having multiple levels: permanent bans from a group for a user vs. moderation of specific posts or topics.

The group discussed what the in-protocol representation of groups should consist of. Fully peer-to-peer groups (that is, groups without a membership list available in any well-known location) can be powerful, but the difficulty of maintaining even a simple text messaging group with both iOS and Android users showed that platforms can often abuse their power in these scenarios; control and agency affordances at the protocol level were therefore important.

_Hosting, access, and availability of content_

The second was asked to examine questions about content addressability and longevity, interactions with legal and regulatory authorities, content removal, and rights to be forgotten. Participants were asked to describe a person’s desired experience and the implications on data locality for each of the following scenarios:

- A person in a war zone fears censorship or reprisal.
- A law enforcement officer wants to remove illegal content from the network.
- A social networking application provider's business shuts down.

Recommendations that came from this session included assigning deterministic CIDs (Content Identifiers) to all content items in the system (not just batch files) would allow for a number of use cases. Any services that cache or index content (like search engines) would also need to be aware of content removal semantics.

The group noted that censorship resistance entails not just the ability to speak, but the ability to be heard; in DSNP, "speaking" is addressed by the announcement model, but being heard relies on the ability for others to reliably find the content. While DSNP as a protocol cannot guarantee that content will continue to be hosted, it can ensure that it is locatable through a CID, not just a specific hosting location.

On the other hand, avoiding reprisal for content relies on the ability for a content creator to be known and to be found. DSNP can facilitate this by ensuring that it is not necessary to include personally identifiable information with any announcement. Onion routing (such as Tor) may additionally help provide anonymity at the IP address level. Avoiding reprisal was contrasted with law enforcement mandates to identify the purveyors of illicit material. However, participants agreed that ultimately the DSNP model required some entity, somewhere, to choose to host and serve content; this entity must therefore be willing to take whatever legal risks this entails, and could ultimately be identified.

The group discussed the concept of a "takedown order". Rather than mandating compliance by network participants, a takedown order should be assessed based on its sender's reputation. For example, the NCMEC is an organization that has a good reputation for identifying and working with social networks to remove CSAM; a takedown order digitally signed by that organization would likely command more attention and respect than one issued by an unknown entity. Takedown orders could identify the jurisdiction of the issuing entity as well as metadata specifying the rationale for the order. Service providers could each make their own determination as to compliance. The group noted that blocklists for IPFS exist already, and there are well established procedures for handling requests for RIAA, DMCA and similar.

The group noted the difference between takedown notices and "soft removals", which may warrant separate announcement types.

In the following joint discussion, it was suggested that experts from law enforcement agencies be consulted to assess the threat model in the protocol in a so-called "red team" exercise.

DR asked if there were scenarios where illicit content could be stored in encrypted user data in a DSNP consensus system. WB noted that the ability to do so was limited currently to the private social graph objects, which could not be publicly introspected. It was noted that such abuse would be subject to consensus system governance including reputational risk to those who aided the perpetrators as delegates, but the risk could not be entirely eliminated.

_Summary and closing_

ES reviewed the progress made in this meeting, relative to the meeting objectives.

ES reminded the group that the next in person meeting would be held March 7, 2024, with the MIT location to be confirmed. The group discussed holding the subsequent meeting to coincide with the Project Liberty Summit at Harvard in April. ES said that details would be forthcoming.

The meeting was brought to a close at 4:30pm by ES.

_Minuted by WB_
