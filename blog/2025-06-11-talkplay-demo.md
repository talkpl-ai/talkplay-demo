# Demoing TalkPlay: An LLM for Music Recommendation at NY MusicTech Meetup

I had a blast presenting [TalkPlay](https://talkpl.ai) at the [NY MusicTech Meetup](https://www.meetup.com/music-techster/) back in March. It was one of those presentations where everything clicked – engaging audience, great questions, and super fun. For those who missed it, the amazing organizer and volunteers recorded the whole thing:

<iframe width="560" height="315" src="https://www.youtube.com/embed/pgevqDNIIqM?si=3cCO19qbM853jUMt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Fair warning: it's got that authentic demo energy where things are live, real, and sometimes a bit messy – exactly how I like it!

# What is [TalkPlay](https://talkpl.ai)?

TalkPlay is, simply put, an LLM specifically trained for music recommendation. But let me back up and explain *why* this matters.

If you've ever tried asking ChatGPT or Claude for music recommendations, you've probably noticed some... issues. First, they have knowledge cutoffs, so you're getting recommendations from years ago. Second, they're biased toward super popular music because that's what dominates their training data. And third – perhaps most importantly for anyone thinking about building actual music products – they're completely disconnected from real music databases.

So while general LLMs can work as conversational interfaces, I wanted to leverage their knowledge base more directly for music recommendation. TalkPlay is essentially an LLM that's connected to a music database and specifically trained to recommend music based on natural language queries.

# The Demo: Highlights and Happy Accidents

During the live demo, I showed off several examples that I think really captured what makes TalkPlay interesting:

## Classic Heavy Metal
When I queried "classic heavy metal," the model provided different recommendations each time – sometimes obvious choices, sometimes unexpected gems. This variability is actually a feature, not a bug! Unlike traditional recommendation systems that might always return the same top-N results, TalkPlay can surprise you.

## Cross-Language Understanding
One of my favorite moments was when I demonstrated non-English queries. TalkPlay responded in English but sometimes recommended Spanish songs, showing it had some understanding of the user's language context. Ideally TalkPlay would respond in Spanish; but thinking about how it responded, now I have an idea to make it happened in TalkPlay 2, without languag-specific datasets.

## Multi-Turn Conversations
The model showed it could maintain context across conversation turns, refining recommendations based on follow-up questions about specific genres. This conversational aspect is where I think music recommendation really needs to go – it should feel like talking to a knowledgeable friend, not querying a database.

# Some Failures

Ok, this isn't a sugarcoating zone! The demo had its failure cases, and I made sure to show them. There were moments where the model recommended songs from completely different genres than requested. Sometimes the descriptions didn't match the actual songs because of how the response generation works.

These failures are important to acknowledge because they show where we still have work to do. Perfect recommendation systems don't exist, and I'd rather be transparent about limitations than oversell the technology.

# Looking Forward

TalkPlay was a research project I co-authored with Dr. Seungheon Doh, and while we've moved on to other things professionally, I'm still excited about the possibilities it represents. Music recommendation is ripe for innovation, and I think conversational, multimodal approaches like this will play a big role in how we discover music in the future.

---

Huge thanks to the organizers at NY MusicTech Meetup for having me, and especially to DJ for editing the video and adding captions – that made it so much more accessible for everyone. If you're in the NYC area and interested in music technology, you have my recommendation for this meetup by Seth Hillinger. Check them out at [nymusictech.com](https://www.meetup.com/music-techster/) and follow [@musictechster](https://twitter.com/musictechster).


PS. This is cross-posted to [my blog](https://keunwoochoi.github.io/post.html?id=2025-06-11-talkplay-demo).