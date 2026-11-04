# Play · agent-attack-surface-mapping

**The one move that makes the vendor's outbound personal.** It turns a detected stack into the single vulnerability worth demoing — so the first message names a real, specific exposure instead of selling "AI security."

Same logic as finding a company's accounting software and arriving with the exact case you can automate on it: here the "software" is the agent stack, and the "case" is the faille the stack is structurally exposed to.

## Inputs

From **2 · Source**: a read of the target's agent stack — framework, model provider, what data the agent touches, what tools it can call, whether it has memory, whether it uses third-party plugins.

## The play

1. **Describe the config in one sentence.** e.g. *"an agent on a hosted LLM, RAG over internal docs, write access to the CRM, no human checkpoint on actions."*
2. **Map config → vulnerability class** (the stack predicts the exposure):

   | If the config has… | The lead vulnerability is… |
   |---|---|
   | RAG / external documents | indirect prompt injection + data leakage |
   | tool / function / API calling | tool abuse |
   | actions with no human checkpoint | excessive autonomy |
   | multi-session memory | memory poisoning |
   | third-party plugins / tools | supply-chain risk |
   | a safety / guardrail layer | guardrail bypass (always worth testing) |

3. **Pick the one to demo.** Choose the class with the highest blast radius for *that* business (money-moving tool abuse for a fintech agent; data leakage for a health or legal RAG agent). One attack, not a list.
4. **Write the exposure line** the outbound uses: *"On a `<stack>`, the `<vulnerability>` that lands first is `<one concrete attack>` — I can show you if it works on yours."*

## What good looks like

A message a founder reads and thinks *"they actually looked at what we run."* The exposure line names their stack and one attack, is true, and leads to a scoped red-team — not a demo of the vendor's dashboard.

## Rules

- Never claim a breach you have not demonstrated or cannot demonstrate on request.
- Probe only a target's **public** surface before contact; anything deeper needs their written go-ahead (that is the red-team, and it is scoped and approved).
- Map to the standards so the exposure carries weight: OWASP Agentic / LLM Top 10, EU AI Act, NIST, the Singapore agentic-AI addendum.

## Handoff

The chosen vulnerability + exposure line feeds **3 · Segment** (the group's angle) and **6 · Close** (the attack the red-team demonstrates).
