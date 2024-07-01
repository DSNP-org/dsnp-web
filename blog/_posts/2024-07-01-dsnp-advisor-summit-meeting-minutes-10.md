---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2024-04-18"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisory Council<br>
June 11, 2024<br>
MIT Media Lab<br>
Cambridge, Mass.</p>

**Agenda**



1. Objective, agenda and Project Liberty Institute updates
2. Comparative Analysis Working Group (CA-WG) update and discussion
3. Project Liberty updates with Q&A
4. Workshops:
    1. Ecosystem Architecture Working Group (EA-WG)
    2. Effective DSNP stewardship
5. DSNP Advisory Council structure
6. Technical specification progress and roadmap discussion
7. Governance Working Group (G-WG) update and discussion
8. Frequency functional overview, Q&A
9. Closing summary and meeting actions

**Attendees**



* Tomicah Tilleman (TT), President, Project Liberty
* Erik Suhonen (ES), Project Liberty Institute
* Wes Biggs (WB), Project Liberty Institute
* Sarah Nicole (SN), Project Liberty Institute
* Braxton Woodham (BW), Amplica Labs
* Harry Evans (HE), Amplica Labs
* Denise Duncan (DD), Amplica Labs
* Dave Clark (DC), DSNP Advisor
* Deb Roy (DR), DSNP Advisor
* Wendy Seltzer (WS), DSNP Advisor
* Sara Wedeman (SW), DSNP Advisor
* Sandy Pentland (SP), DSNP Advisor
* Wes Chow (WC), DSNP Advisor Team
* Maggie Little (ML), Ethics Lab
* Jonathan Healy (JH), Ethics Lab

**/ Objectives, agenda, and PLI updates /**

ES discussed goals for the day's agenda, including the continued focus on aligning DSNP and the ecosystem with Project Liberty Institute's (PLI) 3 core principles of Choice, Voice, and Stake. He also put forward the objectives of enhancing the efficacy of the DSNP Advisory Council and providing additional ideas on successful DSNP stewardship.

ES thanked the group for a productive previous meeting (April 18) and application of the mock trial concept to debating governance and ecosystem architecture.

ES updated the group on various PLI and broader Project Liberty initiatives.

For April 2024:



* Harvard's ASML has now hired a Senior Director to lead developments pods which will be looking at exploring DSNP and will be hiring more people.
* PLI has been progressing efforts with the India tech ecosystem. The Centre for Digital Public Infrastructure now recommends DSNP in their curated solution stack. (See [https://docs.cdpi.dev/references/home](https://docs.cdpi.dev/references/home))
* The 4/19 PLI Summit was considered a success, and participants were gratefully thanked.
* DSNP is now listed in the Civic Tech Field Guide, which is a large principles-aligned resource for others using tech for the common good.

For May 2024:



* Frank McCourt announced the People's Bid for TikTok.
* The Governance working group released the draft DSNP governance framework v1 on DSNP.org.
* Audrey Tang joined as a DSNP Advisor.
* PLI made progress on analysis of DSNP and peer protocols to support our WG.
* PLI is working to document use cases for DSNP including social media, commerce, creator economy, sports, media and entertainment, music and gaming.
* Matthew Nay from DR's group published his thesis including DSNP: “Decentralized Social Networking Protocol (DSNP) and User Empowerment: An Analysis of Online Identity Ownership, Data Privacy, and Comparative Assessment with Other Decentralized Protocols”

Ongoing projects:



* DSNP stewardship strategy (more in the breakout today)
* DSNP messaging (including "Why DSNP"), a new DSNP logo and updates to the DSNP website
* Partner Toolkit (content, tooling and support)
* Continuing with Working Groups meeting bi-weekly (generally)
* Continuing to host monthly DSNP Community Calls
* 870k+ users on DSNP and Frequency through MeWe, with social graph migration now underway. [https://metrics.frequency.xyz](https://metrics.frequency.xyz)  
* Economic task force, aligned with our 3rd principle
* Engaging with creators to better understand how we can advance DSNP and ecosystem to support them

SP highlighted his work with Thomas Hardjono in relation to the India stack, noting that many governments were beginning to sign up to implement different components, and that DSNP may be relevant to those efforts. WB noted that the engagement with CDPI was a first step in sounding out those opportunities.

DR said he would share Matt Nay's thesis with the group.

DR expressed a hunch that a form of Citizen Assembly would be important and noted the continuing intersection of his team's work with that of Jonathan Zittrain and Larry Lessig at Harvard. ES noted that this would be a good topic for an update at the PLI Fall summit.

HE and WC discussed details of the graph migration currently underway (MeWe is using the encrypted "private follows" relationship). SW asked how users were opting in to this migration, and if this was causing user confusion. BW noted that the approach was to have users opt in to both identity and graph at the initial point of contact; the current migration was catching up with previously opted-in accounts.

DR asked about the security of graph data and posited a challenge for developers to determine what could be discovered in terms of graph navigability from the current data set. BW noted that Frequency had passed a detailed security audit. SP suggested that all protocols will have certain privacy problems, and the potential leakage should be examined. He noted that timestamp-based traffic analysis was able to yield significant information, even when data on a blockchain was encrypted. WS noted that these questions tie into governance with respect to who (if anyone) has access to side channel data.

**/ Comparative Analysis Working Group /** \


WC discussed the structure of the analyses proposed as output for the working group and shared a document with proposed assignments of different feature areas to meeting attendees.

WS suggested that the group be provided with a template to be filled in for each category. WC agreed to take an action. For each category, he asked participants to provide concrete use cases, e.g. "User wants to change to a different provider".

**/ Project Liberty updates with Tomicah Tilleman Q&A /**

TT provided further updates and plans. He welcomed Audrey to the group and emphasized the value of the working group structure for the advisors.

TT suggested some themes for the Fall summit including proposing an agenda for the next U.S. administration's technology roadmap as well as a culmination of the "quilting party" begun in April where solutions could be presented.

**/ Workshops /**

The group split into two workshops as follows.

**/ Workshop 1: Ecosystem Architecture Working Group /**

DC led the first workshop as a continuation of topics introduced previously within the EA-WG, guided by a working document he shared with the group. He noted that key goals of the ecosystem included privacy, harm prevention, and decentralization of control.

DC discussed learning about the Matrix project (a decentralized network using the same underlying protocol as the Signal app) from AT. The group discussed if DSNP could interoperate with this type of protocol, and whether it could prove instructive for guiding needed DSNP functionality such as direct notification addressing, discovery and introductions.

Signal's donor-funded economic model was discussed. DC noted that operational costs for pure social network communication technology are much less than costs to operate advertising technology and monetization of the same social networks. Models such as Signal, Spotify, and Medium were discussed. DC suggested that the per-user annual cost of DSNP over Frequency be interrogated.

HE revisited the model of DSNP as a data layer accessible to many applications, detailing some of the assumptions of trustlessness that were fulfilled by a consensus system architecture and differentiating this "neutral space" from a portability goal. DC agreed that the goal of freeing the user from the need for trust was important, but noted that DSNP still assumed that users would create trust relationships with applications. The opposing forces of usability versus trustlessness were highlighted.

The group distilled a number of topics for further discussion in Q3, including data locality by date type (e.g. whether the public and private graph should exist on the consensus system as currently specified), and how the ecosystem can be made economically sustainable.

**/ Workshop 2: DSNP Stewardship /**

ES led the second workshop, focusing on three aspects:



* Current PLI stewardship framework
* What does ideal DSNP and ecosystem stewardship look like to you?
* Ideas to enhance effectiveness

A key finding from the group was that the desire to have Project Liberty's mission and principles remain highly influential to DSNP may have ramifications for the governance model.

**/ DSNP Advisory Council Structure /**

The group discussed how the current structure of the Advisory Council, including the various working groups, could be improved.

SW noted a very practical consideration, that all working group members should have edit access to the relevant documents. The group agreed that it would remedy any access control issues.

WS noted that the prior workshop had highlighted a need to get more feedback from participants outside the working group itself. DC suggested that there should be a cadence for coming together to review findings with the full group.

A structure was proposed for quarterly in-person meetings to replace the current six-weekly ones. DD noted that these meetings needed to be well planned to encourage cross-pollination between working groups. DC asked for more clarity on how decisions are made and communicated within the Advisory Council.

SP suggested the need for a clear value proposition to take to government, business, and other external stakeholder groups. He noted that the current materials took a bottom-up approach, but a top-down view was lacking, which could run the risk of enabling unwanted behavioral outcomes. The group discussed the need to unite the working groups around a common set of such use cases.

SW expressed concern that too much focus on working groups only would not leave space for anecdotal discussion.

After discussion, the group agreed that the next in-person meeting would be held in early September, with a virtual (Zoom) meeting scheduled in between as a checkpoint.

**/ Specification roadmap and discussion /**

WB summarized recent work on the DSNP specification.

He mentioned that the next minor version of DSNP (1.3) was slated for updates including:



* Public keys in core user data (final)
* Links to profile resources in core user data (draft)
* Attribute set announcements and attestation framework (draft)
* Content addressable storage for user-generated content (awaiting draft)

He highlighted key talking points that the group might use in discussing the impact of these changes. These were:



* Importance of direct ownership of key data items beyond identity and graph
* Affordances enabling user-to-user and application-to-user trust
* Options for decentralization to avoid content de-platforming and link rot

**/ Governance Working Group /**

WS summarized the recent work of the G-WG as follows:



* Publication of the draft DSNP governance framework V.1 
* Several individuals have expressed their interest in participating in governance, either verbally or through email.
* Creation of a DSNP Governance section in the DSNP forum 

Proposed next steps were outreach to specific stakeholders to engage with the framework, and coordination among other WGs. WS noted that clarity around the question of PLI stewardship and its impact on the governance structure documents should be addressed prior to this work commencing. 

**/ Frequency Functional Overview, Q&A /**

HE fielded questions and facilitated discussion on functional aspects of the Frequency blockchain, relative to DSNP.

The group interrogated how to distinguish DSNP and Frequency in conversations. BW noted that an analogy to TCP/IP (TCP over IP) had been used to talk about "DSNP over Frequency".

SP asked if DSNP over Frequency incorporated concepts of value routing, as this was an active topic from a standardization point of view for the work that he and TH were engaged in. HE noted that Frequency does not currently support NFTs. The group discussed that the concept of value could be very broadly applied to social media and in particular the monetization of content within a social context, and that the intersection of this work with DSNP should be investigated.

**/ Closing /**

ES summarized the meeting, bringing the various agenda topics together, tied into the overall vision and strategy.

The next in-person DSNP advisory council meeting will take place on September 4, 2024 at MIT. The following in-person meeting will be held at Georgetown University on November 18, 2024, just before the next PLI Summit.

_Minuted by WB_
