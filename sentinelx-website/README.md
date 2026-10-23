# SentinelX

**Organizational memory for production systems**

An AI-powered incident response agent that remembers how *your* organization solved problems before — powered by [Hindsight](https://hindsight.vectorize.io/) agent memory + Microsoft Azure.

## Quick Start

Open `index.html` in any modern browser (or serve with a static server):

```bash
open index.html
# or
npx serve .
# or
python3 -m http.server 8080
```

## Demo features

- **Incident journey** (not a chatbot): triage → recall → root cause → human approval → remediate → verify → retain
- **Memory ON/OFF toggle** — same scenario with vs without organizational memory (before/after)
- **Memories recalled for this reply** — evidence panel with similarity scores
- **Blast radius** panel — severity, services, error rate, affected users
- **Confidence levels** (HIGH / MEDIUM / LOW) with explainability
- **Human-in-the-loop approval** before remediation
- **Live remediation** with error rate dropping
- **Continuous learning** — save resolved incident back to memory bank
- **Learning curve** indicator (#1 Cold → #5 Warm → #20 Expert)
- **Before vs After** MTTR comparison

## Pitch

> Don’t troubleshoot from scratch. Remember.

An AI that doesn't just troubleshoot — it remembers how your organization solved problems before, explains the evidence, waits for approval, then learns from every resolution.

## Connecting a real backend

This is a front-end demonstration with simulated responses. For production:

1. Deploy [Hindsight](https://github.com/vectorize-io/hindsight)
2. Seed historical incidents via `retain()`
3. Use Azure OpenAI + Microsoft Agent Framework with HindsightProvider
4. Wire Azure Monitor alerts into the triage agent

## Links

- Hindsight Docs: https://hindsight.vectorize.io/
- Hindsight GitHub: https://github.com/vectorize-io/hindsight
