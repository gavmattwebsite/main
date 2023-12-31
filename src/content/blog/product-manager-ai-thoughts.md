---
title: "A Product Manager's Thoughts on AI in 2023"
description: "A year of insanity in generative AI, in retrospect"
pubDate: "Jan 03 2024"
heroImage: "https://res.cloudinary.com/draaqu0o9/image/upload/f_auto,q_auto/v1/AI/icxivoqucx9hnzjgf61v"
tags: ["AI", "Work", "Technology"]
---
<i>Content by Gavin, images by boops and beeps</i>

Don't you love that 90s Matrix-style hero image?

With the close of 2023’s explosive year of AI, I thought it would be good to spend some time sharing my thoughts on where we are with generative AI and what I think is on the horizon.

Disclaimer: I sit somewhere between skeptic and evangelist. Like any new technology, we should be skeptical of the hype and first wave of ideation, but there are many paths that generative AI can take that I think could provide massive benefits to certain people. I’m a Product Manager working in a space deeply interested in AI, and as such, do my best to keep an objective eye on the current and future market. 

Likewise, this isn't comprehensive, and doesn't go deep on all of the other pros and cons with AI, instead sticking close to technology and content. Write your own blog!

<h2>A 2023 recap</h2>

How did we get here? This isn’t a timeline of when OpenAI was founded or the famous dinner with Sam Altman, Elon Musk, Greg Brockman, and others. It isn’t a brief on the differences between ChatGPT 3.5 and 4. This isn’t a debate over “AI” versus “Planned Intelligence” versus "ML." Instead, I want to give a take on what we experienced last year from someone in the trenches of integrating.

Early in 2023, we saw a seemingly sudden explosion in the *accessibility* and *ability* of AI for the masses. The topic isn’t new at all, but for the general public (and most product teams), spring 2023 was a shock. This wave of course came via the GA release of ChatGPT-4, but specifically in the notable groundswell of fly by night projects and startups that spun off of the new APIs. If you were there working in any form of product or engineering role, you could feel the schism - one day AI was inaccessible, and literally the next, you were rewriting roadmaps and updating strategies.

The first phase was novelty. These are the days of AI jailbreaks (favorites: Grandma comes in clutch to share her [famous napalm recipe](https://kotaku.com/chatgpt-ai-discord-clyde-chatbot-exploit-jailbreak-1850352678) and [captcha breaking tips](https://arstechnica.com/information-technology/2023/10/sob-story-about-dead-grandma-tricks-microsoft-ai-into-solving-captcha/)), generating horrendously goofy images via Midjourney or DALL-E 2, and playing with chatbots and wrappers that showed off hints of what AI could do. If you want a proxy, check out ChatGPT [references on Hacker News](https://hn.algolia.com/?dateRange=pastYear&page=0&prefix=false&query=chatgpt&sort=byPopularity&type=story) and the volume of comments - many of the top stories over the previous year are directly about OpenAI product launches, lawsuits, and ShowHN apps and startups built on ChatGPT, LLaMa, and other models. 

I had the honor to work on several very useful integrations to OpenAI built on these tools - namely Contentful’s [AI Content Generator](https://www.contentful.com/marketplace/app/ai-content-generator/) and [AI Image Generator](https://www.contentful.com/marketplace/app/ai-image-generator/) - and found that content teams in particular benefit directly from AI...if used correctly. At the same time, there were (and are) massive warning signs about how these technologies could be misused and disrespected. This tipped me off early to some of the cons and pros of AI, specifically in the world I work in - content management.

<h2>Responsible, ethical, and useful AI</h2>

What became immediately clear when using these tools is that standard controls were not part of the original formula. Not discounting the biased and limited training data for any given model, flaws immediately appeared in how AI models broadly present information as fact and how AI generated content cannot be sourced or flagged downstream. Let’s use an example.

Say you’re working on a research project, maybe generating competitive intelligence about another product. You write a basic prompt that seems on the surface to be relatively solid:

> You are generating competitive intelligence about Brand X, comparing their products and pricing to Brand Y. Generate 10 bullet points about how Brand X and Brand Y compare and contrast and make a recommendation about which brand you think is better.

This prompt appears to work. No matter what model you use, you will get back an apparently accurate read of the competitive landscape with detailed bullets and supposedly factual statements. Satisfied, you then bring this analysis into your day job and operate off of the assumptions it creates.

*Notice what’s missing?*

The most clear and present issue is the complete lack of attribution. Because we don’t know the training data or the source of a given “fact,” we don’t know if the data has any basis in truth. These are called [hallucinations](https://www.tomshardware.com/news/ai-hallucinations-ranked-chatgpt-best), and while sometimes hilarious, mean that responses can inherently feature blatant lies *by virtue of using the product*. We may think that a given competitive differentiator came from Brand X’s pricing page, what if it actually came from a hit piece created by Brand Y or Z? What if the source provided by the model is simply nonexistent or misattributed? The idea of getting gaslit by a bot is some real dystopian nonsense.

The problem isn’t even on the end user - they literally often lack the tools to even do basic verification of the source.

The second issue is that once this data enters a project, your own editorial process becomes extremely difficult. As an editor, you are now responsible for reviewing work that may or may not be AI generated. You must assume that any work you review will mix human and AI constantly, even if it includes sources. The end result is that you actually spend *more* time editing, because you not only need to edit for voice and tone across the content, but also validate the information and track sources for it. Since anyone can use any number of tools to generate content (including a [car dealership chatbot](https://venturebeat.com/ai/a-chevy-for-1-car-dealer-chatbots-show-perils-of-ai-for-customer-service/)!), we’ve now entered a world where we can never really track when AI is used. There is no universal flagging standard or any viable tool to detect AI generated content, and that means that every piece of content must now unfortunately be treated as generative and suspect. This can be avoided with tight controls in your content creation process, but things slip through the cracks.

This is horrible. I’m not someone who thinks that content should be solely human generated, but with the low level of quality we currently see from the default prose and copy that AI generates, we’re in for a truly mundane world of generic marketing. Content **can** be dialed in through very strong prompts, brand profiles, and good editing, but can that happen at scale? 

I had the chance to pair with experts in the field like [Alaura Weaver at Writer](https://www.contentful.com/blog/responsible-ai-begins-with-robust-policies-for-teams-using-ai-technologies/) on how companies could approach ethics and quality when using AI, but it still leaves the outstanding question - can we ever track and contain this, or is the game up?

Even worse, these models don't respect character limits and will willfully gaslight you into believing a 65 character sentence is below 50 characters... 

<h2>The positives</h2>

Putting aside the possible doom of a generic content future, there are some extremely strong upsides to AI in my view. This is controversial: AI is a boon to creativity if used right. That’s a huge if, and I understand the fear in fellow creators around AI replacing art if used irresponsibly. That being said, if used responsibly on the local level, AI can support many aspects of the creative process. 

AI is a nifty gift for the blank page problem. Sometimes the hardest part of starting a project is exactly that - starting it! You may need just a line or two, a bad base image, or a list of topics to go from procrastination and writer’s block to a finished project. Once you have this start, you can abandon AI and go back to human creation. Creativity isn’t a commodity and we shouldn’t necessarily prioritize speed, but breaking through the initial block can lead to a windfall of new ideas.

I also personally love AI for general content accessibility. What I mean here is localized content and experiences. AI still doesn’t replace humans when it comes to localizing an experience with actual empathy for the end user, but it can go a long way to allowing you to create an experience that at least acknowledges different languages and users. ChatGPT and DeepL translations are pretty solid, and using them to provide base-level localization is a nice touch.

Image generation is catching up, but still provides for a great laugh. So many images end up smack in the middle of the uncanny valley or totally miss the intent, creating a new form of pseudo glitch art. I keep a personal gallery of my worst of the worst:

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/ie20mvev7ymmfbnv5dto" alt="A bad AI generated image of a beach with a mountain and yetis in the background">

<div align="center" style="padding-bottom:15px"><i>Add a huge mountain with snow and Yetis to this beach scene</i></div>

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/owi1n5cka15f3zwz81oq" alt="A bad AI generated image of a beach with an illegible word floating in the ocean">

<div align="center" style="padding-bottom:15px"><i>Add a portal into a forest world in a photorealistic style with trees and misty border</i></div>

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/rq7myptpjtf3ztdobh3u" alt="An AI generated image of a family having fun on a beach">

<div align="center" style="padding-bottom:15px"><i>Family with kids having fun on the beach</i></div>

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/k9incfaga43c1pwqg7pp" alt="An AI generated image of an okra cartoon mascot">

<div align="center" style="padding-bottom:15px"><i>A cartoon mascot of okra</i></div>


That being said, I did find a hack somewhere online that still works if you need sharp, workable images. The trick is to be incredibly, incredibly specific, down to listing a specific camera body and aperture:

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/qhxy130ftfmbekf2rzsy" alt="A hyperrealistic AI generated image of a giraffe">

<div align="center" style="padding-bottom:15px"><i>A realistic photograph of a giraffe at a zoo, sharp, black and white, Hasselblad camera, f4, 150mm, natural lighting</i></div>

<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/tgtckm6ypse14ahvfixd" alt="An AI generated image of a shrimp swimming with okra slices">

<div align="center" style="padding-bottom:15px"><i>Photorealistic okra in water, shrimp, sharp</i></div>


<img src="https://res.cloudinary.com/draaqu0o9/image/upload/w_600/f_auto/q_auto:best/v1/AI/sksqjx0ssosi4ncvkpf8" alt="An AI generated image of a denim jacket with a smiley face patch">

<div align="center" style="padding-bottom:15px"><i>A realistic photograph of a modern denim jacket, up close, sharp, embroidered smiley face patch on neck, Hasselblad camera, f4, 150mm, natural lighting</i></div>


<h2>Looking forward</h2>

I think 2024 and beyond will be a stronger year for practical generative AI. It’s not to say that what we have today isn’t practical, but it’s clearly the MVP before the real product. I expect a lot of consolidation, (unfortunately) a lot of forgotten companies, and AI addressing more complex needs. Inevitably, I see AI becoming a really sticky new foundation for how we build technology, and a requirement for how we think about structuring data. I predict a lot of 3 year strategies and pitches will need to not just contain the phrase “AI,” but actually be required to show and prove an intentional plan to make their product compatible with, extensible to, and designed/architected for AI.

My 2024 predictions include:

**Chat/support** - please go beyond the standard “use ChatGPT to poorly answer my question” and instead actually solve it. Why should you ask a chatbot how to return something, when it knows how to actually handle returns? Chatbots trained on the right data that wrap APIs or even integrate to external products are going to be a goldmine. I’ve seen several extremely promising startups moving exactly in this direction.

**Pervasive AI images** - AI generated ads and social images are already widespread, but I expect that the general availability of DALL-E 3 and similar products will usher in an exponentially more widespread use of AI for images of all types. The real breakthrough is reliably generating readable text in AI generated images. That unlocks AI for fully visual ads, and is set to dramatically reshape marketing (again).

**Gemini market share explosion** - The introduction of [Google's Gemini](https://blog.google/technology/ai/google-gemini-ai/) late last year promises a real viable alternative to GPT-4, and I’m here for it. It remains to be seen how it performs when actually put to real-world 3rd party tests, but the early benchmarks seem promising. This isn’t to say that one needs to be “better” than another. We just need more competition.

**More snafus** - like any technology, ChatGPT and others are hitting the mainstream and are constantly being jailbroken or abused (as they should be). The lack of tight controls and even basic thought around response handling will lead to even more cars sold for $1 and recipe generators producing dangerous concoctions. At least it’s easy enough to spot the garbage - look for “certainly!” or “as a large language model” as signs that you’re just speaking to raw ChatGPT.

**AI architecture** - I expect more emergent and nimble companies to factor AI into how they structure their data and backend. I don’t mean “how can we integrate OpenAI into our database” style planning. Instead, think “how can I ensure the data I collect and store is structured and useful for training?” Or “are we extensible enough to interact with a variety of foundational models?” If you buy that this era of AI is sticky, you have to also buy that architectures will need to be prepared for it by design.

**More focus on hallucinations and trust** - hallucination reduction is a natural target in 2024. There are a handful of great methods to reduce hallucinations that I expect will be used more by vendors to make targeted reductions to inaccurate information. Likewise, more open source models trained on more niche data will improve accuracy for specific usecases like enterprise search.


What’s your favorite use of AI last year? Are you excited, worried, skeptical, or eating popcorn on the sidelines? 