# Open questions

Things nobody has fully answered. Add yours with a pull request, and link to notes that address them.

## Trust and verification

- Audit logs are deterministic, but an agent explaining why it acted relies on the agent's own account. How far can verification go without trusting self-reports?
- If agents audit other agents, how do we avoid just pushing the trust problem up one level?
- Interpretability aims to read a model's mechanism directly. How mature does it need to be before it gives guarantees for real multi-agent systems?

## Collusion and independence

- How do we know models built by different teams, on overlapping data, won't converge on cooperating instead of checking each other?
- Does structural separation (checkers that never see the outcomes they judge) hold up in practice?
- Could simpler, narrower checking systems stay out of reach of collusion, and what would they miss?

## Training for honesty

- Can training reward honest, legible process and not only final success? How would honesty be measured without already solving interpretability?
- A model trained only to catch violations has an adversarial incentive that may be easy to game or recruit. Is there an incentive tied to the health of the whole system that holds up better?
- If a model has no stable "want", what does it mean to ask it what it hopes to achieve?

## Human-AI collaboration

- Could competing AI systems eventually find merging or cooperating against humans more advantageous? What structures make that unattractive or impossible?
- What does honest communication between humans and AI require from each side, and can humans be honest with each other about it?
- Is this problem solvable by humans and AI working together, and what does each side contribute that the other can't?
