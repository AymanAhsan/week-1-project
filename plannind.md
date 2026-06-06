## Domain
The domain I chose is learning ratings for Math professors at CCNY. This knowledge is obviously valuable for any student in the STEM field because math is a pretty hard subject already, and finding good professors really goes a long way.
Because there are so many professors to choose from, even going through 10 different ones can be a hassle, switching through tabs.

## Documents
Mathematics professors at CCNY

https://www.ratemyprofessors.com/professor/1583271
https://www.ratemyprofessors.com/professor/1583271
https://www.ratemyprofessors.com/professor/1588752
https://www.ratemyprofessors.com/professor/1751203
https://www.ratemyprofessors.com/professor/631569
https://www.ratemyprofessors.com/professor/1023742
https://www.ratemyprofessors.com/professor/1807944
https://www.ratemyprofessors.com/professor/221879
https://www.ratemyprofessors.com/professor/1249262
https://www.ratemyprofessors.com/professor/1913056


## Chunking Strategy
A fixed size seems ideal because each review is short.

Useful AI prompts:
- "Explain how chunk size affects retrieval quality for short, opinion-based reviews."
- "What are the tradeoffs between chunking by paragraph vs. fixed character count for [my document type]?"
- "If I use 200-character chunks for review text, what kinds of queries might this fail for?"]

## Retrieval Approach
[Which embedding model are you using (e.g., all-MiniLM-L6-v2 via sentence-transformers)? How many chunks will you retrieve per query (top-k)? If you were deploying this for real users and cost wasn't a constraint, what tradeoffs would you weigh in choosing a different embedding model — context length, multilingual support, accuracy on domain-specific text, latency?

Guiding questions:
- How many retrieved chunks is enough to give the LLM useful context? What happens if you retrieve too few? Too many?
- Why does semantic search find relevant chunks even when the query doesn't share exact words with the document?

Useful AI prompts:
- "What are different strategies for structuring embeddings for short, opinion-based text?"
- "What does top-k mean in a retrieval system, and what are the tradeoffs of setting it too high vs. too low?"]

## Evaluation Plan
[List your 5 test questions with their expected correct answers. Questions should be specific enough that you can judge whether the system's response is right or wrong — "What are good dining halls?" is too vague; "What do students say about wait times at the [dining hall name] during lunch?" is testable.]

## Anticipated Challenges
[What could go wrong? Consider: noisy or inconsistent documents, missing source attribution, off-topic retrieval, chunks that split key information across boundaries. Name at least two specific risks.]

## AI Tool Plan
[Which parts of the pipeline do you plan to use AI tools (Claude, Copilot, ChatGPT, etc.) to help you implement? For each part, describe what you'll give the AI as input — which sections of this planning.md, which requirements from the instructions — and what you expect it to produce. Be specific: "I'll prompt Claude with my chunking strategy section and ask it to implement the chunk_text() function" is a plan. "I'll use AI to help me code" is not.]
