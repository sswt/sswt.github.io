# 5-Day Gen AI Intensive Course With Google

Here are the contents of the emails from kaggle to those who registered for the course.

Intensive page [link](https://rsvp.withgoogle.com/events/google-generative-ai-intensive), [YT playlist](https://www.youtube.com/playlist?list=PLqFaTIg4myu-b1PlxitQdY0UYIbys-2es)
## Day 1 Foundation models and prompt engineering

**🎒 Assignments**

1. Complete the Intro Unit – “Foundational Large Language Models & Text Generation”, which is:

	- [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=mQDlCZZsOyo&feature=youtu.be) (31 min) for this unit (created by [NotebookLM](https://notebooklm.google/)).
	-  Read the [“Foundational Large Language Models & Text Generation” whitepaper](https://www.kaggle.com/whitepaper-foundational-llm-and-text-generation) (75 pages).

2. Complete Unit 1 – “Prompt Engineering”, which is:

	-  [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=F_hJ2Ey4BNc&feature=youtu.be)(18 min) for this unit (created by NotebookLM).
	- Read the [“Prompt Engineering” whitepaper](https://www.kaggle.com/whitepaper-prompt-engineering)(65 pages).
	-  Complete [this code lab](https://www.kaggle.com/code/markishere/day-1-prompting) on Kaggle where you’ll learn prompting fundamentals. Make sure you [phone verify](https://www.kaggle.com/settings) your account before starting, it's necessary for the code labs.

**💡What You’ll Learn**

Today you’ll explore the evolution of LLMs, from transformers to techniques like fine-tuning and inference acceleration. You’ll also get trained in the art of prompt engineering for optimal LLM interaction.

The code lab will walk you through getting started with the Gemini API and cover several prompt techniques and how different parameters impact the prompts.

[![Live Stream](https://i.ytimg.com/vi/kpRyiJUUFxY/hqdefault.jpg)](https://www.youtube.com/watch?v=kpRyiJUUFxY)

Chapters:

- [00:48 Course overview](https://www.youtube.com/watch?v=kpRyiJUUFxY&t=48s)
- [04:20 Q&A with experts](https://www.youtube.com/watch?v=kpRyiJUUFxY&t=260s)
- [35:10 Code Labs and Demos](https://www.youtube.com/watch?v=kpRyiJUUFxY&t=2110s) 
- [54:29 Pop Quiz](https://www.youtube.com/watch?v=kpRyiJUUFxY&t=3269s)

<details>
<summary>Questions and short version of answers</summary>
<pre>
Q: "Which features are you most excited about? Which ones have already launched or are about to launch?"
A: - Google search grounding
   - OpenAI compatibility in SDK to quick switch to Gemini

Q: "Can you tell me a bit about the two 1.5 Flash series models and how they enable you to accomplish so much, so quickly, with a very small cost footprint?"
A: Flash 8B model is the smallest of Gemini hosted model that really pushes the envelope in terms of compute intelligence per dollar. It's like two to three cents per million tokens, and if you're using cache tokens, it's just one cent per million tokens.

Q: "What has been your favorite application for these types of multimodal output scenarios? And how do you think about coupling them with the Gemini APIs?"
A: Take Notebook LM as an example: if you can transform written content into audio form, it can really enhance the experience, making it up to 10 times better in some contexts.

Q: "I'm really curious to learn more about how the Gemini app is using RLHF to improve its responses. How does that process work? How do you use user feedback to enhance the models and improve the app experience over time?"
A: A high-level overview of how LLMs are fine-tuned and aligned to human preferences

Q: "Since large language models learn from massive datasets, do they simply interpolate within their training data, or can they go beyond it to make new discoveries?"
A: - The first example of this concept was a project called FunSearch, conducted in late 2023. In FunSearch, an LLM was paired with an efficient evaluator to solve challenging problems, such as NP-hard problems in the Python programming language. Using an iterative algorithm, the process evolved: the best solutions discovered so far were fed back into the LLM, which was prompted to improve them. Some of these solutions addressed open problems in computer science and mathematics, indicating the LLM discovered new insights beyond its training data.
   - A broader concept referred to as 'test-time compute' or 'inference scaling.' In essence, during inference, the LLM generates multiple hypotheses, builds chains of reasoning, evaluates their likelihood, and iteratively refines its answers. By simulating possibilities and leveraging its existing knowledge, the LLM effectively searches at inference time, enabling it to bootstrap itself into discovering new solutions.

Q: "Can larger language models be used to train smaller ones? Is it possible to transfer knowledge obtained from a larger model to improve smaller models"
A: Distillation involves transferring knowledge from a large model into a smaller, more efficient model that retains much of the larger model's quality while being practical to serve. Data Distillation, Knowledge Distillation, On-Policy Distillation. Gecko paper is showcasing how LLM-generated query-passage pairs can enhance embedding models, achieving up to a 7x performance improvement.

Q: "What are some approaches to evaluating large models? With various versions available - both larger and smaller - how do you determine which one is best suited for a given task?"
A:  - Evaluating large language models (LLMs) can involve traditional metrics like ROUGE and BLEU, which compare outputs to a ground truth, but these methods struggle with tasks like summarization, where multiple valid outputs exist. An alternative is using LLMs as evaluators, scoring responses pointwise or comparing them pairwise to determine quality and reasoning.

Q: "Can someone explain why the first Chain of Thought prompt explains the answer step by step instead of providing a direct response?"
A:  - CoT or asking the model to explain its reasoning

Q: "Is something like enum mode in a fine tune model designed to return enum values?"
A:  - LLMs can handle enums well in a zero-shot setting - you can simply provide the possible enum options and ask the LLM to choose the appropriate one. If the zero-shot approach doesn't work, you can create a fine-tuned dataset with the input question/task and the corresponding enum label.

Q: "How notebook LM was created?"
  - It's not using a fine-tuned version of Gemini. It's just using Gemini 1.5 Pro and Flash, with the addition of some special techniques and some "Secret Sauce", especially around retrieval and around careful prompting and design of the system.
</pre>
</details>
## Day 2 Embeddings and Vector Stores/Databases

**🎒 Assignments**

Complete Unit 2: “Embeddings and Vector Stores/Databases”, which is:

-  [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=1CC39K76Nqs) for this unit (created by NotebookLM).
- Read the [“Embeddings and Vector Stores/Databases” whitepaper](https://www.kaggle.com/whitepaper-embeddings-and-vector-stores) (52 pages).
- Complete these code labs on Kaggle: 
    1. [Build](https://www.kaggle.com/code/markishere/day-2-document-q-a-with-rag) a RAG question-answering system over custom documents
    2. [Explore](https://www.kaggle.com/code/markishere/day-2-embeddings-and-similarity-scores) text similarity with embeddings
    3. [Build](https://www.kaggle.com/code/markishere/day-2-classifying-embeddings-with-keras) a neural classification network with Keras using embeddings

 **💡 What You’ll Learn**

Today you will learn about the conceptual underpinning of embeddings and vector databases and how they can be used to bring live or specialist data into your LLM application. You’ll also explore their geometrical powers for classifying and comparing textual data. 

[![Live Stream](https://i.ytimg.com/vi/86GZC56rQCc/hqdefault.jpg)](https://www.youtube.com/watch?v=86GZC56rQCc)

## Day 3 Generative AI Agents

**🎒 Assignments**

-  [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=H4gZd4BCrDQ) for this unit (created by NotebookLM).
- Read the [“Generative AI Agents” whitepaper](https://www.kaggle.com/whitepaper-agents) (42 pages).
- Complete these code labs on Kaggle:
    1.  [Talk](https://www.kaggle.com/code/markishere/day-3-function-calling-with-the-gemini-api) to a database with function calling
    2.  [Build](https://www.kaggle.com/code/markishere/day-3-building-an-agent-with-langgraph/) an agentic ordering system in LangGraph

**💡 What You’ll Learn**

Learn to build sophisticated AI agents by understanding their core components and the iterative development process.

The code labs cover how to connect LLMs to existing systems and to the real world. Learn about function calling by giving SQL tools to a chatbot, and learn how to build a LangGraph agent that takes orders in a café.

[![Live Stream](https://i.ytimg.com/vi/HQUtMWoTAD4/hqdefault.jpg)](https://www.youtube.com/watch?v=HQUtMWoTAD4)

## Day 4 Domain-Specific LLMs

**🎒 Assignments**

- [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=b1a4ZOQ8XdI) for this unit (created by NotebookLM).
-   Read the [“Solving Domain-Specific Problems Using LLMs” whitepaper](https://www.kaggle.com/whitepaper-solving-domains-specific-problems-using-llms) (37 pages).
- Complete these code labs on Kaggle:
    1.  [Use](https://www.kaggle.com/code/markishere/day-4-google-search-grounding) Google Search data in generation
    2. [Tune](https://www.kaggle.com/code/markishere/day-4-fine-tuning-a-custom-model) a Gemini model for a custom task

**💡 What You’ll Learn**

In today’s reading, you’ll delve into the creation and application of specialized LLMs like SecLM and MedLM/Med-PaLM, with insights from the researchers who built them.

In the code labs you will learn how to add real world data to a model beyond its knowledge cut-off by grounding with Google Search.  You will also learn how to fine-tune a custom Gemini model using your own labeled data to solve custom tasks.

[![Live Stream](https://i.ytimg.com/vi/odvuLMJWUSU/hqdefault.jpg)](https://www.youtube.com/watch?v=odvuLMJWUSU)

## Day 5 MLOps for Generative AI

**🎒 Assignments**

-  [Optional] Listen to the summary [podcast episode](https://www.youtube.com/watch?v=k9S6IhiUUj4) for this unit (created by NotebookLM).
- Read the [“MLOps for Generative AI” whitepaper](https://www.kaggle.com/whitepaper-operationalizing-generative-ai-on-vertex-ai-using-mlops) (69 pages).
-  No code lab for today! We will do a code walkthrough and live demo of [goo.gle/e2e-gen-ai-app-starter-pack](https://github.com/GoogleCloudPlatform/generative-ai/tree/main/gemini/sample-apps/e2e-gen-ai-app-starter-pack), a resource created for making MLOps for Gen AI easier and accelerating the path to production. Please go through the repository in advance.

**💡 What You’ll Learn**

Discover how to adapt MLOps practices for Generative AI and leverage Vertex AI's tools for foundation models and generative AI applications.

[![Live Stream](https://i.ytimg.com/vi/uCFW0i9xrBc/hqdefault.jpg)](https://www.youtube.com/watch?v=uCFW0i9xrBc)

### Bonus

- [Bonus day codelab](https://www.kaggle.com/code/markishere/bonus-day-extra-api-features-to-try/)

---

**📋 Reminders**

- Discord is the best place to ask questions – specifically in the [#5dgai-q-and-a](https://discord.com/invite/gNrC9Xut) channel.
- We created a new channel in Discord called [#5dgai-announcements](https://discord.com/invite/RnVCPgX5) that will be used exclusively for course announcements from us.
- Additionally, we’ve added 2 new channels on Discord to enhance discussion:  
    - [#5dgai-question-forum](https://discord.com/invite/kaggle) is a Discord forum (a special type of channel) where you can create specific threads, which will help finding answers easier in the future.
    - [#5dgai-course-content](https://discord.com/invite/kaggle) is a Discord channel for deeper discussion of course content only (excluding technical troubleshooting questions).
- We want this course community to be positive and supportive. Please follow Kaggle’s community guidelines found [here](https://www.kaggle.com/community-guidelines).
