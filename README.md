# Subhajit Das

**GTM AI Infrastructure Builder** | LLM Routing | Cost Optimization | Open-source Systems

---

## A3M Router: Adaptive Multi-Model LLM Routing

**The fastest way to cut AI costs without sacrificing quality.**

A3M Router is an open-source LLM gateway that automatically routes requests to the cheapest capable provider — saving you up to 99.7% on API costs while maintaining the same quality.

### Quick Start

```bash
npm install adaptive-memory-multi-model-router
npx a3m-router serve
```

Then use it like OpenAI (drop-in replacement):

```python
from openai import OpenAI
client = OpenAI(base_url="http://localhost:8787/v1")
response = client.chat.completions.create(
    model="auto",
    messages=[{"role": "user", "content": "..."}]
)
```

### Real Results

| Query Type | Without Routing | A3M Routes To | Savings |
|---|---|---|---|
| Simple lookup ("What is 2+2?") | GPT-4o ($0.03) | Groq ($0.0001) | **99.7%** |
| Knowledge ("Explain quantum") | GPT-4o ($0.03) | Mistral ($0.0002) | **99.3%** |
| Code generation | GPT-4o ($0.05) | DeepSeek ($0.002) | **96%** |
| Complex reasoning | GPT-4o ($0.15) | GPT-4o ($0.15) | 0% (correctly routed) |

**Evidence:** See full routing benchmarks in [eval/results/report_latest.md](https://github.com/Das-rebel/a3m-router/blob/main/eval/results/report_latest.md)

### Key Features

- **80+ providers** — Groq, Mistral, DeepSeek, GPT-4o, Claude, Ollama, and more
- **Automatic routing** — Semantic analysis + ML decision head (`model="jev-auto"`)
- **Failover resilience** — If one provider fails, automatically route to another
- **Semantic caching** — Reduce repeat queries to zero cost
- **Self-hosted** — No API key sharing, no vendor lock-in (Docker + Node.js + Python)
- **Production-ready** — 49k npm downloads, 16 GitHub stars, active development

**Repository:** https://github.com/Das-rebel/a3m-router  
**npm package:** https://www.npmjs.com/package/adaptive-memory-multi-model-router  
**Homepage:** https://www.npmjs.com/package/adaptive-memory-multi-model-router

---

## The Problem It Solves

Most AI products send every request to the same expensive model:

✗ **GPT-4o costs $0.03 per request** — whether it's "What's the weather?" or "Solve a differential equation"  
✗ **Vendor lock-in** — If OpenAI is down, your product breaks  
✗ **No fallback** — You're one provider's outage away from downtime  

A3M Router solves this by:

✓ Routing simple queries to cheap providers (saves 99%)  
✓ Routing complex queries to capable models (no quality loss)  
✓ Supporting 80+ providers with automatic failover  
✓ Running entirely on your infrastructure  

---

## Platform Integration

**A3M Kong Plugin** — Routes LLM requests through A3M Router in Kong API Gateway  
Repository: https://github.com/Das-rebel/a3m-kong-plugin

---

## Market Knowledge

These curated lists track the broader AI infrastructure ecosystem:

- **Awesome AI Gateway** — Comparison of 100+ AI gateways, proxies, and LLM infrastructure
- **Awesome AI Model Routing** — Routing patterns, orchestration, and inference optimization
- **Awesome CLI Coding Agents** — Terminal-native AI agents and developer tooling

---

## Background

- 10+ years in growth, strategy, and product across fintech and AI infrastructure
- Research-focused approach to systems architecture and applied strategy
- Based in Bangalore

---

## Connect

**For partnerships, collaborations, or questions:**

- **GitHub:** https://github.com/Das-rebel
- **A3M Router:** https://github.com/Das-rebel/a3m-router
- **LinkedIn:** https://linkedin.com/in/subhajitd
- **X / Twitter:** https://twitter.com/Subholearns

---

**Open-source LLM routing. Self-hosted. No vendor lock-in. Production-ready.**
