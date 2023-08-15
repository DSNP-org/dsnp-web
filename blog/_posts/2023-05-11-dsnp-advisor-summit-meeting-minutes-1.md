---
layout: post
title:  "DSNP Advisor Summit meeting minutes - 2023-04-20"
tag: minutes
--- 
<p>Meeting Minutes<br>
DSNP Advisor Summit<br>
April 20, 2023<br>
MIT Media Lab</p>

**Agenda:**

1. Welcome: DSNP and other protocols, introductions
2. Problem domain and guiding principles
3. Review of core technology decisions
4. Whiteboard on governance structure
5. Whiteboard on technical needs
6. Next steps and actions

**Attendees:**

- Wes Biggs (WB), Amplica Labs
- Constance Bommelaer de Leusse (CBL), McCourt Institute
- Wes Chow (WC), MIT Center for Constructive Communication
- David Clark (DC), MIT Research
- David Conrad (McCourt Institute invited observer)
- Harry Evans (HE), Amplica Labs
- Thomas Hardjono (TH), MIT Internet Trust Consortium
- Sandy Pentland (SP), MIT Connection Science
- Deb Roy (DR), MIT Center for Constructive Communication
- Wendy Seltzer (WS), Tucows
- Christian Tom (CT), McCourt Institute
- Sara Wedeman (SW), Behavioral Economics Consulting Group
- Braxton Woodham (BW), Amplica Labs

**Meeting Summary:**

- The meeting was called to order at 9:00am by CBL. The attendees introduced themselves and gave a brief background of their experience and affiliations.

- CBL shared context for the meeting
  - DSNP is being donated to Project Liberty to be under the stewardship of the McCourt Institute
  - Role of advisors is to set up structures that will strengthen the specification and foster its adoption

- BW gave historical background on the creation and development of DSNP
  - Acknowledgement that DSNP is currently under-documented
  - Context for scope, decomposition and timing
  - Evolution of concept of the Social Web
  - Three distinct phases are envisioned:
    - Social Identity—with connection to other identity providers
    - Data—public and private
    - Value—rewiring the attention economy
  - Current state and tactics
    - Ethereum evaluation led to development of Frequency L1 blockchain
    - MeWe partnership is a catalyst for Labs development workstreams
    - Introduction of Amplica Access launcher, a definancialized, custodial wallet (launching w/c April 24 at Consensus conference)
    - Future possibilities for a decentralized “app store” via the launcher

- The group held an open discussion on the approach and design of DSNP.
  - SP suggested having hooks to analyze changes in behavior in applications; BW agreed that application providers might be open to partnering; suggested SP connect with MeWe CEO
  - DR asked whether focus was on creating spaces for civic engagement or entertainment; HE answered that DSNP base layer allows different types of communities, with data usable across applications/environments. HE noted that group-related work is in development but not yet mature or part of the specification.
  - TH asked what mechanisms were contemplated to attempt to eliminate bots and paid actors; BW noted that attestation workstreams were focused on data enablement for this, but that moderation is seen as a layer above the core protocol.
  - SP asked if improving mental health and democracy were design goals; BW agreed these were important and noted workstreams with Georgetown University Ethics Lab would look at both the core technology and emergent behaviors.
  - DR noted studies his teams had developed to measure affective polarization on large social networks.
  - WC suggested that application provider stakeholders should be represented in the advisor group, BW agreed. SP suggested that a head of product/UX would be the right type of representative.
  - DC asked how current efforts had characterized value; from a “follow the money” perspective, or as social values. He suggested that a user pays model could enable a shift from advertising-based surveillance economy, which could still persist in a decentralized form. SP noted that an emerging alternative economic model is a community cooperative; UK, India and South Korea governments are looking at this approach. DR mentioned that public (taxpayer funded) services presents another model, and is being used for projects like Tim Berners-Lee’s SOLID. HE noted that initial Labs work on 3PI (privacy preserving provable interactions) was designed to enable subscription services as well as privacy-centric advertising-based ones.
  - SW noted that while privacy and its exploitation for economic gain is important, much bad behavior online has little to do with privacy, the recent US intelligence leak being an example of emotional incentives leading to undesired outcomes.
  - WC began a discussion on how to democratize who should run nodes on the blockchain. SP noted that cooperatives built 50% of internet infrastructure, so community-based organizations might be a viable option.
  - BW highlighted three types of sustainability that were desired: economic, cultural, and environmental (noting that the proof-of-stake blockchain consensus method was significant in helping the latter).

- WB and HE presented slides on the current status of DSNP, concluding with a diagram showing its position in the social web ecosystem and distinguishing the protocol from functionality that would be implemented at a service or application layer. This was interleaved with further discussion.
  - SP stressed the importance of being able to interrogate identities to detect bots and prevent different forms of Sybil attacks.
  - DC asked why the decision was made to put both the public and private social graph on the blockchain. HE noted that the application interaction model means users put trust in their tools and apps and can control their key sharing; BW summarized the delegation model in DSNP as the ability to “fire your agent”, and noted that storage on the blockchain was an important part of this “portability” story.
  - The ability to maintain multiple networks or graphs (different personae or facets of identity) was discussed. DSNP in its current form would require the user to maintain a separate social identity for each discrete graph. SW noted that usability and the user experience were important factors; several product examples (both positive and negative) were mentioned by participants.
  - SP noted that the ability to link a given identity back to a single source, with due process, was of keen interest to government actors, and that compatibility with official/NGO-operated identity services would be important for adoption, especially outside the western world. An action was suggested to capture a taxonomy of industries, government, etc. use cases with their expectations.
  - The group discussed how to allow for a marketplace of attestation and trust providers without the protocol/system becoming a kingmaker.
  - The advisors suggested that a chart of the different organizational entities heretofore involved be produced, particularly to understand the distinctions between for-profit and nonprofit structures.
  - SP asked how long-term decentralization could be achieved, and noted that local government involvement could provide a means toward this.

- The group opened a discussion on defining governance for the protocol.
  - BW proposed a series of phases: (1) centralized governance, as is currently the case; (2) credible independent structure; (3) scaled governance working with a larger organization.
  - CBL put forward several questions to take away and be prepared to discuss at the next meeting, including
    - What model do we want to use?
    - How can we best collaborate with other working groups?
    - What features are most important to capture in governance mechanisms?
  - BW noted that insight into public/private dynamics was welcome, as this would shape both processes and perceptions.
  - The group whiteboarded a set of success criteria for a governance structure, including
    - Credibility
    - Speed/urgency
    - Stakeholder voice
    - Trustworthiness (SW noted this had been defined as Competence, Beneficence, and Consistency)
    - Diversity
    - Political neutrality (examples such as Mozilla, Linux Foundations, as well as Brookings)
  - The group discussed how to ensure stakeholder voices were resistant to capture based on economic power. DC pointed to ICANN as a body where for-profit companies crowded out public interest; WS described W3C as a forum where all participants have equal votes, but implementers often have louder voices based on the reach of their platforms.
  - With respect to diversity criteria, participants were encouraged to come back with the axes they felt were most important (e.g. geography, business sector, etc.)
  - SP suggested it is important to have non-Western-centric participants, for example following the Indian NGO model. A discussion followed on the limits of decentralization when operating under different regimes, and whether federation of multiple DSNP systems allowing for varying levels of state/LEO access might be an option.
  - Communication channels for work going forward were proposed. DC cautioned against breaking into working groups too quickly and suggested the group work as a committee of a whole at this stage. CBL took an action to set up a mailing list for participants.

- After a lunch break, the group began a further discussion on technology decisions and directions.
  - An action was taken to document on-chain vs. off-chain data distinctions following a discussion on the importance of data locality for political/regulatory purposes.
  - WS asked whether the protocol should address bad actors or be neutral to usage. The group discussed that there might be a distinction between what is expressed in the protocol, and what is in scope for the group sponsoring the protocol.
  - DR asked how data migration works for users coming to DSNP. HE explained the concept of a “reconnection list” that could be used to facilitate migration of relationships from Web2 providers.
  - The group discussed key management and the logistics of key rotation. It was noted that the nature of trust relationships with shared providers introduced the group key management problem, making perfect forward privacy problematic. It was noted that it is an open question whether key management is in the domain of the specification, or if it should sit with blockchains/wallets.
  - DC requested a brief on how the Polkadot parachain ecosystem works, and the definitions of Level 0/1/2 blockchains.
  - WC asked if a bad actor could consume all resources (if sufficiently funded). HE noted that the Frequency model uses staking for capacity, which provides some defense against this. BW used this opportunity to encourage participants to recruit additional collators to the system to improve its resilience.
  - TH asked about published specifications. HE noted that specs are already public on spec.dsnp.org, while agreeing that further narrative alongside the technical details was needed.
  - DC asked how groups would work. HE said groups were still being defined, but were envisioned to allow for both public and private formats. WC discussed the usefulness of group identities being publicly uncorrelated with real-world identities, but such correlation being privately provable. HE noted that another aspect of group metadata is whether moderation is done preemptively (admin approval), post-hoc, or not at all. DC suggested a smart contract model might allow for evolution of these options without spec changes. TH proposed looking at a more formal calculus of access control to arrive at a working model; DR noted that most successful real-world projects purposely simplified these structures to avoid loops.

- A second round of questions and discussion on governance followed, laying out some further topics to return to in the next session.
  - WS asked which level should be the initial focus of the group: (1) change control of the spec, or (2) ecosystem governance. BW asked the further question of whether governance should extend beyond the DSNP box to (3) governance for the Social Web generally?
  - SP queried if LLMs were an immediate concern in a social media context. BW said moderation had been considered an option for this but is seen as more of a service/application-layer concern. He suggested that Project Liberty grants could have an impact in shaping this.
  - WS suggested the group create a statement of scope and charter for work as a next step.
  - DR noted the distinction between advisors and directors and that the group should define who actually pushes spec changes.

- BW introduced a brief conversation about universal handles for social identities, and noted that Labs had done some work toward this with MeWe, but not yet within the scope of the DSNP spec.
  - WC noted the difference between uniqueness and discoverability. SP asked if there was the ability to have identity not be publicly discoverable, but personae be discoverable. HE related that Labs found that when using a facet/persona-based approach, it was difficult to avoid correlatibility between personae. TH suggested looking at ABC4Trust, an attribute-based encryption system targeting similar use cases. DC proposed the group look at identity escrow, whereby an identity could be proved to correspond to a unique individual without revealing precisely who the person is.

- In the final session, each participant was asked to summarize their key takeaways, directions, and actions from the day.
  - TH and several other participants requested that Labs provide further documentation of the rationale behind technical decisions that have been taken.
  - SW thought the session was very positive. She suggested that future in-person meetings be formatted to provide more movement and variety.
  - CBL agreed that a lot of work had been accomplished, and suggested the group think about the most effective way to tackle the upcoming work.
  - DC suggested he would follow up with a written dialogue to clarify points and ensure that his understanding was correct on certain technical points, which was welcomed by Labs staff. He also requested that a competitive analysis be provided for discussion at the next meeting.
  - SP stressed the importance of thinking about the worldwide context of social media and the need for secure non-anonymous spaces.
  - DR commented that while the high-level vision for the Social Web and low-level spec for DSNP were relatively clear, the modules in between that were needed to address the challenges and solve the problems perceived were more murky. He suggested that user stories be fleshed out to better illustrate what can and can’t be addressed.
  - WB asked how the group could best be set up to succeed at fostering the DSNP specification itself, while bringing its members’ multidisciplinary backgrounds to also tackle some of the higher-level issues.
  - HE said he appreciated the opportunity to broaden the conversation and noted the action to produce further documentation.
  - BW expressed his understanding of DSNP with regard to the power dynamics of the current state of the web, and noted that DSNP aims to pull the network effect back into the network itself. With respect to documentation, he noted that Project Liberty resources will be required.
  - WC appreciated that a lot of ground was covered, and was curious to see how the group’s advice would be implemented.
  - CT brought up the motto of PL to “fix the internet” as overly broad in this context and suggested the group focus on creating a simple and understandable message that could work in an ELI5 (Explain it Like I’m 5) format.

- The meeting closed with tentatively scheduling the next virtual and in-person meetings, 3 and 6 weeks out respectively. CT will serve as point of contact and coordinator for next steps.
- The meeting concluded at 5:00 pm.

_Minuted by WB_
