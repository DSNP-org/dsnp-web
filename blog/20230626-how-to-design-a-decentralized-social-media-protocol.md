# How to Design a Decentralized Social Media Protocol – Be Ruthless About Technical Requirements and Eager to Build Coalition

*By Constance de Leusse, Executive Director of Project Liberty’s McCourt Institute*

Project Liberty’s Institute sat down with Dave Clark, an early contributor to the TCP/IP protocols that built and run the Internet, and one of the expert advisors on DSNP, the Decentralized Social Networking Protocol.

---

## You’ve been involved in networking since the early days of the Internet. Can you tell us about your book ‘Designing an Internet’?

The book’s called ‘Designing _an_ Internet’ because there are many possible ways to do this. It’s about making choices, but if you do an undergrad class in networking, they just give you a pile of facts about what TCP/IP headers look like. Anyone can look up facts. Networking is a design discipline. Computer scientists are awkward about saying it’s a design discipline, not fundamental facts derived from science. We should teach design.

In 1975 we had some idea of the basic function of the network we wanted to accomplish. It was just about getting data from one point to another. By the 1980s, new people would come in and say, ‘Why can’t we do x?’ We had to get clear about our requirements and priorities. Functionality is key.

The Internet Protocol didn’t succeed because it was intrinsically better than the competitors, though we thought it was. There were forks in the road where we could have lost to IBM, the OSI, even Xerox. We spent the 1990s engineering new features into the internet—like Quality of Service to deal with jitter. We had to go head to head on functionality to win in the marketplace.

## Can you talk about TCP/IP and dividing up network functionality?

The design principle of the Internet is to push functions out of the network and implement them in the end nodes. That’s the end-to-end principle. The Internet Protocol (IP) just tells routers how to forward packets. The Transmission Control Protocol (TCP) is implemented in the end nodes, and has a more complex set of responsibilities. Only the end nodes look inside the packets. (That’s changing now, with deep packet inspection, but you get the idea.) It’s a layered design. You can innovate independently in each layer and build functionality onto the network because it is not in the network. We split TCP and IP in half. Any function you could avoid putting in the routers, avoid it. The less you put in the IP, the more general the platform and the more innovation you’ve empowered.

## So where does DSNP fit?

DSNP uses the Internet as a transport like everything else does, for example, SMTP, the protocol that supports email. That’s the power of modularity. It sits on top. Layering is a modularity assertion that says I’m sitting on top of you. I depend on your correct operation, but you don’t depend on mine. If an app screws up, it should just break the app, not the internet. The modularity is pretty clean. You get a layer cake of functionality.

## Why create a protocol for decentralized social media?

Two fundamental hypotheses motivate the development of DSNP. First, there’s a lot of resistance to the power that the operators of large centralized platforms have acquired. The Internet itself is distributed. There are seventy thousand autonomous systems that make up the Internet, but the application platforms are essentially all under centralized control. This distresses people worried about the concentration of power, like Shoshanna Zuboff, who wrote ‘Surveillance Capitalism.’ I agree. So, can we come up with a decentralized way to build a competitor to the significant apps of today? Can we build a decentralized solution that succeeds in the marketplace?

Secondly, the big social media apps are being used for incredibly destructive purposes. How can you build a system that encourages benign human behaviour and discourages malign behaviour? And can you do that in a decentralized system? I think you can, but that is the challenge.

## You’ve worked on the technical protocols that changed the world. What does a protocol need to gain traction?

Functionality, finding your collaborators, building the coalition. It’s a brutal marketplace. You need a ruthless self-criticism of your requirement priorities and to understand how services can compete on your platform. What is the feature set incumbents offer that consumers want to see? Build that, then go to them and say, ‘This is a better solution’.

## What does DSNP offer?

DSNP allows me to record certain facts, such as who I choose to follow on social media, in a publicly accessible way. It’s writing the social graph to the blockchain. That information can be encrypted, and I’m the only person who can decrypt it. Because it is external to any particular app, I can use it to move to a new app with a user interface or moderation system that I prefer. Also, if I use a bunch of different social media apps, I want something to talk to all of them. DSNP will let me do that, though the definition of ‘friend’ or ‘follower’ is different from Facebook to LinkedIn, so DSNP supports different kinds of relationships.

## Why did you get involved in DSNP?

Frank McCourt just put his head around my office door and asked me to be involved in the project. There was real passion and sufficient support that the project won’t just run into a hole. It’s a really exciting place to play, to learn about the modularity of this app experience. I’m especially interested in how DSNP can disincentivize malign behaviour on social media. The starting point is the pernicious effect of an advertising-based economy. Facebook sends out false and damaging content because that’s what makes people more sticky. They show you more ads. They work out the ARPU. With DSNP, people might be able to choose to buy an app at $5 a month that doesn’t preferentially send misinformation or ads. Then again, some people like that. If you gave the Fox News crowd a choice, would they still pick outrage?

## What does success for the DSNP look like?

Market share. You have to think about that as a problem of marketing, which starts with being ruthless about your requirements and functionality.

It’s also about collaboration. Wikipedia has thirty entries of people doing decentralized social media. So, you go through them and see ‘Who can I form a coalition with?’ And you look at the app builders on top. Why are the best ones succeeding? What’s their modularity?

Cool features and economics come in here, in the end. What do users use to pick? Features. And different people want different features. My forty-year old son is a Discord fan. It’s a gamers’ platform. He was trying to get my wife to use it. The blinking cat made her crazy. Gamers love it. Other users do not. It’s an iterative process to figure out the cool features that people will want. If you get it right, app designers can innovate at the edges. You allocate function in a modular way, like how TCP/IP split what goes into the router and what goes into the end device.

There’s still a conversation about the modularity that best fits DSNP, what gets defined and what’s left for innovation. Modularity means you open up clear space for people to innovate, just like the original Internet design principle. That’s how you win.

## What are the three most important things for DSNP to do in the next year?

Find your collaborators. Develop a marketing strategy. Be ruthless in analyzing requirements. And maintain clarity of scope—don’t boil the ocean. It’s all about choices. Be able to say what you’re not doing.

## We started by talking about a book, so let’s finish that way. What’s something you’re reading right now?

I enjoy escapist science fiction and just re-read the Harry Dresden books by James Butcher. The series starts a little slow but is great by a few books in. I recently read ‘Sociological Theory for Digital Society: The Codes that Bind Us Together’ by Ori Schwarz. It’s about how sociology is being changed by technology. I love reading books from folks that have a totally different perspective than I do.

---

Dave Clark is Senior Research Scientist at MIT’s Computer Science and Artificial Intelligence Laboratory (CSAIL) and Fellow of the National Academy of Engineering and the American Academy of Arts and Sciences. Previously he was chief protocol architect of the precursor body to the Internet Architecture Board, and chairman of the Computer Science and Telecommunications Board of the National Academies. His book, ‘Designing an Internet,’ is published by MIT Press and won the 2019 Prose Award in the History of Science, Technology and Medicine category.
