# Cesar B — Senior AI Engineer @ Coinbase

**Production agents that survive on-call.**

Senior AI Engineer at Coinbase. I design and ship LangGraph and Claude Agent SDK systems — checkpointing, evals, sandbox tooling — so agents run like services, not demos.

**Site:** [cesarb.ai](https://www.cesarb.ai) · **Projects:** [cesarb.ai/projects](https://www.cesarb.ai/projects) · **LinkedIn:** [longlivecesar](https://www.linkedin.com/in/longlivecesar/)

---

## Featured Production Systems

### Autonomous Onboarding Agent (Vision + Web Browsing)

- **Context**: At Coinbase, onboarding customers was a time intensive process.
- **Role**: As part of an internal **AI Tiger Team**, I architected and led the development of an **autonomous onboarding agent** that combines vision (UI understanding) with web-browsing capabilities to navigate expedite customer onboarding.
- **Architecture**: Multi-agent **LangGraph** orchestration, **LangSmith**-driven observability, tool-augmented browsing, and policy-guarded actions. Integrated with internal services via **Kafka**, **Golang**, and **Python** microservices, with **Postgres** for state and checkpointing.
- **Impact**: The agent's findings and results **saves hundreds of hours monthly**.
- **Keywords**: autonomous AI agents, enterprise AI agents, AI agent building, LangGraph in production, agentic workflows, observability-first design.

### Docs-Quality Agent (Claude Agent SDK)

- **Context**: Developer docs drift from reality — examples break, commands rot, and support burden grows.
- **Role**: Built a **secure docs-quality agent** on the **Claude Agent SDK** that reads developer documentation and **runs it in a sandbox the way a developer would**, to catch docs drift before customers hit it.
- **Architecture**: Sandboxed docs execution → drift detection → automatic **Linear** issues and **GitHub PRs** that remediate the drift.
- **Why it matters**: Treats docs as executable contracts, not static pages — with the same service discipline as production agents (sandboxing, evals, actionable remediation).

### Enterprise KB Engine & RAG Playground (Knowledge Base Engine)

- **Context**: Teams needed a reliable way to prototype and harden **RAG pipelines** over heterogeneous, evolving knowledge bases (docs, wikis, tickets, code, internal tools).
- **Role**: I designed and built a **Knowledge Base Engine (KB Engine)** and public **KB Engine Playground** that make it easy to stand up, iterate on, and evaluate production-ready RAG pipelines.
- **Architecture**: Config-driven ingestion graph that automates **Fetch → Parse → Chunk → Embed**, combining **vector + symbolic retrieval**, pluggable rerankers, and **LangGraph-based flows** for complex multi-hop queries. Backed by **Postgres/pgvector**, orchestrated via **Kubernetes** scheduled jobs and chart-driven configs.
- **Impact**: Enabled rapid iteration on RAG strategies, objective evaluation of retrieval performance, and smoother promotion from “playground” experiments into hardened **enterprise RAG services**.
- **Links**:
  - **KB Engine Playground (GitHub)**: [`github.com/cesarb-ai/kb_engine_playground`](https://github.com/cesarb-ai/kb_engine_playground)
  - **Repo in this workspace**: `./kb_engine_playground`
- **Keywords**: enterprise RAG, knowledge base engine, automated RAG pipelines, pgvector, LangGraph RAG, retrieval evaluation, knowledge management.

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
