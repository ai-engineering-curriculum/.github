# AI Engineering Curriculum

## ⚠️ AI-Generated Content Disclaimer

> The content in these repositories is generated with AI assistance and undergoes ongoing human review. It may contain errors or outdated information. Treat it as a learning resource: cross-reference official docs, test code in a safe environment, and report issues via GitHub Issues or Discussions.

---

> A hands-on, role-based curriculum for engineers who build with AI — LLM apps, RAG, agents, and multi-agent systems, from first app to systems architect.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/orgs/ai-engineering-curriculum/discussions)
[![Repositories: 16](https://img.shields.io/badge/repositories-16-blue.svg)](https://github.com/orgs/ai-engineering-curriculum/repositories)

## 🎯 Overview

This org covers **AI engineering** — *building with* the models: LLM application development, retrieval and RAG, agents and multi-agent systems, evaluation, guardrails, harness engineering, and production operations. Every role track has a paired **learning** repository (modules, lecture chapters, exercises, quizzes) and a **solutions** repository with reference walkthroughs.

**At a glance:**

- 🏢 **16 curriculum repositories** (8 learning + 8 solutions)
- 📚 **8 role tracks**
- 🤖 **Agentic track** of four rungs: Agentic AI Developer → Engineer → Senior → Systems Architect

## 🔗 Curriculum Family

One of 5 sibling orgs in the **AI Career Curriculum ecosystem**, organized by what you *do* relative to a model:

- **[AI Infrastructure Curriculum](https://github.com/ai-infra-curriculum)** — *run* the platforms (Kubernetes, GPUs, training infra, serving, MLOps, IaC, SRE).
- **[ML Engineering Curriculum](https://github.com/ml-engineering-curriculum)** — *build & train* the models (data, fine-tuning, pretraining, RLHF, evals).
- **AI Engineering Curriculum** *(you are here)* — *build with* the models (agentic apps, RAG, multi-agent systems).
- **[AI Governance Curriculum](https://github.com/ai-governance-curriculum)** — *govern & assure* AI (security, compliance, evaluation, safety).
- **[AI Startup Curriculum](https://github.com/ai-startup-curriculum)** — *turn it into a company* — the startup operating school for technical founders (functional curricula × role pathways × stages).

---

## 📚 Learning Tracks

### 🟢 Builder (L20)

| Role | Focus | Repositories |
|------|-------|--------------|
| **Agentic AI Developer** | LLM fundamentals, prompting & structured output, tool calling, retrieval basics, first agent, shipping | [📘 Learning](https://github.com/ai-engineering-curriculum/agentic-ai-developer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/agentic-ai-developer-solutions) |
| **LLM Application Developer** | Prompting, tool calling, streaming & async, model selection, prompt caching, retrieval, minimal evals | [📘 Learning](https://github.com/ai-engineering-curriculum/llm-application-developer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/llm-application-developer-solutions) |

### 🔵 Engineer (L30)

| Role | Focus | Repositories |
|------|-------|--------------|
| **AI Evaluation Engineer** | Trace instrumentation, trajectory & tool evals, LLM-as-judge, RAG evals, eval-gated CI/CD, online evals | [📘 Learning](https://github.com/ai-engineering-curriculum/ai-eval-engineer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/ai-eval-engineer-solutions) |
| **Agentic AI Engineer** | Agent loop, frameworks, RAG & memory, multi-agent, evals, guardrails, production, harness engineering | [📘 Learning](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/agentic-ai-engineer-solutions) |
| **Applied AI Engineer** | AI feature design, production prompting, RAG in product, orchestration, product agents, guardrails | [📘 Learning](https://github.com/ai-engineering-curriculum/applied-ai-engineer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/applied-ai-engineer-solutions) |
| **RAG & Retrieval Engineer** | Ingestion & chunking, embeddings, vector DBs & ANN tuning, learning-to-rank, hybrid retrieval, reranking | [📘 Learning](https://github.com/ai-engineering-curriculum/rag-engineer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/rag-engineer-solutions) |

### ⭐ Senior & Architect (L40+)

| Role | Focus | Repositories |
|------|-------|--------------|
| **Senior Agentic AI Engineer** | Agent systems from an architecture, eval & observability infra, multi-agent at scale, reliability, cost | [📘 Learning](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/senior-agentic-ai-engineer-solutions) |
| **Agentic Systems Architect** | When not to use an agent, orchestration & memory architecture, eval harnesses, security, durable execution | [📘 Learning](https://github.com/ai-engineering-curriculum/agentic-systems-architect-learning) · [✅ Solutions](https://github.com/ai-engineering-curriculum/agentic-systems-architect-solutions) |

---

## 🚀 Quick Start

1. **Choose a track** from the table above, based on your experience and direction.
2. **Clone its repository:**

   ```bash
   git clone https://github.com/ai-engineering-curriculum/agentic-ai-developer-learning.git
   cd agentic-ai-developer-learning
   ```

3. **Start with the first module** and read its `README.md`.
4. **Work through the exercises** in each module.
5. **Check the paired solutions repository** for reference walkthroughs.

---

## 🛠️ Technologies Covered

- **Model APIs:** Anthropic, OpenAI
- **Agent frameworks:** LangGraph, CrewAI, AutoGen, LangChain, LlamaIndex
- **Tools & protocols:** Model Context Protocol (MCP), Pydantic, FastAPI
- **Coding-agent harnesses:** Claude Code, Codex CLI, Claude Agent SDK
- **Retrieval:** pgvector, Chroma, Qdrant, BM25 hybrid search, reranking
- **Production:** Temporal, Docker, Kubernetes, GitHub Actions
- **Observability & evals:** OpenTelemetry, Langfuse, LangSmith, Phoenix, Ragas, Inspect
- **Safety & governance:** OWASP LLM Top 10, NIST AI RMF, EU AI Act

---

## 📈 Career Progression

See the **[Career Progression Guide](https://github.com/ai-engineering-curriculum/.github/blob/main/CAREER_PROGRESSION.md)** for level descriptions, a skills matrix, promotion criteria, and specialist tracks.

---

## 🤝 Contributing

Contributions are welcome across the organization:

- Fix broken links, stale references, or inaccurate explanations
- Add depth to modules, exercises, or projects
- Improve validation for runnable exercises
- Report issues or ideas via [GitHub Discussions](https://github.com/orgs/ai-engineering-curriculum/discussions)
- Follow the `CONTRIBUTING.md` in the specific repository you want to improve

---

## 📜 License

Curriculum repositories are MIT-licensed unless noted otherwise. See the target repository's `LICENSE` file for authoritative terms.

---

## 📞 Support

- **Issues:** use the relevant repository's GitHub Issues
- **Discussions:** [organization discussions](https://github.com/orgs/ai-engineering-curriculum/discussions)
- **Docs:** [Career Progression](https://github.com/ai-engineering-curriculum/.github/blob/main/CAREER_PROGRESSION.md)

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
