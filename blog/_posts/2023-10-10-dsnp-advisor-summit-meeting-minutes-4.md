---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2023-09-11"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
September 11, 2023<br>
MIT Media Lab</p>

**Agenda:**

1. Introduction, goals, and updates from Project Liberty
2. Governance discussion
3. Specification open issues and feedback
4. Naming discussion status and feedback
5. Update on ecosystem technical progress and roadmap
6. Use case prioritization
7. Any other business

**Attendees:**

- Constance de Leusse (CL), Project Liberty (via video)
- Kulani Abendroth-Dias (KAD), Project Liberty (via video)
- Erik Suhonen (ES), Project Liberty
- Wes Biggs (WB), Project Liberty
- Harry Evans (HE), Amplica Labs
- Braxton Woodham (BW), Amplica Labs
- Dave Clark (DC), DSNP Advisor
- Sandy Pentland (SP), DSNP Advisor
- Deb Roy (DR), DSNP Advisor
- Wendy Seltzer (WS), DSNP Advisor
- Sara Wedeman (SW), DSNP Advisor
- Wes Chow (WC), DSNP Advisor Team
- Thomas Hardjono (TH), DSNP Advisor Team
- Patricia Russ (PR), Project Liberty (via video)

**Meeting Summary:**

Introduction and status updates

- The meeting was called to order at 9:30am by ES.
- ES fielded questions from advisors relating to the ongoing advertising campaign from Project Liberty Action Network. It was noted that despite the similarity in name, PLAN is a separate entity from Project Liberty. Several advisors questioned PLAN's support for specific legislation like the U.S. KOSA bill, noting its near universal criticism from leading digital rights organizations. ES took an action to follow up with others at Project Liberty regarding the distinctions between organizations and positions expressed.
- ES advised that the next advisor meeting would be held in New York on the morning of October 25. The afternoon would be devoted to a series of talks and workshops coordinated by Project Liberty, its board of stewards, and alliance partners.
- The group selected Friday, December 8, as the date for the following meeting, to be held in Cambridge.

Governance

- KAD was introduced to the group and will be coordinating governance workstreams.
- The group agreed to establish a working group to define the right structure and artifacts required for working with interested contributors outside the core advisor set.
- The group was encouraged to finalize the mission statement document so that it could be reviewed by Maggie Little and the team from Georgetown University's Ethics Lab.
- The group discussed the IETF committee on identity linkage. DC provided an overview of the non-profit managed ORCID identity protocol and platform, which has similarities to DSNP in terms of "pulling the concept of identifying yourself out of an app".
- On the technical track, Project Liberty and Amplica Labs participants took an action to succinctly describe the technical scope of DSNP. SP suggested that the scope document define the relationship between DSNP and the IETF project, as well as DSNP and the X.509 standard.

Specification open issues and feedback

- WC shared his thoughts on decomposing the DSNP specification into multiple related subspecs. These would cover (1) core identity and attestations, (2) social primitives, and (3) content discovery. BW commented that the Web 2.0 environment has shown that power accrues at the intersection of these areas, and that had been a driver for DSNP to express them holistically in the current approach. WC noted that at a minimum, more modularity in the structure of the specification was necessary to aid in readers' understanding of the different aspects being addressed. WB took an action to work with WC and HE to examine how the spec could be restructured for clarity.
- The group discussed the notion of identity as it relates to the specification. SW argued that some piece of identity is intangible and examined the difference between ascribed and achieved status; the group discussed how these relate to DSNP's identity primitives. This led to a discussion of data minimism. SP mentioned an approach where instead of sharing attribute data, users might instead share permission for others to have visibility of attributes, a "right to query" approach.
- BW noted that choosing good defaults was an important aspect of design for privacy. BW took an action to share the ethical design principles initially developed within Amplica Labs in coordination with the Ethics Lab, so that they could be understood and applied more broadly across the project.

Update on naming discussion

- ES gave an update on the discussion about possible new names for the protocol, noting that keeping the DSNP name and acronym was the working group's recommendation. He noted that a separate naming discussion was still in progress to give a distinctive name to the "social web" paradigm that the DSNP ecosystem creates.

Ecosystem technical progress and roadmap

- HE summarized recent milestones from Amplica Lab's work with the MeWe social network, and noted that early adoption metrics were very encouraging, and migration of existing users who opt in to DSNP would be ramping up. BW noted that calls to action that had initially focused on abstractions like data freedom had proved less effective than a more direct, utilitarian approach to requesting user opt-in.
- HE explained that Labs' focus is adoption of DSNP over the Frequency blockchain, and helping the Frequency Network Foundation to ensure that Frequency becomes sufficiently decentralized to support the goals of DSNP. He noted that interoperability of different DSNP systems was contemplated as a long-term goal but was not a core focus or priority at this stage. To support decentralization, Labs will be proposing a community rewards model whereby both application providers like MeWe and the users adopting DSNP via their applications can be rewarded with tokens. These utility tokens could be used for participation in decentralized governance on-chain, and could also be used in a staking model (provider boosting) to help fund the blockchain-related operational costs of applications of interest to the community.
- The group discussed incentives for smaller applications to thrive within the DSNP ecosystem. SP suggested considering a freemium model, where providers might be progressively "taxed" based on the size of their audience, thus allowing new applications to operate in a low- or no-cost manner.
- DR questioned whether the value creation inherent in social networks should be monetized and shared, or if there were mechanisms by which it could be kept free of market cap considerations. WC noted recent work that suggested that in the social media environment, the highest margin providers would inevitably concentrate in power. He suggested that an alternative to token-based governance might be something like shared governance by a reasonable number of independent non-profit organizations, for example 12 unrelated 501(c)3 charities. BW noted that opinions on governance had much to do with where the line was drawn between public and private sector funding, and that this was an area that may evolve over time.
- HE continued with a brief summary of the roadmap for Labs' planned contributions to Frequency. He noted that supporting content for MeWe would require not only protocol support for group contexts, but also private groups, with inherent challenges around key management and key rotation, and thus providing the facilities for those prerequisites is the focus of research and development efforts at Labs, with a target date toward the end of 2024. WB noted that DSNP spec changes might be fairly minimal to support groups and private groups, but the heavy lifting to achieve data privacy goals would be on the blockchain.

Use case prioritization

- ES asked for advisor feedback on the list of use cases for DSNP, and suggestions for prioritization. DC noted that it is important to differentiate which items are core to DSNP itself and which are facilitated by other participants in the ecosystem. He suggested that we identify which use cases are necessary and sufficient for DSNP to be decentralized, and prioritize those.
- SP suggested that value transfer and attestation be added to the list. WS suggested group formation. DR suggested inter-group dialogue. ES took an action to revise the list with these considerations.

Closing

- The meeting was brought to a close at 4:30pm by ES.

_Minuted by WB_
