# Subhajit Das

GTM AI Infrastructure Builder. I design systems that route LLM requests intelligently — cutting costs, improving quality, and avoiding vendor lock-in.

## Flagship: A3M Router

**Adaptive multi-model LLM router that cuts your AI bill by 90% while maintaining quality.**

- Drop-in OpenAI API replacement
- Automatic routing to cheapest capable provider
- 80+ providers (Groq, Mistral, DeepSeek, GPT-4o, Claude, etc.)
- Self-hosted, no vendor lock-in
- 49k npm downloads (87% in Sep 2026)

**Try it in 30 seconds:**

```bash
npm install adaptive-memory-multi-model-router
npx a3m-router serve
```

Then use it like OpenAI:

```python
from openai import OpenAI
client = OpenAI(base_url="http://localhost:8787/v1")
response = client.chat.completions.create(
    model="auto",  # Routes to cheapest capable provider
    messages=[{"role": "user", "content": "..."}]
)
```

**Results:**
- "What is 2+2?" → $0.03 (GPT-4o) → $0.0001 (Groq) — **99.7% cheaper**
- "Explain quantum computing" → $0.03 (GPT-4o) → $0.0002 (Mistral) — **99.3% cheaper**
- Complex reasoning → correctly routes to GPT-4o, no overspend

📊 **Full README:** https://github.com/Das-rebel/a3m-router (includes benchmark harness, provider list, architecture)

---

## Why this matters

AI teams face three problems:

1. **Cost sprawl** — Every request costs the same whether it's a simple lookup or complex reasoning
2. **Vendor lock-in** — Relying on one provider (OpenAI) creates business risk
3. **Failover pain** — When a provider is down, your product breaks

A3M solves all three:
- Routes based on query complexity and cost
- Supports 80+ providers with fallback
- Runs on your infrastructure (Docker, Node.js, Python)

---

## Product + Platform

**A3M Router** — Open-source adaptive routing and model orchestration  
Repository: https://github.com/Das-rebel/a3m-router

**A3M Kong Plugin** — Kong API Gateway integration for LLM routing  
Repository: https://github.com/Das-rebel/a3m-kong-plugin

---

## Market Context

These are curated resources on AI infrastructure, gateways, and routing:

- **Awesome AI Gateway** — Comparison of AI gateways, proxies, and LLM infrastructure
- **Awesome AI Model Routing** — Routing patterns, orchestration, and optimization
- **Awesome CLI Coding Agents** — Terminal-native AI agents and tooling

---

## Background

- 10+ years in growth, strategy, and product (fintech, AI infrastructure)
- Research-focused approach to systems and decision-making
- Based in Bangalore

---

## Connect

- **GitHub:** https://github.com/Das-rebel
- **A3M Router:** https://github.com/Das-rebel/a3m-router
- **LinkedIn:** https://linkedin.com/in/subhojitd
- **X / Twitter:** https://twitter.com/Subholearns

---

**Building AI infrastructure for routing, failover, and intelligent model selection.**
