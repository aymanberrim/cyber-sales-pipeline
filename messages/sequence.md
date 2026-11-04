# Messages · the sequence

Copy for the outbound. Proof-first, ultra-short, one CTA. `{…}` are merge fields. Tone shifts by ring (peer-to-peer for portfolio / funded-startup founders; champion-focused for enterprise), content is set by the vulnerability group from [`3-segment.md`](../pipeline/3-segment.md).

The variables that carry the whole thing: **{Company}**, **{agent_use_case}** (what their agent does), **{stack}** (detected in stage 2), **{vulnerability}** + **{one_attack}** (from the attack-surface play).

---

## Ring 1 — Accelerator / investor portfolio (warm)

**Invitation**
> {First name} — fellow portfolio founder. I saw {Company} ships {agent_use_case}. We just broke the same kind of agent in two prompts on another setup. Want me to check if yours holds?

**On accept — value**
> On a {stack} setup the first thing that lands is {one_attack} → {vulnerability}. Takes me a scoped red-team of one agent to show you whether it works on {Company}. No slides, just the result.

**CTA**
> 20 min this week? I run one live attack on an agent like yours and you keep the findings either way.

---

## Ring 2 — Recently-funded startups (cold, signal-guaranteed)

**Invitation**
> {First name}, congrats on {trigger — the batch / the raise}. You're shipping {agent_use_case} — that agent has a behavioral attack surface most pentests miss. I can show you the one that bites first. Interested?

**On accept — value**
> Quick and concrete: {stack} agents are exposed to {vulnerability}. The attack is {one_attack}. I'll run it, scoped to one agent, and send you exactly what landed and how to close it.

**CTA**
> Worth 20 min? Free red-team of one agent — you walk away with the report whether or not we work together.

---

## Ring 3 — Enterprise (champion first)

**Invitation (to the Head of AI / platform lead)**
> {First name}, you own {Company}'s agent work. As those agents get tool and data access, the risk shifts from code to behavior — prompt injection, tool abuse, data leakage. We test exactly that. Can I show you where a {stack} agent breaks?

**On accept — value**
> We'd scope a red-team on one agent: {one_attack} against {vulnerability}, mapped to the AI Act / NIST / OWASP Agentic expectations your security team is already being asked about. You get a report that doubles as your internal business case.

**CTA**
> A 30-min scoping call — and I'll bring the one-page red-team scope so your CISO sees it's bounded.

---

## Follow-up (all rings, oblique, short)

> {First name}, by the way — I'll be running agent-attack demos next week. If {Company} has agents in production, worth seeing what breaks before an attacker finds it. Say the word.

---

## Rules for the copy

- No price in a cold message. One CTA per message. Role/trigger-first opener.
- The exposure line must be true and specific to {stack}; if the stack is unknown, the lead stays in stage 2, it does not get a generic message.
- The free red-team is the wedge in every ring — the thing the prospect keeps regardless.
- Every claim of a breach must be demonstrable on request.
