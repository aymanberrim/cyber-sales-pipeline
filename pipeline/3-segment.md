# 3 · Segment

**Input:** accounts with a confirmed agent stack and a reachable buyer.
**Output:** homogeneous groups, one message angle per group, keyed on the vulnerability the stack exposes — not on industry.
**Exit criterion:** every account sits in exactly one group with one lead vulnerability and one message angle.
**Metric:** reply rate per group after 60 sends (re-cut any group under 3%; double down above 8%).

## Segment by exposure, not by sector

Industry is a weak cut for the vendor; **stack-and-faille is the strong one**, because it maps straight to the attack we demo:

- **RAG-over-internal-docs group** → lead with *indirect prompt injection + data leakage*.
- **Tool/API-calling agent group** (CRM, payments, infra) → lead with *tool abuse + excessive autonomy*.
- **Memory / multi-session assistant group** → lead with *memory poisoning*.
- **Plugin / third-party-tool group** → lead with *supply-chain risk*.

The ring (portfolio / funded-startup / enterprise) sets the **tone and channel**; the vulnerability group sets the **content**.

## One message per group

Role-first opener, the group's vulnerability named concretely, no price in cold, exactly one CTA. The copy lives in [`messages/sequence.md`](../messages/sequence.md). Replies are the test: a group that does not answer is re-cut, not re-written.

## Handoff

Pass each group, with its lead vulnerability and approved angle, to **4 · Engage**.
