# Career Progression Guide — AI Engineering

A career-ladder guide for the discipline of **building with AI models** — shipping LLM applications, agents, and multi-agent platforms that consume models through APIs rather than training them. This guide maps the eight roles in the AI Engineering Curriculum — a four-rung **agentic ladder** plus four **specialist tracks** — the skills that separate them, and how to progress through the authored learning tracks.

## Career Ladder Overview

```
        ┌──────────────────────────────────────────────┐
  L48   │  Agentic Systems Architect                    │   12+ yrs
        │  orchestration topology · durable execution   │
        └──────────────────────────────────────────────┘
                          ▲
        ┌──────────────────────────────────────────────┐
  L40   │  Senior Agentic AI Engineer                   │   8–12 yrs
        │  eval/observability infra · multi-agent scale │
        └──────────────────────────────────────────────┘
                          ▲
        ┌──────────────────────────────────────────────┐
  L30   │  Agentic AI Engineer                          │   4–8 yrs
        │  ReAct loops · RAG & memory · agent frameworks│
        └──────────────────────────────────────────────┘
                          ▲
        ┌──────────────────────────────────────────────┐
  L20   │  Agentic AI Developer                         │   0–4 yrs
        │  LLM APIs · prompting · tool/function calling │
        └──────────────────────────────────────────────┘
```

| Level | Role | Typical experience band |
|-------|------|--------------------------|
| L20 | Agentic AI Developer | 0–4 years |
| L30 | Agentic AI Engineer | 4–8 years |
| L40 | Senior Agentic AI Engineer | 8–12 years |
| L48 | Agentic Systems Architect | 12+ years |

Experience bands are directional. This discipline rewards demonstrated shipping of agentic systems over raw tenure — strong builders compress these timelines.

**Specialist tracks** branch off the ladder for engineers who want depth in one area: **LLM Application Developer** (L20), and **AI Evaluation Engineer**, **Applied AI Engineer**, and **RAG & Retrieval Engineer** (L30). See [Specialist Roles](#specialist-roles) below.

## Level Descriptions

### L20 — Agentic AI Developer

**Responsibilities.** Build and ship a first generation of LLM-powered features. Call model APIs reliably, design prompts that hold up in production, parse structured output, and wire up tool/function calling for simple workflows.

**Representative work.** A customer-support assistant backed by a single LLM with function calling; a document-summarization endpoint with structured JSON output; a first retrieval-augmented Q&A prototype over a small corpus.

**Technical depth.** Fluency with at least one model provider's API (chat, streaming, tool calls), prompt engineering fundamentals, structured output via schemas, token/cost awareness, and retrieval basics (chunking, embeddings, top-k). Understands the difference between a prompt that demos well and one that survives real input distributions.

### L30 — Agentic AI Engineer

**Responsibilities.** Own production agents end to end. Design ReAct-style loops, integrate agent frameworks, build real RAG and memory systems, compose multi-agent workflows, and put evaluation and guardrails around them.

**Representative work.** A multi-step research agent on LangGraph with persistent memory and a retrieval layer; a harness (instruction files, hooks, permissions, evals) that makes a coding agent reliable in a real repo — or a custom harness built from scratch; a CrewAI/AutoGen multi-agent pipeline with role specialization; an eval suite that gates prompt and model changes; input/output guardrails for safety and policy.

**Technical depth.** ReAct and planning loops, framework internals (LangGraph/CrewAI/AutoGen), retrieval strategy (hybrid search, re-ranking, chunk design), short- and long-term memory, offline/online evaluation, and guardrail patterns. Reasons about failure modes — loops that don't terminate, retrieval that misleads, tools that misfire.

### L40 — Senior Agentic AI Engineer

**Responsibilities.** Build the infrastructure other engineers' agents depend on. Own evaluation and observability platforms, run multi-agent systems at scale, and lead on reliability, cost, and incident response. Provide technical leadership across teams.

**Representative work.** A trace-and-eval observability stack (tracing, scoring, regression detection) used org-wide; a multi-agent platform handling high concurrency with cost controls; an on-call/incident-response practice for agent failures; mentorship and technical direction for several agent teams.

**Technical depth.** Eval/observability infrastructure design, distributed agent execution, latency/cost/quality trade-off management, reliability engineering for nondeterministic systems, and incident response for agentic failures. Sets standards rather than following them.

### L48 — Agentic Systems Architect

**Responsibilities.** Define the architecture for agentic systems across an organization. Choose orchestration topologies, design memory/context and eval/observability as platform layers, set security and governance boundaries, and establish durable-execution foundations and internal developer platforms.

**Representative work.** An organization-wide agent platform with a chosen orchestration topology (hierarchical, blackboard, graph), a durable-execution layer for long-running workflows, a shared memory/context architecture, and a security/governance model for tool access and data flow — exposed to product teams as an agentic developer platform.

**Technical depth.** Orchestration topology design, context/memory architecture, eval/observability as first-class platform concerns, security and governance for agentic systems, durable and recoverable execution, and platform engineering for agent developers. Operates at the intersection of architecture, reliability, and organizational strategy.

## Specialist Roles

### L20 — LLM Application Developer

**Focus.** Ship product-facing LLM features without needing a full agent stack: prompt engineering, tool and function calling, streaming and async orchestration, model selection with cost and prompt caching, retrieval basics, minimal evals and regression checks, and shipping a first feature.

### L30 — AI Evaluation Engineer

**Focus.** Make quality measurable inside the product: product-shaped eval design, trace instrumentation, trajectory and tool-call evals, LLM-as-judge in production, RAG evaluation at the app layer, eval-gated CI/CD, online evaluation and regression detection, guardrail evals, and human review workflows.

### L30 — Applied AI Engineer

**Focus.** Embed AI into existing products and workflows: AI feature design, production prompting and structured outputs, RAG integrated into the product, tool calling and orchestration, shipping product agents, feature-side evaluation, and guardrails on the user-facing surface.

### L30 — RAG & Retrieval Engineer

**Focus.** Own retrieval quality: retrieval engineering foundations, document ingestion and chunking, embedding selection and benchmarking, vector databases and ANN tuning, Lucene-family search and learning-to-rank, hybrid retrieval with fusion and query rewriting, and reranking.

## Skills Matrix by Level

| Skill Area | L20 Developer | L30 Engineer | L40 Senior | L48 Architect |
|------------|---------------|--------------|------------|---------------|
| LLM APIs | Calls chat/streaming/tools reliably | Optimizes provider mix, caching, fallbacks | Sets provider strategy & cost controls | Defines model-access platform & abstractions |
| Prompting | Solid prompt patterns | Systematic prompt design + testing | Prompt-as-config governance | Org prompt standards & libraries |
| Structured Output | Schema-constrained JSON | Robust parsing, validation, repair | Output contracts across services | Output schema governance |
| RAG & Memory | Retrieval basics, top-k | Hybrid search, re-ranking, memory | Retrieval/memory infra at scale | Memory/context architecture |
| Agent Frameworks | — (aware) | LangGraph/CrewAI/AutoGen in prod | Framework selection & extension | Orchestration framework strategy |
| Multi-Agent | — | Builds multi-agent workflows | Runs multi-agent at scale | Designs orchestration topology |
| Eval & Observability | Token/cost awareness | Offline/online eval + guardrails | Owns eval/observability infra | Eval/observability as platform |
| Architecture | Single-feature design | Production agent design | Cross-team system design | Org-wide agentic architecture |
| Leadership | Individual contributor | Owns features/agents | Mentors, sets standards | Sets technical direction |

## Compensation Ranges (United States, 2026)

Applied AI and LLM engineering skews high relative to general software roles; demand outpaces supply for engineers who can ship reliable agents. Bands are total compensation (base + bonus + equity).

| Level | Role | Total comp (USD) |
|-------|------|------------------|
| L20 | Agentic AI Developer | $130k – $190k |
| L30 | Agentic AI Engineer | $180k – $290k |
| L40 | Senior Agentic AI Engineer | $280k – $450k |
| L48 | Agentic Systems Architect | $400k – $700k+ |

The four specialist roles are not yet benchmarked here.

**Variance.** These figures reflect major US tech hubs (SF Bay Area, NYC, Seattle). Other metros typically run 10–25% lower. Company type matters more than level: frontier labs and well-funded AI startups can exceed the top of each band substantially (especially on equity), while non-tech enterprises and agencies often sit at or below the floor. Specialized eval/observability and agent-platform skill sets command a premium within each band.

## Promotion Criteria

**L20 → L30 (Developer → Engineer).** Has shipped at least one production LLM feature with tool calling and retrieval. Can now design an agent — not just a prompt — including ReAct loops, a real RAG/memory layer, and an evaluation harness that gates changes. Demonstrates ownership of an agent in production, not just a prototype.

**L30 → L40 (Engineer → Senior).** Has run agents in production at meaningful scale and reliability. Builds infrastructure others depend on (eval, observability, guardrails as shared services), leads on cost/latency/reliability trade-offs, handles agent incidents, and provides technical leadership and mentorship beyond their own work.

**L40 → L48 (Senior → Architect).** Has set architecture for agentic systems spanning multiple teams. Chooses orchestration topology and durable-execution strategy, designs memory/context and eval/observability as platform layers, owns security and governance for agentic systems, and delivers an internal agentic developer platform that raises the whole org's velocity.

## Learning Paths

Each role has a paired **-learning** repo (authored modules) and a **-solutions** repo (reference implementations). The agentic ladder is sequential — each rung assumes fluency with the one below it. Specialist tracks can be taken after the rung they branch from.

1. **Start at L20** — work through [`agentic-ai-developer-learning`](https://github.com/ai-engineering-curriculum/agentic-ai-developer-learning), checking your work against [`agentic-ai-developer-solutions`](https://github.com/ai-engineering-curriculum/agentic-ai-developer-solutions). Goal: ship a first LLM app with tool calling and basic retrieval.
2. **Advance to L30** — [`agentic-ai-engineer-learning`](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-learning) with [`agentic-ai-engineer-solutions`](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-solutions). Goal: production agents with frameworks, RAG/memory, multi-agent workflows, evaluation, and guardrails.
3. **Move to L40** — [`senior-agentic-ai-engineer-learning`](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-learning) with [`senior-agentic-ai-engineer-solutions`](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-solutions). Goal: eval/observability infrastructure, multi-agent at scale, reliability, and technical leadership.
4. **Reach L48** — [`agentic-systems-architect-learning`](https://github.com/ai-engineering-curriculum/agentic-systems-architect-learning) with [`agentic-systems-architect-solutions`](https://github.com/ai-engineering-curriculum/agentic-systems-architect-solutions). Goal: orchestration topology, memory/context architecture, security/governance, durable execution, and agentic developer platforms.

Work the learning modules first; consult the solutions repo only after a genuine attempt. The gap between your implementation and the reference is where the learning lives.

## Specialist Tracks

Beyond the linear ladder, specialist tracks let engineers go deep in one area rather than broad across all of them.

- **LLM Application Developer** *(available, L20)* — product-facing LLM apps: prompting, tool calling, streaming, cost, and shipping. Branches from the start of the ladder.
- **AI Evaluation Engineer** *(available, L30)* — evaluation methodology, tracing, and quality gates for nondeterministic systems.
- **Applied AI Engineer** *(available, L30)* — embedding AI into existing products and business workflows.
- **RAG & Retrieval Engineer** *(available, L30)* — retrieval quality, hybrid search, reranking, and knowledge systems at scale.
- **Agent Platform Engineer** *(planned)* — internal platforms, orchestration runtimes, and durable execution for agent developers. Until it's authored, pursue this through the L40 and L48 tracks and the Agentic AI Engineer's harness-engineering modules.

## Repository Map

All repositories live under the [`ai-engineering-curriculum`](https://github.com/ai-engineering-curriculum) GitHub organization. Every role has a paired `-learning` repo (modules, lecture chapters, exercises) and a `-solutions` repo (reference walkthroughs).

| Level | Role | Modules | Learning | Solutions | Status |
|---|---|---|---|---|---|
| L20 | Agentic AI Developer | 6 | [agentic-ai-developer-learning](https://github.com/ai-engineering-curriculum/agentic-ai-developer-learning) | [agentic-ai-developer-solutions](https://github.com/ai-engineering-curriculum/agentic-ai-developer-solutions) | Complete |
| L20 | LLM Application Developer | 7 | [llm-application-developer-learning](https://github.com/ai-engineering-curriculum/llm-application-developer-learning) | [llm-application-developer-solutions](https://github.com/ai-engineering-curriculum/llm-application-developer-solutions) | Authored · 1 module's solutions pending |
| L30 | AI Evaluation Engineer | 12 | [ai-eval-engineer-learning](https://github.com/ai-engineering-curriculum/ai-eval-engineer-learning) | [ai-eval-engineer-solutions](https://github.com/ai-engineering-curriculum/ai-eval-engineer-solutions) | Authored · 1 module's chapters pending |
| L30 | Agentic AI Engineer | 9 | [agentic-ai-engineer-learning](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-learning) | [agentic-ai-engineer-solutions](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-solutions) | Complete |
| L30 | Applied AI Engineer | 12 | [applied-ai-engineer-learning](https://github.com/ai-engineering-curriculum/applied-ai-engineer-learning) | [applied-ai-engineer-solutions](https://github.com/ai-engineering-curriculum/applied-ai-engineer-solutions) | Complete |
| L30 | RAG & Retrieval Engineer | 13 | [rag-engineer-learning](https://github.com/ai-engineering-curriculum/rag-engineer-learning) | [rag-engineer-solutions](https://github.com/ai-engineering-curriculum/rag-engineer-solutions) | Authored · 1 module's solutions pending |
| L40 | Senior Agentic AI Engineer | 5 | [senior-agentic-ai-engineer-learning](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-learning) | [senior-agentic-ai-engineer-solutions](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-solutions) | Complete |
| L48 | Agentic Systems Architect | 10 | [agentic-systems-architect-learning](https://github.com/ai-engineering-curriculum/agentic-systems-architect-learning) | [agentic-systems-architect-solutions](https://github.com/ai-engineering-curriculum/agentic-systems-architect-solutions) | Complete |

## The AI Career Curriculum Ecosystem

AI Engineering is one of five sibling organizations in the AI Career Curriculum ecosystem. Each covers a distinct discipline in the AI stack:

- **[AI Engineering](https://github.com/ai-engineering-curriculum)** *(this org)* — **build WITH models.** Consume models through APIs and agents to ship LLM applications, RAG systems, and multi-agent platforms.
- **[ML Engineering](https://github.com/ml-engineering-curriculum)** — **build the models.** Train, fine-tune, and optimize the models themselves.
- **[AI Infrastructure](https://github.com/ai-infra-curriculum)** — **run the substrate.** Operate the platforms, compute, and serving infrastructure that everything else depends on.
- **[AI Governance](https://github.com/ai-governance-curriculum)** — **govern & assure.** Establish policy, risk, safety, and assurance across the stack.
- **[AI Startup](https://github.com/ai-startup-curriculum)** — **turn it into a company.** The startup operating school for technical founders.

**Where the boundary sits.** If you call a model's API and orchestrate it, you're in **AI Engineering**. If you train or fine-tune the weights, you're in **ML Engineering**. If you keep the GPUs, serving layers, and platforms running, you're in **AI Infrastructure**. The disciplines compose: an agent platform (AI Engineering) runs on infrastructure (AI Infra), may call models that someone trained (ML Engineering), all within governance boundaries (AI Governance).

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
