# Scope — AI Agent Observability

A lightweight SaaS dashboard that gives developers out-of-the-box observability when creating a new AI agent. No build step, no install — just open `index.html` in any browser.

## What it does

**Agent creation** — create an agent with a name, model, and an optional observability toggle. When enabled, an OpenTelemetry configuration is auto-generated alongside the agent.

**Overview** — see model, total token usage, and estimated cost at a glance, with a prompt/completion token breakdown.

**Evaluation** — upload a golden dataset (JSON array of `{ input, expected_output }` pairs) to score agent responses, and run functional tests using pre-built checks (safety, latency, PII detection, groundedness) or custom developer-written assertions.

**Logs** — upload OpenTelemetry-formatted JSON logs to populate dashboard metrics.

## How to run

```
open index.html
```

No dependencies, no npm, no build step. React and Tailwind load via CDN.

## Stack

- React 18 (CDN)
- Tailwind CSS (CDN)
- Vanilla JS — single `index.html`, no framework
