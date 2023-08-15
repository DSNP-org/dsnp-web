---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2023-08-02"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
August 2, 2023<br>
MIT Media Lab</p>

**Agenda:**

1. Introduction, goals and status from Project Liberty
2. DSNP competitive analysis and ecosystem discussion
3. Update on technical work in progress
4. Interoperability use case discussion
5. Overview of Attribute Set Announcements proposal
6. Discuss protocol scope and naming
7. Discuss intersection of DSNP with current AI and data rights issues
8. Discuss use cases and affordances required to capture groups/contexts/personae

**Attendees:**

- Erik Suhonen (ES), Project Liberty
- Wes Biggs (WB), Amplica Labs
- Harry Evans (HE), Amplica Labs
- Braxton Woodham (BW), Amplica Labs
- Dave Clark (DC), DSNP Advisor
- Sandy Pentland (SP), DSNP Advisor
- Deb Roy (DR), DSNP Advisor
- Wendy Seltzer (WS), DSNP Advisor
- Sara Wedeman (SW), DSNP Advisor (via Zoom)
- Wes Chow (WC), DSNP Advisor Team
- Thomas Hardjono (TH), DSNP Advisor Team

**Meeting Summary:**

- The meeting was called to order at 9:30am by BW.
- ES gave an update on Project Liberty status and creation of the Project Liberty Action Network 501(c)4 and clarified the separation of concerns between PL, PLAN, and Amplica Labs. He noted that the groups were still figuring out how different partnerships fit under the different workstreams. A head of communications has recently been hired at PL and will be involved in promotion of DSNP. TH suggested that a workshop or panel held at MIT could be a useful way of raising awareness and visibility of DSNP.
- BW gave an update on MeWe's plan to transition users to DSNP for identity and social graph, with the next phase of migration happening in Q3.
- SP brought the group's attention to the Unstoppable Wallets project, which addresses key recovery by sharding with threshold encryption in concert with a trusted computing environment (SGX).
- DR reflected on the importance to distinguish between social networking and social media. A social network for trust may be different from a social network for media (e.g. TikTok). Social network has a broader definition, and many times users may not be consciously thinking of an application as a social network; for example, Slack is a social network even if not branded as such. SP agreed that the discussion on fixing social is often focused on media. DR suggested that this could be better framed by using the phrasing of a "social network for [X]".
- BW noted in related industry events that the Narwhal project is being discontinued, though Blink has been incorporated into Cortico's stack.
- ES noted the potential for partnership with the Beckn protocol (decentralized commerce). BW commented that this would fit into a sequence of evolution conceptually, with areas of identity, communication, contexts, and commerce all necessary for the long-term success of the project. SP noted that there were complexities in how Indian banks see decentralized approaches such as Beckn. WB and ES took an action to get a map of Indian projects in this space such as iSPRIT and UPI.

DSNP competitive analysis

- WB gave an overview presentation comparing some of the technological details of several of the highest profile decentralized and federated systems for social (Frequency/DSNP, Bluesky, Mastodon, Lens, Farcaster, Nostr, DeSo, and Threads given their planned ActivityPub support). He noted that it is hard to do apples to apples comparisons given the different configurations of various offerings; for example, Mastodon is a large piece of the Fediverse, but not all Fediverse users are Mastodon users. Similarly, the relationships between blockchains, protocols, and applications exhibit different approaches for different projects.
- BW noted that decentralized social is currently in a moment of market fragmentation and uncertainty. DR questioned whether Threads would allow account migration even if they do federate with other ActivityPub servers.
- WC suggested the inclusion of Tumblr (135m MAUs) given their announcement of ActivityPub support.
- SP noted the approach of companies like Flybits for commerce using a local access point model. He pointed out the emergence of Akoya as a trusted intermediary between banks for KYC was underpinned by a model where they took on liability.
- DR suggested a multicompetitive map may be necessary to look at some of the adjacent spaces.
- The group discussed the competitive axes used for the assessment, and agreed that merely categorizing the technology of various players was only a first step; a values-based framework needed to be made to explain and justify the rationale behind DSNP's opinions and placement on these axes.
- Several reframings of categories for the competitive analysis were suggested. DR noted the difference between historical concepts of the public square and the way the term is applied to mass communication in today's social networks, and suggested that "suitability for democratic discourse" might be a more useful criteria. SP noted that a micro-community model has a natural tension with building out meaningful reputation systems. DC suggested that freedom of assembly or the right to private assembly could be assessed. WS added the concept of maintaining community boundaries.
- BW asked if the technical criteria could be meaningfully grouped into a smaller number of mission-driven criteria, and suggested these might focus on individual empowerment, health and safety, and adoption and scale. DR noted that it may be useful to group these but it may be more meaningful to matrix a set of technical criteria with more abstract goals.
- BW queried whether the concept of the intimacy gradient might capture one high-level aspect. DR explained that the term intimacy gradient comes from architectural studies into the need for creating distinct spaces and the norms within those spaces.
- SP suggested we attempt to capture suitability for community and use by people interested in coming together to do things. For safety, this could be the ability to find and correct criminal behavior. BW noted the need to include children's mental health in this goal. WS remarked on the difficulty of capturing norms in a protocol that may have different jurisdictions overlapping in practice. SP noted that there are at least some universal norms that could be looked at. ES suggested that the definitions cover values and principles vs. the "how".
- WS argued that there is a feedback loop between the values you choose and the community of users that are attracted to a particular system. SP suggested the group attempt to converge to something sensible that aligns with PL stated goals and suggested creating two sentences for each of the values, forming the "why" behind the value ratings.
- DC suggested control point analysis as a method that had worked to help structure work on previous protocols. He asked what aspects were meant to be transportable; e.g. could you build Medium using DSNP? The focus would be on describing the centering of the desired user experience, and how generalized this could be within the way the system is embodied. BW noted that the early direction of DSNP purposefully started on the "big public room" use case but envisioned work through the spectrum of spaces and relationship types, possibly down to one-to-one messaging. DC cited the work of Zuboff and others that surveillance capitalism creates selective amplification. In that way, it is important for the system to define specific control points such as search and amplification aligned with the overarching goals.
- DR noted that the economic model of a system may contribute to polarization, leading to tradeoffs and complexity. Incentives for publishers can be very different between subscription and ad models, for example.
- WC asked that the group set up a more structured means of sharing documents and topics, suggesting a tool like Notion. ES took an action to work on creating this environment.
- SP suggested a discoverability criteria would involve a method for searching on descriptive user features without sharing public data; in other words, can you find a set of people who fit given criteria without individuating them.
- The group discussed trust networks and the ability to detect that communication was not from a bot or AI. SP pondered if there was value in using the X.509 format to encapsulate authentication over the existing HTTPS channel from a browser environment as a means of kickstarting the injection of this data. He noted that this discussion was very timely given recent EU AI regulation. The group discussed the challenges of working with big companies such as Apple and Google to take these approaches. WS mentioned a similar governance challenge to get the public to trust a private institution.
- DR noted the social capital of non-profit organizations could be used to create networks of trust. WC is actively exploring this area with a group of MIT students. SP related a similar model in finance where a network of certified fiduciaries numbering a few thousand were used for identity verification. DR gave an example from work with the New York City department of health and hygiene, where trust is sourced from the grass roots; they have verified two dozen community organizations that are location and demographic/vertical based. WC noted that this leverages the real-world private marketplace of grassroots trust that exists today. SP related this to the role of Community Reinvestment Fund, USA (Comm-USA); rural electrical co-ops are a good example of bottom-up organization used for broadband distribution.
- With respect to identity providers and verification, WC asked about the announced Frequency-KILT integration. HE answered and noted that while KILT technology enabled attestations to be available and verifiable via the blockchain, they were not an identity verification provider. TH noted the importance of defining who would take on liability in this approach. HE mentioned the Worldcoin project as a top-down approach to trust and identity verification, and asked how we could define a scalable bottom-up version instead.  SP noted a study on reciprocal interactions to predict trust found this was highly predictive. WC mentioned a presentation that was made for MIT's CCC could be shared as resource. SW shared a link to a relevant paper titled "Trusting the trust machine".

Attribute Set proposal and technical work in progress

- WB talked about affordances in attribute sets and attestations, and gave a brief overview of a DSNP improvement proposal providing a technical means of associating W3C Verifiable Credentials with DSNP. The proposal looks at an open ecosystem for claim schema that could facilitate a wide range of use cases and be used to annotate DSNP users, DSNP content, and arbitrary external content.
- WB briefly touched on other relevant topics in the DSNP specification project, including a discussion on the ability for providers to remove content from the system currently being discussed in a github issue. He urged any interested participants to contribute to the online discussion and to join the next monthly DSNP community meeting and thanked WS for her feedback after attending the previous session.

Interoperability use case

- ES talked about Project Liberty's interoperability initiative, which seeks to meaningfully demonstrate the way different applications can interact and collaborate via DSNP. PL will be working toward specific examples (visibility of the shared social graph for following) that can be demonstrated in real-world apps by the end of the year.
- DC suggested it is important to have a list of which functions we want to prove and show (beyond this initial work on "public follow"), and urged the group to consider the ability to moderate the replies to one's own post as an important use case. WS noted that there were a broad range of technical solutions for this, which can scale from a shared blocklist to community-driven moderation.
- With regard to the proposed initial use case, BW noted that there was a need to establish product overlap between Fora and MeWe. WC spoke about the importance of groups to Fora relationships, and asked how he could connect with MeWe; an action was taken to coordinate a meeting.
- This led to a discussion on apps with specific vs general modalities, and how DSNP could support the full range of these, but that not all content was expected to be part of a single global stream. BW detailed one approach, where global content could link out to specific apps to interact with particular content types or communications. WC suggested that it might be valid for audio content from Fora to be shared (if the user chose to) more broadly, and the shared version would follow DSNP conventions for threaded replies and reactions.

Protocol scope and naming

- ES kicked off a discussion on the naming of DSNP, noting that Project Liberty and its academic partners were interested in understanding how a wider scope could be encompassed, while potentially still keeping the acronym the same.
- HE gave historical context of the naming of DSNP and noted that the current name (Decentralized Social Networking Protocol) aptly describes the primitives that the protocol expresses.
- Alternatives such as "Digital Sovereignty" and "Digital Society" were discussed and analyzed. It was noted that "Sovereign" has political connotations that may be undesired. It was discussed that "Decentralized" itself has different connotations to different audiences; for example, it was used by Apple and Google when positioning their COVID-19 tracking solutions vs. EU government solutions.
- DC suggested that establishing a short description of the goal of the project would help in naming. "Protecting the connected experience" was suggested for discussion. The group discussed who the intended audience was for the name, and that the protocol name may not be as important as establishing a higher-level name or branding that could be used, for example, in compliance badging. BW noted that in addition to end users and developers, another focus is government/lobbying efforts. SP referenced a Stanford group that is looking to produce a Federalist Papers-like "Digital Society" corpus.
- HE suggested that the "seal" might encompass both protocol and policy/regulation and thus relate to the wider scope of PL, not just DSNP. DC noted that connecting affordances to mission goals ultimately requires a leap of faith, and that it would be important to articulate the position that, for example, connects interoperability with the higher-order goal of protecting democracy.

AI and digital rights issues

- BW introduced a discussion on the relationship between PL and current trending issues, and asked how DSNP might be utilized or connected with these. When initially conceived, DSNP was related to work on improving children's mental health and preserving democracy; now AI and data rights are big public topics.
- HE suggested that bot-or-not attestation is foundational to provenance, which allows for the identification and auditing of human-generated content. SP gave an example from the carbon capture world which uses zero knowledge proofs to show provenance without revealing identifying information. SP/DR noted a student project under their supervision to capture metadata for training data given to LLPs.
- WS commented that copyright seems the wrong tool to talk about data extraction permissions, thus we were at an inflection point where new strategies were required. It was noted that a liability regime is still being established.
- DR showed an example from a CCC project of provenance of audio content. The core needs for attestation are to know is this a real person and is this a real action they took. He noted that community groups often had pre-existing attestations that could be brought into a system.
- DR noted an Austrian project to both preclude unauthorized use of a designated corpus and enable a high quality training set.

Contexts and personas

- WC expanded on the concepts of contexts and personas and how they relate to groups and communities.
- HE noted that early DSNP designs included personas, but led to hard problems around prevention of correlation and amplification. WB suggested that the current notion of a DSNP User Id could be mapped to a persona, with context switching between personas being handled via a wallet interface or similar.
- WC felt that the "person" concept (owner of multiple personas) was important to include in the protocol; because many useful attestations would be made at the person level, the ability to make particular attestations visible under various persona was a key affordance.
- TH mentioned a past paper he published that gave a cryptographic approach to protecting against correlation between Bitcoin addresses while still allowing for verification of validity.

Closing

- A tentative date of September 11 was proposed for the next group meeting.
- The meeting was brought to a close at 4:30pm by ES. 

_Minuted by WB_
