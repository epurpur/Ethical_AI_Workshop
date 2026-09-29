# Ethical AI Use Workshop

```
Last updated 09/29/26
```

Erich Purpur

    Research Librarian for Science & Engineering
    epurpur@virginia.edu
    

These workshops are offered by [research data services](https://data.library.virginia.edu/) in the UVA Libraries. Research Data Services does these things:
    
1. Find and Manage Data
2. Data Analysis & Visualization
3. Workshops & Trainings (Like this one!)
4. Free Statistics & Technical Consultations in the [StatLab](https://library.virginia.edu/data/statlab)

## StatLab
* [StatLab](https://library.virginia.edu/data/statlab)
The UVA Library StatLab provides free statistics & similar technical consulting to students, faculty, staff at UVA


## Upcoming Workshops

| Workshop | Date | Time |
| ---- | ---- | ---- |
| Intro to Python pt 1                                                |       Tuesday 9/1   |  11:00am - 12:30pm
| Intro to Python pt 2                                                |       Friday  9/4   |  11:00am - 12:30pm
| Local Large (and small) Language Models                             |       Tuesday 9/8   |  11:00am - 12:30pm
| Vibe Coding & AI Agents                                             |       Tuesday 9/15  |  11:00am - 12:30pm
| AI and Model Context Protocol                                       |       Tuesday 9/22  |  11:00am - 12:30pm
| Ethical AI Use & Best Practices                                     |       Tuesday 9/29  |  11:00am - 12:30pm

----------------------------------------------------------------------------------------------------

## AI Disclosure
I used AI, mostly Claude, to help point me to various links and other external resources I used to verify the points I am making throughout this workshop. 

## Ethics 
To judge whether or not AI use is ethical, we should at least pause on what are ethics in the first place? [According to the dictionary definition](https://www.britannica.com/topic/ethics-philosophy), ethics are the discipline concerned with what is morally good and bad or right and wrong. The term is also applied to any system or theory of moral values or principles. Ethics can be personal or societal. You can adopt a code of ethics that in not necessarily the same as what society at large agrees with.

## Current State of Things
This is just my interpretation.

The current paradigm around AI is that you are either with it or you'll be left behind. Today, various tech giants like Meta, X, Anthropic, OpenAI are in an arms race to develop tools to re-imagine every aspect of our lives and make billions in the process, leaving normal people in the wake as collateral damage. This is widening the gulf between the haves and the have nots as AI eliminates jobs and divides us along political lines. A quick google search of "ethical AI use" will deliver the promises of [IBM](https://www.ibm.com/products/watsonx-governance) and [Accenture](https://www.accenture.com/en/services/ai-data). Anthropic's Claude purports to be the "ethical AI" and has even [written a constitution](https://www.anthropic.com/constitution) explaining their vision. In the constitution is a section on "Being Broadly Ethical" and states that <i>Our central aspiration is for Claude to be a genuinely good, wise, and virtuous agent.</i> How nice of Anthropic for looking out for their users!

UVA at the institutional level is delivering the message to get on board with AI. While there are plenty of individual skeptics among the ranks of faculty, staff, and students, for the higher-ups it seems that AI is the future. I try not to be too cynical. AI has its positives too. It makes my life easier every day. But at what cost? Do the downsides outweigh the upsides?

**Evolution of underlying technology**
Despite all the controversy that AI has come to represent, the technology today is interesting and is the product of an evolutionary process dating back to the 1950s. In 1954, Georgetown University exhibited a primitive machine learning system which translated between English and Russian phrases. In 1966, MIT professor Joseph Weizenbaum created the first Chatbot ([ELIZA](https://en.wikipedia.org/wiki/ELIZA)), which mimicked human behavior based on natural language prompts. Technologies such as Natural Language Processing (NLP), Machine Learning, and Neural Networks have all evolved over time to the point where they are today. Hardware and data storage evolved along with them. To the general public, AI first dropped in 2022 with ChatGPT, but that is far from the truth. These systems have taken decades to develop.  

**Environmental Impact**
To put it simply, AI and its associated technologies take a huge toll on the environment and the earth. "Cloud Computing" is a myth. The cloud is really a server farm somewhere, maybe Northern Virginia, in a massive data center used for various purposes, including providing the computing power to train large language models. Huge amounts of water are needed to cool the data centers, thus using this valuable resource. Tech companies are being granted tax exemptions by local politicians whose votes are being bought. On top of all that, the raw materials needed to manufacture the hardware needed in the LLM-training process such as Graphics Processing Units (GPUs), are being extracted from the earth and ruining fragile environments in the process. Unfortunately it seems inevitable that this will continue and contribute to the exacerbated increase in global warming leading to the eventual heat death of the planet. 

**Is Ethical Use of AI Even possible?**
I will let you be the judge.

**Follow up: Is there a difference between ethics and morals?**
Can AI use be ethical but not moral or vice versa?

## Everyday best practices
Whether or not AI use is ethical, there are some things you can look for in order to trust an AI system more.

**Fairness:** Is this model fair towards all? In particular already marginalized groups. Bias occurs when algorithms produce prejudiced or unfair results that favor or discriminate against specific groups of people. This point is particularly hard to overcome as LLMs typically model historical human choices that encode past discrimination or stereotypes.
- [Anthropic Model System Cards](https://www.anthropic.com/system-cards) - For some of Anthropic's latest models as of September 2026 ([Fable 5.1 and Mythos 5.1](https://www-cdn.anthropic.com/0339e6a7c5c7b87f5c07798616dc32c215d14235/Claude%20Fable%205.1%20&%20Claude%20Mythos%205.1%20System%20Card.pdf)) Section 4 (p.59) *Safeguards and harmlessness* addresses this an also references [Anthropic's Usage Policy](https://www.anthropic.com/legal/aup). This section features information on the harmfulness of the model's responses and also how often the model refuses to answer sensitive subjects. They've also tested it across longer conversations instead of one exchange.
- [Meta System Cards](https://ai.meta.com/tools/system-cards/) - Categorizes models into difference use cases
- [Open AI GPT 5.5 Sytem Card](https://openai.com/index/gpt-5-5-system-card/) - Could not find comprehensive list of cards for all AI models so here is one specifically for GPT 5.5 

**Explainable:** Is there documentation about the provenance of the data? Provenance refers to the place of origin or history of an item. This is a big topic in libraries as we are concerned with capturing metadata about items in our collections. You might also hear about provenance of a work of art. This means who it was created by, who owned it, what museums was it in, etc. Data provenance for LLMs let users trace an AI answer back to the source data the model was trained on. It should also tell you where the data came from, how it was modified, and who handled the data. 
- Taken from the system card for Claude's Opus 5 model: <i>"Claude Opus 5.5 was trained on a proprietary mix of publicly available information from the internet, public and private datasets, user data included in feedback or bugs or which users have explicitly permitted for training, and other sources, such as synthetic data generated by other models."</i> They are not going to tell you exactly what is in the training data.
- [OLMo](https://huggingface.co/allenai/OLMo-7B) is considered a <i>"gold standard"</i> example of LLMs for which all code, checkpoints, logs, details are documented. This includes the pre-training data. **Side Note:** the link above is to the HuggingFace page for these models. HuggingFace is a platform which hosts many LLMs, both open and proprietary. They are available for download and accompanying documentation is provided. 

**Robustness:** This is a point that is hard to verify from an outside perspective. Unlike fairness or privacy, there is rarely a document to read. This makes sense if you think about it. Would a tech company tell you what are the ways in which to attack their LLM or AI system? This remains internal to a company or developer. Not all points under the robustness umbrella are security risks. The industry tries to <i>red-team</i>, a practice of testing security threats to their system preemptively before attackers do. Here are some points about robustness of a system. 
- Does the system give consistent answers to similar questions?
- Is it resilient to noisy or malformed input? Can it interpret your mess?
- Can someone deliberately craft an input to make it misbehave, pass safety filters, leak its system prompt, or execute unauthorized actions?
- Does it protect against security attacks? Especially in agentic setups where the model can take real actions?

**Transparency:** It should be clearly indicated when AI is making a decision and this is one of the more legally concrete tenets of these best practices. Though the law around AI use is still being formed, AI disclosure has been written into various states' laws. There are many many AI laws and lawsuits going on currently. These are just 2 examples. 
- [California SB 243:](https://calmatters.digitaldemocracy.org/bills/ca_202520260sb243) Effective Jan 1, 2026, chatbot operators are to provide clear and conspicuous notice that the chatbot is AI and not human and to disclose the AI identity at the start of a session and at defined intervals. This applies to California AI users, not California-based companies. Any company that operates an AI service in California must comply. 
- At home, Virginia came within one signature of being the second state (after Colorado) with a comprehensive AI law which would have required businesses using AI in high-risk decisions, such as determining your college admission acceptance or home insurance rate, to exercise care to prevent algorithmic discrimination. [Governor Glenn Youngkin](https://ogletree.com/insights-resources/blog-posts/virginia-governor-vetoes-artificial-intelligence-bill-hb-2094-what-the-veto-means-for-businesses/) vetoed it citing concerns about innovation and compliance costs.

Legalities aside, here are a few best practices in everyday life that translate to concrete, actionable questions.
- Does a product tell you, unprompted, that you are talking to an AI? Look for that disclosure. 
- If a decision affects you, such as a job hiring decision, does the platform you are interacting with specify the name of a tool and how to request a human review? If it doesn't you are entitled to ask for that in a growing number of jurisdictions, according to law.
- As an individual, if using AI in your own work, pick your disclosure rule <i>before</i> you need it. You'll notice I disclosed my AI use at the beginning of this workshop. 

**Privacy:** How is your data being used?
- When using many AI systems, your personal information, chat history, interactions are all being used against you for various purposes. Those purposes could be for training data for future AI use, selling your data for marketing purposes, surveillance, etc. An AI system should have a stated data privacy policy about where and how personally identifying information is being collected. Assume the worst!

## A few other daily practices
It seems like a lot to check all this stuff in real life. Probably what you want is a way to use AI but not actively participate in the heat-death of the earth. I wish it was as easy as pointing you towards the *right* tool to use and all would be well. Unfortunately it is not so simple!

**Do you really need it in the first place?**
- AI use is meant to supplement human thought processes, not replace them. First you should consider if AI use is necessary for this task in the first place? Less AI use is probably good for the world!

**Disclose your own AI use**- Take it upon yourself to create your own AI disclosure policy and use it in your work where you see fit. You can also include a statement about NOT using AI!
- [University of Waterloo](https://aidframework.org/): Librarian Kari Weaver created the AID framework for crafting your own AI use policy, which you can use in your work
- [Arizona State University](https://libguides.asu.edu/generativeai/acknowledgement): <i>For now, however, there is an expectation in academia that users to disclose when AI tools contribute meaningfully to the development of ideas, content, or structure in a project.</i>
- [University of Melbourne](https://students.unimelb.edu.au/academic-skills/academic-integrity/acknowledging-use-of-ai-tools-and-technologies#examples) <i>If you have used an AI tool or technology in any other way (see below) in the process of completing your assessment, an acknowledgement of how you have used AI tools or technologies is required. </i>

**UVA AI Tools**- UVA licenses various AI tools for the UVA community to use. They are always changing, so to see what is available it is best to take a look at the [UVA ITS AI page](https://virginia.service-now.com/its?id=itsweb_kb_article&sys_id=dbe41947dbe3f91066d98f38139619db).
- Personal information protected
- Cost managed
- Increased Usage limits
