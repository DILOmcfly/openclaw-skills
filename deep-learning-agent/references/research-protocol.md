# Research Protocol — Deep Methodology

## Search Strategy Matrix

For any topic, execute searches across these dimensions:

### Dimension 1: Breadth
```
"[topic] fundamentals"
"[topic] beginner guide 2026"
"[topic] comprehensive overview"
"[topic] wikipedia" OR "[topic] investopedia"
```

### Dimension 2: Depth (Expert Level)
```
"[topic] advanced strategies"
"[topic] professional techniques"
"[topic] expert tips 2026"
"[topic] research papers"
```

### Dimension 3: Anti-Patterns (Critical Learning)
```
"[topic] common mistakes"
"[topic] what I wish I knew before"
"[topic] biggest failures"
"[topic] myths debunked"
"[topic] reddit lessons learned"
```

### Dimension 4: Cutting Edge
```
"[topic] trends 2026"
"[topic] what changed recently"
"[topic] new developments"
"[topic] future predictions"
```

### Dimension 5: Community Wisdom
```
"site:reddit.com [topic] advice"
"[topic] twitter thread"
"[topic] real experience"
"[topic] case study"
```

## Source Quality Hierarchy

| Tier | Source Type | Trust Level | Use For |
|------|-----------|-------------|---------|
| 1 | Academic papers, official docs | Very High | Core principles |
| 2 | Established publications (Bloomberg, Nature) | High | Current data |
| 3 | Expert blogs, technical docs | Medium-High | Strategies |
| 4 | Reddit, forums (with votes) | Medium | Anti-patterns, real experiences |
| 5 | Social media, anecdotes | Low | Trends, signals |

Always cross-reference Tier 4-5 claims with Tier 1-3 sources.

## Research Session Structure

Each research session (~30-60 min of searches):

1. **Define scope** — What specific questions am I answering?
2. **Broad scan** — 5-10 searches across dimensions
3. **Deep dive** — Pick 3-5 best sources, read thoroughly (web_fetch)
4. **Synthesize** — Update the Brain Module
5. **Gap check** — What questions remain? Add to Open Questions
6. **Log** — Record what was learned in the Learning Log

## When to Stop Researching

Stop when:
- 3+ sources agree on the same principle → it's established
- New searches return info you already have → diminishing returns
- You can explain the topic to someone else → understanding achieved
- The Open Questions list is short and specific → major gaps closed

Continue if:
- Sources contradict each other → need resolution
- A sub-topic feels vague → need more depth
- The decision framework has gaps → need more conditions
- Confidence is still 🔴 or 🟠 → need more foundation

## Debate Protocol (Agent Adversarial)

When spawning agents for debate:

```
Task for adversarial agent:
"I am building expertise in [topic]. Here are my key conclusions:
[list 3-5 main conclusions]

Your job is to CHALLENGE these. For each conclusion:
1. Find evidence that contradicts it
2. Identify edge cases where it fails
3. Suggest a stronger version if possible

Be rigorous. Don't agree just to be nice."
```

After debate, update the Brain:
- Conclusions that survived → increase confidence
- Conclusions that were challenged → revise or add caveats
- New insights from debate → add to Learning Log
