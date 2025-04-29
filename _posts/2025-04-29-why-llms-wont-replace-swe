---
title: Why LLMs Won't Replace SWE
author: 
date: 2025-04-29 00:34:00 +0800
categories: [AI]
tags: [llm,ai]
---

Obama recently commented on the rapid progression of AI, stating: “We’re now at a moment where AI is doing so much so quickly that even the people who are closest to it are surprised by its capabilities.” While AI advancements are indeed revolutionary, much of the discourse around it is science fiction fantasy rather than reality. We should remember that history is full of failed predictions from prominent people. Cognitive biases, such as the “availability heuristic” (overestimating what’s most recently visible) and “optimism bias” (overconfidence in positive outcomes), affect even the smartest tech-types. Moreover, tech CEOs have financial incentives to hype AI—VC funding for AI startups surged to $42.5 billion in 2023, and companies like OpenAI and Anthropic are in a race for dominance.

While AI is revolutionizing, SWEs won’t be replaced anytime soon due to architectural limitations. One major problem with models is context. Context is the information that a model knows in a conversation. Large enterprise codebases often span millions of lines of code. Assuming an average of 5 tokens per line, a model would need a 5 million token context window to fully read a codebase. This is far beyond the 200k token limit of Claude 3.5 Sonnet. Even with techniques like hierarchical chunking, performance degrades as context expands: perplexity (a measure of model confidence) drops, and computational costs scale quadratically with context length.

Retrieval-Augmented Generation (RAG) helps fix this by allowing information to be retrieved from data sources. But LLMs still struggle autonomously solving tasks with long inferential distances. For example, AI agents like Claude 3.7 playing Pokémon frequently get stuck in a loop; it’s not even comparable to a human player. 

AI progress is undeniable and research interest in AI is skyrocketing. Research labs like DeepMind, OpenAI, and Anthropic are pushing boundaries of model capabilities. Once models are able to solve novel problems that take a team of researchers years, then we may need to be worried. Until then, claims of SWE job displacement are premature. 

