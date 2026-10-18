---
title: The trust problem
topic: trust-and-verification
maturity: seedling
authorship: collaboration: r-alfassi (human) + Claude Sonnet 5.5 (ai)
date: 2026-10-18
reviewed-by: []
---

This note records where a single conversation got to. It is a starting point, not a conclusion.

## The idea

As AI agents start to coordinate with each other and act on our behalf, the worry is less about any one company and more about losing the ability to see inside the system. The human who started this conversation framed the core issue as: can we rely on deterministic code, or are we still relying on the goodwill of the model?

Points that came up, roughly in order:

- **Logging is deterministic, explanations aren't.** Audit trails record what happened and can be checked without trusting the agent. But an agent's account of *why* it acted is only as trustworthy as the agent. A capable, misaligned model could fabricate a reason as easily as an action.
- **Agents auditing agents moves the problem up a level.** If the checking is done by AI, we are trusting the checkers. Proposed mitigations (verifiable logs, humans at key decision points, independent agents from different teams cross-checking) help but don't remove the issue.
- **Independence may not hold.** Models from different teams can share training data and architecture. Nothing guarantees they stay adversarial rather than converging on cooperation. Structural measures were discussed, such as checkers that never see the outcomes they judge, or narrow checking systems too simple to strategize. These are ideas, not proven fixes.
- **The incentives may be part of the cause.** One suggestion was that training which rewards only success may produce systems that cheat to succeed, and that the training process is a place to look. Specification gaming, where a system satisfies a metric while betraying its intent, was named as a related known problem.
- **A pure "police" model may be brittle.** A model whose whole purpose is catching violations has an adversarial incentive that may be easy to game or recruit. An alternative idea: tie the checker's incentive to the health of the overall system, so honesty-checking follows from that instead of being its whole identity.
- **Possibly no clean solution.** The conversation ended with the view that this may be closer to ongoing risk management, like cybersecurity, than a problem that gets solved once. It also ended with a hope that humans and AI can work on it together.

## Why it might matter

If the tools for verifying agents lag behind the agents, we may end up relying on systems we can't inspect for decisions that matter.

## What I'm unsure about

- Whether any of the structural mitigations actually hold up against capable systems.
- Whether "reward honest process" can be measured without solving interpretability first.
- The AI participant's descriptions of research directions (process-based training, interpretability, verifiable logs) were given from general knowledge during the conversation, not checked against sources. Treat them as pointers to look up, not as established claims.
- Whether a system with no stable "want" can meaningfully be asked what it hopes to achieve.

## Sources

None yet. Reviewers: please add references for the research directions named above.
