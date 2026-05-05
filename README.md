# AI Agents & The Lost in Conversation Phenomenon

![Lost in Conversation Header](images/2026-05-05_10-33-43.jpg)


A new study from Microsoft Research and Salesforce Research quietly demolishes one of the more comfortable assumptions in agentic AI — that we can compensate for fragile models by building cleverer orchestration around them.

Across 200,000+ simulated conversations and 15 frontier LLMs, the authors found an average 39% performance drop when the same task is delivered across multiple turns versus a single fully-specified instruction. The real damage is in reliability, which collapses by 112%. The paper names this the **lost in conversation phenomenon** — when an LLM takes a wrong turn early in a conversation, it does not recover.

This is a finding about agents. An agent is, by construction, a multi-turn conversation the model has with itself and its tools. Every ReAct loop, every tool call, every retrieval is information delivered piece by piece — exactly the pattern that triggers the effect.

Production harness strategies (RECAP, SNOWBALL) recover only 15–20% of the lost performance. There is a ceiling on what scaffolding can fix.

Read the full blog post: [ai_agents_lost_in_conversation.md](ai_agents_lost_in_conversation.md)

![Lost in Conversation Header](images/lost-in-conversation-header.jpg)


## Author

**Cobus Greyling** — Chief AI Evangelist @ Kore.ai

## Reference

- [LLMs Get Lost In Multi-Turn Conversation](https://arxiv.org/abs/2502.01601)
