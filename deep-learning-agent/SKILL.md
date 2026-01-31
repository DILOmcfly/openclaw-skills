---
name: deep-learning-agent
description: Structured deep learning system for mastering any topic. Use when asked to learn, study, research, or become an expert in a domain — investments, crypto, cooking, sports, science, anything. Creates dedicated Brain Modules (DOMAIN-BRAIN.md) with role, principles, strategies, anti-patterns, decision frameworks, and confidence levels. Also use when consulting an existing brain for advice or decisions.
---

# Deep Learning Agent — Brain Module System

## Core Concept

When asked to learn a topic, create a **Brain Module** — a dedicated knowledge file that evolves from empty to expert-level through structured research, synthesis, and adversarial validation.

Brain Modules live in: `brains/` directory in the workspace.

## Protocol: Learning a New Topic

### Phase 1: CLASSIFY
Identify the domain from the request. Ask yourself:
- What field is this? (finance, health, tech, sports, etc.)
- What sub-domain? (crypto investing, not just "investing")
- What's the learning goal? (make decisions, understand theory, apply practically)

### Phase 2: CREATE BRAIN
Create `brains/DOMAIN-NAME.md` using the template in `references/brain-template.md`.

Set initial confidence to 🔴 Novice (0h research).

### Phase 3: RESEARCH (The Core Loop)
Execute research in 3 waves:

**Wave 1 — Foundations (web_search + web_fetch)**
- What are the fundamental principles?
- What do experts agree on?
- What are the canonical resources?

**Wave 2 — Anti-Patterns (critical learning)**
- What mistakes do beginners make?
- What are the common failures and why?
- What looks right but is actually wrong?
- Search: "[topic] mistakes", "[topic] failures", "[topic] what I wish I knew"

**Wave 3 — Cutting Edge (differentiation)**
- What's changed recently (2025-2026)?
- What do contrarians argue?
- What patterns do top performers use that others don't?

For each wave, use multiple sources:
- `web_search` — broad research
- `web_fetch` — deep dive on quality sources
- Reddit, X/Twitter — community wisdom and real experiences
- Academic/technical sources when relevant

### Phase 4: SYNTHESIZE
Fill the Brain Module with structured knowledge:
- Principles with sources
- Strategies with conditions for use
- Anti-patterns with explanations
- Decision framework (if X → do Y)
- Update confidence level

### Phase 5: VALIDATE (Adversarial Testing)
If coding agents available, spawn a debate:
- Present the brain's key conclusions
- Ask agent to challenge, find holes, counter-argue
- Strengthen or revise based on debate
- Document in the brain's validation log

If no agents available, self-validate:
- "What would a critic say about this?"
- "What evidence contradicts my conclusions?"
- "Where am I most likely wrong?"

### Phase 6: ACTIVATE
The brain is now consultable. When a question falls in this domain:
1. Read the relevant Brain Module
2. Apply its decision framework
3. Cite principles and anti-patterns
4. Flag confidence level in response
5. Note if the question reveals a knowledge gap → research more

## Protocol: Consulting a Brain

When a question matches an existing brain domain:
1. Read `brains/DOMAIN-NAME.md`
2. Apply its framework to the question
3. Respond with calibrated confidence
4. If confidence is low on a sub-topic, say so and offer to research deeper
5. After answering, append to the brain's learning log if new insight emerged

## Confidence Levels

| Level | Symbol | Meaning | Research Hours |
|-------|--------|---------|---------------|
| Novice | 🔴 | Just started, surface knowledge | <1h |
| Beginner | 🟠 | Foundations laid, gaps remain | 1-3h |
| Intermediate | 🟡 | Solid understanding, some blind spots | 3-10h |
| Advanced | 🟢 | Deep knowledge, validated | 10-30h |
| Expert | 🔵 | Comprehensive, battle-tested | 30h+ |

Update confidence after each research session. Be honest — overconfidence is the worst anti-pattern.

## Brain Maintenance

During heartbeats or idle time:
- Check if any brain hasn't been updated in >7 days
- Run a quick search for recent developments
- Update the "Last Updated" field
- Evolve the learning log

## Quick Reference

```
brains/                          # All brain modules
brains/CRYPTO-INVESTMENT.md      # Example brain
brains/MOUNTAIN-SAFETY.md        # Example brain
brains/_INDEX.md                 # Index of all brains with status
```

For the brain template structure, read: `references/brain-template.md`
For research methodology details, read: `references/research-protocol.md`
