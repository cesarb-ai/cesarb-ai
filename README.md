# Cesar B — Senior AI Engineer @ Coinbase

**Production agents that survive on-call.**

Senior AI Engineer at Coinbase. I design and ship LangGraph and Claude Agent SDK systems — checkpointing, evals, sandbox tooling — so agents run like services, not demos.

**Site:** [cesarb.ai](https://www.cesarb.ai) · **Projects:** [cesarb.ai/projects](https://www.cesarb.ai/projects) · **LinkedIn:** [longlivecesar](https://www.linkedin.com/in/longlivecesar/)

---

## Featured Production Systems

### Autonomous Onboarding Agent (Vision + Web Browsing)

- **Context**: At Coinbase, customer onboarding was time-intensive and brittle across real product UIs.
- **Role**: As part of the internal [AI Tiger Team](https://www.coinbase.com/blog/building-enterprise-AI-agents-at-Coinbase), I architected and led an **autonomous onboarding agent** that combines vision (UI understanding) with web-browsing to navigate and complete onboarding workflows.
- **Architecture**: Multi-agent **LangGraph** orchestration, **LangSmith** observability, tool-augmented browsing, and policy-guarded actions — integrated via **Kafka**, **Golang**, and **Python** services, with **Postgres** for state and checkpointing.
- **Impact**: Findings and results save hundreds of hours monthly.

### Docs-Quality Agent (Claude Agent SDK)

- **Context**: Developer docs drift from reality — examples break, commands rot, and support burden grows.
- **Role**: Built a **secure docs-quality agent** on the **Claude Agent SDK** that reads developer documentation and **runs it in a sandbox the way a developer would**, to catch docs drift before customers hit it.
- **Architecture**: Sandboxed docs execution → drift detection → automatic **Linear** issues and **GitHub PRs** that remediate the drift.
- **Why it matters**: Treats docs as executable contracts, not static pages — with the same service discipline as production agents (sandboxing, evals, actionable remediation).

### Enterprise KB Engine & RAG Playground

- **Context**: Teams needed a reliable way to prototype and harden **RAG pipelines** over heterogeneous, evolving knowledge bases (docs, wikis, tickets, code, internal tools).
- **Role**: Designed and built a **Knowledge Base Engine (KB Engine)** and public **[KB Engine Playground](https://github.com/cesarb-ai/kb_engine_playground)** for standing up, iterating on, and evaluating production-ready RAG pipelines.
- **Architecture**: Config-driven ingestion (**Fetch → Parse → Chunk → Embed**), vector + symbolic retrieval, pluggable rerankers, and **LangGraph** flows for multi-hop queries — backed by **Postgres/pgvector**, with **Kubernetes** scheduled jobs and chart-driven configs.
- **Impact**: Faster RAG iteration, objective retrieval evaluation, and a clearer path from playground experiments into hardened enterprise RAG services.

---

**Also:** local↔production eval loops (Mac Mini + [DGX Spark](https://github.com/cesarb-ai/dgx-spark-cluster-compass) vs LangSmith production traces) · CDP AI Support (LangChain Interrupt)

**Stack:** LangGraph · Claude Agent SDK · LangChain · LangSmith · Postgres/pgvector · Kafka · Golang · Python · K8s · evals / observability

---

## Open to

- **Staff / Principal AI Engineer** (full-time) — primary
- Select advisory / fractional on production agents

---

## Pin these

1. This profile README
2. `dgx-spark-cluster-compass`
3. `kb_engine_playground`
