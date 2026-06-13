# Hi, I'm Keith (Qice) Sun 👋

**Senior GenAI Software Engineer at Microsoft**  
Building production-grade LLM applications, Java agent infrastructure, enterprise RAG, and AI-native developer/SRE workflows.

[![Email](https://img.shields.io/badge/Email-qicesun0401%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:qicesun0401@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-qicesun-181717?style=flat&logo=github)](https://github.com/qicesun)
[![Java](https://img.shields.io/badge/Java-17%2B-ED8B00?style=flat&logo=openjdk&logoColor=white)](#)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=flat&logo=springboot&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/TypeScript-Next.js-3178C6?style=flat&logo=typescript&logoColor=white)](#)
[![LangChain4j](https://img.shields.io/badge/LangChain4j-Enterprise%20Java%20AI-3B82F6?style=flat)](#)

---

## What I build

I focus on turning LLM ideas into **operational systems**:

- **Agentic workflows** that can observe, reason, decide, and act with tool-using loops.
- **Enterprise Java AI infrastructure** for LangChain4j, MCP, Jira, Confluence, GitLab, and web knowledge ingestion.
- **Production RAG systems** with document loaders, query transformers, guardrails, evaluation, and operational safety.
- **AI for DevOps / SRE**: Kubernetes incident diagnosis, Git correlation, Jira escalation, and self-healing workflows.
- **TypeScript product demos** that make AI systems inspectable through clean UX and fast iteration.

---

## Open source focus: LangChain4j & Java AI

I contribute heavily to the **LangChain4j ecosystem**, especially where Java applications meet enterprise knowledge systems and AI agent protocols.

### Model Context Protocol (MCP)

- Extracted shared MCP protocol DTOs and reusable stdio JSON-RPC transport helpers for LangChain4j.
- Built the community-side **stdio MCP server module**, enabling Java applications to expose `@Tool` methods to MCP clients such as Claude Desktop and IDE agents.
- Added lifecycle hardening such as `awaitClose()` for clean stdio server shutdown.
- Authored Java MCP server documentation and example flows for end-to-end Claude Desktop usage.

### Enterprise tools & RAG integrations

- Added **Jira Tool** support for LLM agents, including JQL search, issue retrieval, issue creation, comments, robust error handling, and ADF-to-text simplification.
- Added **Web Scraper Tool** with lightweight HTML-to-Markdown extraction and noise reduction for agent context.
- Added document loaders for **Confluence** and **GitLab**, including pagination, metadata extraction, branch fallback, URL normalization, and resilient API handling.
- Added stronger integration-test coverage for Jira tooling with real-LLM end-to-end scenarios.

### Guardrails, prompt repetition & framework correctness

- Implemented prompt repetition components for AI Services and RAG, including input guardrails, query transformation, AUTO-mode gates, idempotence, and rollout guidance.
- Fixed a LangChain4j framework ordering issue so input guardrails see materialized multimodal content after RAG augmentation and before model invocation.
- Documented the prompt repetition module and connected it to guardrails/RAG tutorials.

---

## Featured projects

### [SRE-Agent-App](https://github.com/qicesun/SRE-Agent-App)

> Autonomous AI SRE Agent for Kubernetes, built with Java, Spring Boot, and LangChain4j.

An AIOps framework that implements an **OODA loop** for incident response:

- **Observe:** inspect Kubernetes pods, workloads, restarts, and logs through Fabric8.
- **Orient:** correlate runtime failures with GitLab commits and external troubleshooting context.
- **Decide:** choose between safe remediation and escalation.
- **Act:** perform bounded remediation actions and create Jira incident tickets with rich context.

Tech: `Java 17`, `Spring Boot`, `LangChain4j`, `Kubernetes`, `Fabric8`, `GitLab API`, `Jira REST API`, `Jsoup`, `Tailwind CSS`.

### [chaos-swarm](https://github.com/qicesun/chaos-swarm)

> Synthetic user swarm UX chaos testing demo powered by cloud browsers and multi-agent simulation.

A TypeScript/Next.js workspace for releasing synthetic user agents against websites and converting user friction into structured reports.

Highlights:

- Agent runtime and persona layer for synthetic user behavior.
- Report generation for funnel friction, clustering, and UX failure inspection.
- Playwright-based local execution, with Browserbase / Supabase style cloud-runtime direction.

Tech: `TypeScript`, `Next.js`, `Playwright`, `Supabase`, `OpenAI`, `Browser automation`.

### [cna-racing](https://github.com/qicesun/cna-racing)

> Community racing platform work: authentication, driver profiles, standings, results, and admin import workflows.

I contributed a large sequence of product and platform PRs around:

- iRacing OAuth login and signed sessions.
- Public driver pages, editable profiles, hover cards, CNA badges, and driver UX.
- Supabase-backed signup and roster flows.
- iRacing result import, DB-first standings, result snapshots, and fallback handling.
- Test coverage and admin workflow improvements.

Tech: `TypeScript`, `Next.js`, `Supabase`, `Vercel`, `iRacing data workflows`.

---

## Selected upstream PR themes

| Area | Work |
| --- | --- |
| **MCP / Agent Protocols** | MCP protocol extraction, stdio JSON-RPC IO, community MCP server, Java MCP stdio examples, lifecycle fixes |
| **Enterprise Knowledge** | Confluence loader, GitLab loader, Jira tool, Web Scraper tool |
| **RAG & Guardrails** | Prompt repetition policy, input guardrails, query transformers, AUTO-mode gates, docs |
| **Framework Reliability** | Multimodal AI Services guardrail ordering fix, regression tests, robust error handling |
| **Product Engineering** | cna-racing auth, profiles, standings, result import, DB-first data flows, UX polish |

---

## Technical stack

| Domain | Tools & Technologies |
| --- | --- |
| **Generative AI** | LangChain4j, LangGraph, LlamaIndex, vLLM, RAGAS, prompt engineering, tool calling |
| **Agent Systems** | MCP, OODA loops, AI Services, guardrails, memory, multi-step tool orchestration |
| **RAG / Knowledge** | Confluence, GitLab, Jira, web scraping, document loaders, query transformation, reranking |
| **Backend** | Java, Spring Boot, Python, REST APIs, Kafka, Redis |
| **Frontend / Product** | TypeScript, Next.js, Tailwind CSS, Playwright, Vercel |
| **Infra / Observability** | Kubernetes, Docker, Azure AKS, Prometheus, Grafana, OpenTelemetry, Supabase |

---

## Engineering style

- I prefer **small, reviewable PRs** with clear sequencing and follow-up plans.
- I design integrations to be **agent-safe**: predictable errors, bounded behavior, and testable contracts.
- I care about **operational usefulness** as much as model capability: logs, metadata, diagnostics, lifecycle hooks, and rollback paths.
- I like bridging ecosystems: bringing modern AI protocols and RAG patterns into **enterprise Java**.

---

## GitHub snapshot

<p align="left">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=qicesun&show_icons=true&theme=default&hide_border=true" alt="qicesun GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=qicesun&layout=compact&theme=default&hide_border=true" alt="qicesun top languages" />
</p>

---

## Let's connect

I'm interested in production LLM systems, Java AI infrastructure, enterprise RAG, MCP, AI agents, and AI for DevOps/SRE.

📬 **Email:** [qicesun0401@gmail.com](mailto:qicesun0401@gmail.com)
