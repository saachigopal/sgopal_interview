# Scope — AI Agent Observability

A lightweight SaaS dashboard that gives developers out-of-the-box observability when creating a new AI agent. No build step, no install — just open `index.html` in any browser.

## What it does

**Agent creation** — create an agent with a name, model, and an optional observability toggle. When enabled, an OpenTelemetry configuration is auto-generated alongside the agent.

**Overview** — see model, total token usage, and estimated cost at a glance, with a prompt/completion token breakdown.

**Evaluation** — upload a golden dataset (JSON array of `{ input, expected_output }` pairs) to score agent responses, and run functional tests using pre-built checks (safety, latency, PII detection, groundedness) or custom developer-written assertions.

**Logs** — upload OpenTelemetry-formatted JSON logs to populate dashboard metrics.

## Screenshots

**Agent list** — all configured agents with model, observability status, and cost at a glance.
![Agent list](UI%20Screenshots/Screenshot%202026-04-17%20at%204.36.24%E2%80%AFPM.png)

**Create agent** — name, model selection, and a prominent observability toggle that auto-generates an OTel config.
![Create agent](UI%20Screenshots/Screenshot%202026-04-17%20at%204.36.31%E2%80%AFPM.png)

**Overview tab** — model, total token usage, estimated cost, and a prompt/completion token breakdown.
![Overview](UI%20Screenshots/Screenshot%202026-04-17%20at%204.37.52%E2%80%AFPM.png)

**Evaluation tab** — golden dataset scores and functional test results (pre-built + custom assertions).
![Evaluation](UI%20Screenshots/Screenshot%202026-04-17%20at%204.38.06%E2%80%AFPM.png)

**Logs tab** — OTel log upload with schema reference.
![Logs](UI%20Screenshots/Screenshot%202026-04-17%20at%204.38.32%E2%80%AFPM.png)

**Log preview** — inspect raw OTel JSON directly in the dashboard.
![Log preview](UI%20Screenshots/Screenshot%202026-04-17%20at%204.39.00%E2%80%AFPM.png)

**No observability state** — empty state for agents created without observability enabled.
![No observability](UI%20Screenshots/Screenshot%202026-04-17%20at%204.39.12%E2%80%AFPM.png)

## How to run

```
open index.html
```

No dependencies, no npm, no build step. React and Tailwind load via CDN.

## Stack

- React 18 (CDN)
- Tailwind CSS (CDN)
- Vanilla JS — single `index.html`, no framework
