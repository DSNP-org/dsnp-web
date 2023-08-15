---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2023-06-15"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
June 15, 2023<br>
MIT Media Lab</p>

**Agenda:**

1. Review of last meeting’s minutes / takeaways, review of today’s agenda, proposed schedule of outputs for the Advisors
2. “Where are we in the stack?” conversation
3. Product roadmap and architecture discussion
4. Institute team shares mission, principles and name proposals
5. Continued discussion from Workshop #1 of governance principles
6. Amplica Labs team continues tech deep dive
7. Open questions, housekeeping, determination of next meeting, etc

**Attendees:**

- Braxton Woodham (BW), Amplica Labs
- Christian Tom (CT), McCourt Institute
- Constance de Leusse (CdL), McCourt Institute (remote)
- David Clark (DC), MIT Research
- Deb Roy (DR), MIT Center for Constructive Communication
- Erik Suhonen (ES), Project Liberty
- Harry Evans (HE), Amplica Labs
- Sandy Pentland (SP), MIT Connection Science
- Sara Wedeman (SW), Behavioral Economics Consulting Group
- Thomas Hardjono (TH), MIT Internet Trust Consortium
- Wendy Seltzer (WS), Tucows
- Wes Biggs (WB), Amplica Labs
- Wes Chow (WC), MIT Center for Constructive Communication

**Meeting Summary:**

The meeting was called to order at 9:00am by BW.

Opening

- BW introduced the session and discussed focusing on (1) further discussion of technical design decisions, (2) governance track, (3) how to help drive adoption.
- CdL noted certain artifacts that have been created for advisors’ review, including a mission document, proposed charter, and proposed work plan for advisor group (governance track, tech track, community building, content). These are currently rough drafts to be finalized through an iterative/consultative process. She suggested a 2-3 week timeframe to collect feedback post this session.
- ES introduced himself having recently joined Project Liberty to run its tech track. He noted the need for a broad ecosystem of partners, and is hoping to work collaboratively with advisors to help create awareness and adoption, as well as a map of the players in this space and their roles.

Where are we in stack?

- WS opened a discussion questioning which layers the advisors should be focused on. She related the work to the “hourglass” model of OSI layering; similarly, DSNP allows for applications that can be doing very different things all using the same low-level protocol. She noted that some of the stated goals for the group for improving human interactions are not well leveraged from the protocol layer; if talking about specific behaviours to encourage or discourage, we should be thinking about the architectures and human interactions, how that has worked with technologies of the past, and how technology can be tweaked to help achieve goals.
- DC asked if you can discipline behavior within an ecosystem or if that has to be done via an app, giving an example of the development of adding code to the web; security/privacy tends to lose out to features and economic growth. He said he felt we were clearly trying to create an ecosystem but last time ended up talking about controlling abuse a lot, and it was unclear what layer this should be at.
- SP said he thought the real goal is giving control over data. Data has become valuable, with parallels with the invention of money or commoditization of labour. He saw a framing in terms of controlling and transacting with data, whether that is sharing cat GIFs or finding people who share a rare disease. To enforce the ability to create good transactions, data has to be treated more like money.
- BW said that DSNP is meant to be low-level to address affordances that are necessary; but that Project Liberty is covering the full stack. TCP/IP allowed communication, the web allowed for a network of computers, and Web2 allowed for network of people – but led to the surveillance economy. DSNP’s focus is on how to reengineer that low-level aggregation of data – hence the need for “Social Primitives”. These must have a sort of economic Ulysses Pact built in from day one to remove the monopoly on value generation from private hands.
- DC discussed parallels in the evolution and design of TCP/IP to ensure separation from commercial motives. When a participating private company touted its own solution, it promised not to put license restrictions on it; when this promise was broken for commercial leverage, the technology (XNS) vanished rapidly because it required a license agreement. TCP/IP succeeded because the US government paid for it, and allowed for an an explosion of investment in the usage of it. Society made its money, but TCP/IP itself didn’t make money.
- A discussion followed with general agreement that the building blocks (protocols, social primitives, “affordances”) must remain non-commercial in order to build trust and allow the ecosystem as a whole to be economically successful and rewarding. SP gave an example of collecting data on rare diseases. WB commented that Apple and Facebook had similar systems for Covid data sharing, but both approaches were proprietary. BW noted a critical distinction between “Can’t be evil” (what we seek to achieve) vs. “Don’t be evil”.
- WS summarized the discussion and encouraged the group to recognize what commitments we can and can’t make; we can have goals that don’t all translate into specific technical artifacts. BW noted that many here may be more interested in full stack, but urged the group to use this to inform the protocol as a first priority.
WC suggested that DSNP is missing context; when I say something, I have an implied context of facts, audience, etc. If everything is public there is no clear idea of a context. He noted that communities are a convenient way of capturing context but not equivalent.
- HE noted that there have been prior discussions about groups and other context-related concepts, but that it is not fully resolved how to delineate the approach between protocol and application layers.
- WC agreed to take an action to provide a discussion document on context and required affordances for the next meeting. He questioned whether a shared schema for context should be part of DSNP or a separate spec, but that it was crucial to avoid “context impedance mismatch”. He noted the terminology of “Context collapse”: when boundaries for understanding go away, communication breaks down and becomes toxic.
BW argued that, seen as a transaction log for human interaction, DSNP should capture this context; by being shared state, people can’t rewrite history. SP noted that systems are being built to allow auditing by injecting context where appropriate.
- The group discussed challenges between anonymity and traceability, citing the failure of sharing of medical records due to incentives for providers to create “vendor lock-in” as well as limitations in the expressive power of early systems.
- WB commented that two overall themes of the discussion were that (1) affordances in scope for the group may go beyond DSNP specifically; (2) “social networks” are different than “social media” and underpin many more types of applications.
- BW brought up the idea that moderation is too opinionated to be part of the spec; but some affordances are necessary to create the ability for moderation to exist at other layers, such as identity, and mechanisms for identifying bad actors. CT asked if we can prevent people ignoring the affordances given technically, or if this needs “terms of service”. DC said he thought it could be done via the spec. As an example, WC noted the intent of the “tombstone” announcement in DSNP can be enforced to an extent by the protocol disallowing replies to tombstoned announcement. SP noted that surrounding agreements, often rooted in government and legal frameworks, were critical to well functioning systems like the banking system.
- SP discussed the need for both trusted and anonymous spaces; trust requires reputation. SW argued that trustworthiness may be a core affordance, and that it was more important to talk about trustworthy spaces rather than trusted spaces. HE noted work in progress on a spec addition for attestation; in DSNP, identity is pseudonymous, but trust, via attestations, can be layered on top.
- SP noted a dichotomy between systems that were secrecy-based (e.g. medicine) rather than anonymity-based foundationally. HE noted that the protocol can represent specific KYC components, including those that may be required by specific legal regimes. SP gave the example that EU regulation requires knowing AI vs. human, but that that doesn’t need to be part of DSNP if it can be referenced.
- The group discussed the origin of the term affordances as related to usability; SW noted that the term came from Don Norman’s work as well as J.J. Gibson, who wrote on the way reality is perceived from different perspectives. DR gave the example that the affordance of a leaf is different if you’re a deer (food) or an ant (shelter). He asked that the group come up with clear use cases and examples; in order to create affordances from visions like McCourt’s, we need to game out the negative space of those affordances. BW asked that DR take an action to bring concrete use cases to test.
- DR noted that his team is working on a particular application that they hope DSNP can be leveraged for or evolve for. He asked what the story/narrative should be for users of DSNP; in other words, what would be a compelling reason for billions to leave Facebook or TikTok, for example. He challenged whether data ownership was a strong enough selling point for mass adoption.
- As an example of companies successfully driving adoption of protocols that were inherently more technical, SP mentioned that Google’s change to rank HTTPS sites hire was enough to drive rapid adoption. WC noted a similar pressure on the decentralized ecosystem from App Stores to police access to illegal content.
- The group discussed alternatives to “own your own data” that may be compelling for end users. HE noted that interoperability gives you a “vote with your feet” option. SW remarked that peer behavior is not always smart but can be very powerful.
- To that point, WC noted that Web3 has latched on to exit but not voice and loyalty; these are competing concerns per the work of Albert Hirschman.

Roadmap

- WB discussed progress on proposed additions to the DSNP specification for Attributes and Attestations building off of the W3C Verifiable Credentials specification. He said a draft should be ready for review by the end of the month.
- HE discussed research work on groups and private messaging. He noted that these require a lot of encryption work and the Labs team has been looking at how to ensure usability when dealing with core concepts like key rotation. Groups are a key “noun” in the space, but it is less clear whether this is a DSNP concern vs. an implementation concern, so this work is ongoing.
- WB noted the continuing transition of administration of DSNP (and potentially other artifacts) to Project Liberty and DSNP.org. The DSNP.org site has been updated with advisor bios and other information.
- BW reviewed the Amplica Labs commercial roadmap, focused on partnering with existing social media providers, with a multi-step rollout of DSNP identity and social graph to opted-in MeWe users a top priority.
- WC asked if applications could use identity but not messaging features of DSNP. HE answered that identity and graph may come first for some providers, but the intention is to bring all providers that utilize messaging into the protocol’s environment.
- WC asked about the interaction model for applications consuming content from DSNP. He noted that the more expensive it is to consume data, the more centralization of auxiliary services is likely to occur. HE responded that Amplica is making tooling to make it easier, and helping providers create services. One project is to build an instance of a content indexer so users don’t have to listen directly to the chain events “firehose”. - A similar area is batch data declaration tooling around IPFS to improve developer usability. He also pointed to Labs’ work on the Amplica Access wallet, which will give users the ability to manipulate their graph “generically”, that is, with no reference to a particular application or provider.
- SP noted a distinction between transactional networks and social networks, and the importance of providing tooling to analyze hidden patterns, such as botnets and state actors; notoriously, these groups tend to go in and out of the shadows. HE said that graph indexers will need to exist to provide data for these analyses, but creating implementations of these is further down the Labs roadmap vs. content indexers. BW asked that WC and SP take an action to identify some use cases for graph analysis based on their work and insights into the challenge.
- SP asked about instrumentation of the adoption curve as MeWe users go online. BW confirmed that Amplica Labs and MeWe were collecting statistical data to analyze and optimize this process.
- DC asked which relationships were being migrated. WB said all MeWe relationship types would be migrated. The spec affords for privateFollow, publicFollow, and privateConnection, and these were all being considered. DC raised a concern that by doing this migration before additional context metadata is defined, the semantics of these relationship types may become confused (e.g. Facebook friend vs. LinkedIn connection).
- The group discussed the pros and cons of keeping these relationships “universal” vs. contextual. WS gave an example that users may want a universal blocklist to block unwanted intrusions from a particular entity regardless of the context; SP countered that a user may not always want this to be universal. In a similar vein, the group discussed the level of detail that should be exposed or expected from users when annotating relationships. SP that it may be too complicated for individuals to annotate all of their relationships, and that in other contexts like banking and medicine, there are trusted fiduciaries that help individuals with this vocabulary. SW noted that Facebook has double opt-in annotations to establish relationships with specific annotations such as friend, family, colleague. HE added the nuance that we may need both public and private classifications of relationships. WC noted that the Nostr protocol has added a taxonomy of content labels e.g. for NSFW content, and the community can define these labels. The group agreed that if the perceived difficulty of migrating ones graph was too high, people will avoid the process entirely.
- BW shared MeWe’s live DSNP-based registration process at MeWe - The Next-Gen Social Network. The group discussed the branding/marketing of “Social Web” and what value proposition of DSNP would be most compelling for end users. Several concepts were discussed, including taking control of your social experience, contrasting with the experience of the megaplatforms, and building bridges to a new generation of apps. The group concluded that the latter was most likely to resonate with users. DR noted that it is important to avoid the perception of “false advertising” when bootstrapping an ecosystem, and asked what the minimally viable ecosystem is to make a promise and deliver on it from a change of user experience viewpoint. An invitation to be a bridge builder may be the most viable at this stage, as the promise is simply that it will be a bridge to somewhere good.

Governance

- WS introduced the governance discussion with a recognition that there was a need to level set on what we were meaning to govern; (1) the evolution of the DSNP protocol, and/or (2) building a forum further up the stack involving the coordination of applications and users across the Social Web. BW asked that the protocol be considered the most urgent need, but that this can be informed by an understanding of the goals the broader ecosystem should seek to achieve. DC noted that this may need to be slightly broader in order, and a key goal was to allow developers to contribute at this stage.
- WS said that a practical need was a structure for how changes are adopted; as a group, the options were to buy, borrow, or build a governance structure. BW said his position was that DSNP should borrow something that gives its governance credibility and addresses developer worries, and that the focus should be more on trust than innovation.
- DC said a strong commitment to backward compatibility is important. A process that has worked in IETF is to hold Birds of a Feather sessions to confirm “proof of interest” before a proposal goes too far.
- WC asked how the group can ensure that Frequency doesn’t deviate from compatibility with DSNP. HE said there is potential for Frequency governance changes to make this happen; WC suggested that one mechanism would be for the Frequency Foundation to hold a large stake but only use it in case of a violation of the implementation agreement. DC noted that multiple implementations were necessary for TCP/IP to progress and succeed; at the time this was accomplished by DARPA grants for multiple implementors.
- Various existing bases for governance structure were discussed, including the Mozilla Foundation, iSpirit in India, and the Linux Foundation. WS noted that the Linux Foundation has mechanisms to create an off-the-shelf build-your-own governance system from templates. The group agreed that creating a discussion document from templates would be a good way to focus on next steps.

Mission/Vision Statements

- The group reviewed and discussed draft documents prepared by Project Liberty staff.
DC suggested that the mission should address more specific goals such as data ownership; preventing harm; preventing capture by private interests (concentration of power).
- The group discussed concerns about the “social web” nomenclature, and whether this would appropriately convey that a DSNP system would be new and different from previous social networks and systems. Some terms discussed included human-centered and shared. Other concepts were the digital environment or a digital transaction platform. SW suggested trying to capture the notion of creating a place that is open, safe, trustworthy and ultimately delightful.
- DC suggested that the ordering principles be ranked as discussed in the seminal 1988 internet paper.
- An action was taken for advisors to further review and comment on the documents over the following two weeks.

Closing

- Wednesday, August 2 was proposed for the next meeting.
- The meeting was adjourned at 4:30pm.

_Minuted by WB_
