# 5 · Convert

**Input:** a reply from an engaged lead.
**Output:** a booked red-team scoping call, with the lead qualified.
**Exit criterion:** call booked **and** three facts confirmed: agents in production, the authority those agents hold, and who owns AI security.
**Metric:** reply-to-call rate; speed from signal to call (default: 2–24 h).

## Handle the reply fast, then qualify on the call

Every reply gets an owner and a dated next action the day it lands — reply SLA 2 h for hot, same business day otherwise. The safety net (unhandled replies) is empty every evening; that is the mechanism, not willpower.

The call does the qualifying, live:

- **Do they run agents in production?** (not a prototype — real traffic, real users.)
- **What authority do the agents hold?** (tools, data, money, autonomy — this sizes the risk and the deal.)
- **Who owns the security of the AI?** (the champion; and in enterprise, who signs.)

## Objections, briefly

- *"We already have a security team / pentest."* — Traditional pentest tests code and infra; it does not test agent *behavior* — prompt injection, tool abuse, memory. Different surface.
- *"Our guardrails handle it."* — Good; the red-team measures whether they actually hold. If they do, that is a result worth having in writing.
- *"Too early, we're small."* — Cheapest moment to harden is before the agent has authority over real money or data. Later is a rewrite.

## Handoff

A booked, qualified call goes to **6 · Close** with the scoping notes and the target vulnerability to demo.
