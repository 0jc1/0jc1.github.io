---
title: Why LLMs Won't Replace SWE
author: 
date: 2025-04-29 00:34:00 +0800
categories: [AI]
tags: [llm,ai]
---

Obama recently commented on the rapid progression of AI, stating: “AI can code better than 60% to 70% of human coders.” While AI advancements are indeed revolutionary, much of the discourse around it is science fiction fantasy rather than reality. We should remember that history is full of failed predictions from prominent people. Cognitive biases, such as the “availability heuristic” (overestimating what’s most recently visible) and “optimism bias” (overconfidence in positive outcomes), affect even the smartest tech-types. Moreover, tech CEOs have financial incentives to hype AI—VC funding for AI startups surged to $42.5 billion in 2023, and companies like OpenAI and Anthropic are in a race for dominance.

While AI is revolutionizing, SWEs won’t be replaced anytime soon due to architectural limitations. One major problem with transformer-based models is context. Context is the information that a model knows in a conversation. Large enterprise codebases often span millions of lines of code. Assuming an average of 5 tokens per line, a model would need a 5 million token context window to fully read a codebase. This is far beyond the 200k token limit of Claude 3.7 Sonnet. Even with techniques like hierarchical chunking and context management, performance degrades as the context length grows: perplexity (a measure of model confidence) drops, and computational costs scale quadratically with context length.

![2b065bd2615efdcf86e6737bcf6ad605a8fe187a-610x544](https://github.com/user-attachments/assets/8a8b5852-f061-4076-bc67-84bcd01d97d9)

Retrieval-Augmented Generation (RAG) helps fix this by allowing information to be retrieved from data sources. But LLMs still struggle to autonomously solve tasks with long inferential distances, such as beating a video game or writing a big piece of software. For example, AI agents like Claude 3.7 playing Pokémon frequently get stuck in a loop or fails to adapt to edge cases; it’s not even comparable to a human player. 

![2025-04-29_14-09](https://github.com/user-attachments/assets/79ac7e6b-9593-449a-907b-7e565c5c8f36)

LLMs are great tools for coding, but they cannot fully replace any coder for the reasons above. In a recent project in C, I encountered a confusing bug and Claude failed to fix it. It got stuck in a negative feedback loop and it kept creating more bugs and hallucinating. Generally speaking, LLMs are terrible with low-level programming in C and Rust. Even when it does write a working program, it creates technical debt and unoptimized code. But for high level programming (like in JS and Python) and frontend development, LLMs can really shine.  

AI progress is undeniable and AI research interest is skyrocketing. Research labs like DeepMind, OpenAI, and Anthropic are pushing boundaries of model capabilities. Once AI models can independently solve novel, complex problems that would take years of effort from researchers, we should be deeply concerned. Until then, claims of SWE job displacement are premature. 

