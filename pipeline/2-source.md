# 2 · Source

**Input:** a qualified account with a trigger.
**Output:** the people who can say yes, plus a confirmed read of the agent stack the account runs.
**Exit criterion:** stack identified (or confidently narrowed) **and** a reachable decision-maker with a verified channel.
**Metric:** stack-identification coverage across the list (default target: 80%+).

## Reconnaissance — knowing their system before any contact

What is knowable from the outside, no insider needed:

- **Job posts** — the richest source. "agent framework / LLMOps / RAG / LLM" postings name the framework, the model provider, the vector DB, the guardrail tooling.
- **Provider case studies** — the major LLM providers publish "built with us" stories that reveal the engine.
- **Engineering blog / conference talks** — teams describe their agent architecture in public.
- **The public agent itself** — if they expose a chatbot or agent, probe it: what it refuses, what it leaks, which model answers. This is the vendor's own craft applied to recon.
- **The AI team on LinkedIn** — titles and tenure reveal the stack and who owns it.

→ Output of recon reads like: *"a hosted LLM + an agent framework + internal RAG; the agent has CRM write access."* That sentence is what makes the later message surgical.

## Decision-makers (buyer, not title)

- **Ring 1/2 (startups):** the founder or CTO. One person, one conversation.
- **Ring 3 (enterprise):** the **champion** is the Head of AI / AI platform lead who owns the agent and carries the headache; the **signer** is the CISO. Reach the champion first — authority is diffuse, and a cold CISO touch dies in a queue.

## Handoff

Pass accounts with a confirmed stack + reachable buyer to **3 · Segment**. Feed the stack read into [`plays/agent-attack-surface-mapping.md`](../plays/agent-attack-surface-mapping.md) to derive the vulnerability class.
