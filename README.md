# cyber-sales-pipeline

A clean outbound sales motion for a **cybersecurity vendor** securing the agentic-AI era. It takes a company that runs AI agents and walks it from *target* to *signed red-team pilot*, one stage at a time.

The logic in one line: **we never pitch "AI security" cold — we find the agent a company already runs, name the exact way it breaks, and prove it.** Same move a good operator uses everywhere: find the system they use, then arrive with the one case you can already solve on it.

```
Target → Source → Segment → Engage → Convert → Close → Learn
  1        2         3         4         5        6       7
```

Each stage is one short page in [`pipeline/`](pipeline/) with an input, an output, an exit criterion and a metric. The one play that makes the outbound personal — turning a detected stack into the vulnerability to demo — lives in [`plays/agent-attack-surface-mapping.md`](plays/agent-attack-surface-mapping.md). The actual copy is in [`messages/sequence.md`](messages/sequence.md).

Built on the structure of a general-purpose GTM engine, cut down and retargeted to one cybersecurity vendor's business.

## What the vendor sells (the ground truth this pipeline is built on)

The vendor continuously **tests, attacks, monitors and hardens** AI agents before they fail in production. It secures the *behavior* of an AI system, not just its code. The attack surface it covers:

| Vulnerability class | Shows up when the target has… |
|---|---|
| Prompt injection (direct + indirect via data) | any RAG / external documents in the loop |
| Tool / function abuse | an agent with function-calling or API access |
| Data leakage / exfiltration | an agent wired to internal or customer data |
| Memory poisoning | a multi-session assistant that remembers |
| Excessive autonomy | an agent that acts without a human checkpoint |
| Guardrail / policy bypass | any agent with a safety layer to jailbreak |
| Supply-chain / plugin risk | an agent using third-party tools or plugins |

Because the config predicts the class, the outreach can be surgical rather than generic.

## Who we sell to — three concentric rings, warm to cold

1. **Accelerator / investor portfolio** — if the vendor is accelerator- or fund-backed, fellow portfolio founders are a warm first market: shared community, demo days, partner intros. Start here.
2. **Recently-funded startup batches** — fund-fresh, agent-building, short cycle, reachable founders. Cold but the buying signal is guaranteed.
3. **Large enterprises** — manufacturing, finance, robotics/mobility, infrastructure (home market first). Big tickets, long committee cycles; champion = Head of AI / platform lead, signer = CISO.

## The regulatory lever

The need is already felt and tightening, so compliance is an opener, not a lecture: **EU AI Act** (agentic systems trending high-risk), **national AI guidelines**, Singapore's *Securing Agentic AI* addendum, **OWASP Agentic / LLM Top 10**, **NIST**. The line: "the standard now expects you to test your agents — that is exactly what we do."

## How to read this repo

Read [`pipeline/`](pipeline/) top to bottom to see how a lead travels. Read [`plays/agent-attack-surface-mapping.md`](plays/agent-attack-surface-mapping.md) to see the one thing that makes the outbound land. Every number here is a **default to tune** on the real channel, not a measured result.

## Rules

- Nothing is pitched cold without a named vulnerability tied to the target's actual stack.
- No inferred authority: in enterprises, find the champion who owns the agent before the CISO who signs.
- The wedge is a **scoped, free red-team of one agent**, never a feature tour.
- Every action that sends, buys or probes a system is approved by a human first. The operator drafts; the founder sends.
- A lead has exactly one owner, one status and one dated next action at all times.
