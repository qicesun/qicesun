# Qice Sun

**Senior Software Engineer @ Microsoft**  
GenAI Engineer building production LLM systems, enterprise AI infrastructure, and agentic platforms.

I work at the intersection of **LLM applications**, **agent protocols**, **enterprise RAG**, and **AI for operations** — turning prototypes into systems that are testable, maintainable, and safe enough for real users.

[Email](mailto:qicesun0401@gmail.com) · [GitHub](https://github.com/qicesun)

---

## Focus

- **Production LLM systems** — RAG, tool calling, guardrails, evaluation, observability, and lifecycle design.
- **Agent infrastructure** — MCP, multi-step workflows, memory, typed tools, and failure-aware orchestration.
- **Enterprise Java AI** — bringing modern AI capabilities into Spring Boot / JVM ecosystems.
- **AI for DevOps & SRE** — Kubernetes diagnosis, incident reasoning, Git/Jira correlation, and safe remediation loops.

---

## Open source leadership

I contribute to the **LangChain4j** ecosystem with a focus on infrastructure-level work that expands what Java AI applications can do in production.

### Model Context Protocol for Java

Led and delivered key pieces of the Java MCP server path across LangChain4j and LangChain4j Community:

- Shared MCP protocol DTOs and stdio JSON-RPC transport foundations.
- Community MCP server module exposing Java `@Tool` methods over MCP.
- Java stdio MCP server example and documentation for Claude Desktop-style usage.
- Lifecycle hardening such as clean stdio shutdown support.

### Enterprise agent tooling

Built agent-ready integrations that connect LLMs to enterprise systems:

- **Jira Tool** — search, create, comment, ADF parsing, robust agent-facing errors.
- **Web Scraper Tool** — lightweight HTML-to-Markdown extraction with context-noise reduction.
- **Confluence / GitLab Document Loaders** — resilient enterprise knowledge ingestion for RAG.

### Guardrails & framework correctness

- Built prompt repetition components for AI Services and RAG: policies, input guardrails, query transformers, AUTO-mode gates, idempotence, and docs.
- Fixed LangChain4j AI Services guardrail ordering so multimodal input is materialized before guardrail execution.

---

## Selected projects

### [SRE-Agent-App](https://github.com/qicesun/SRE-Agent-App)

Autonomous AI SRE agent for Kubernetes, built with **Java, Spring Boot, LangChain4j, Fabric8, GitLab, Jira, and web tooling**.

It implements an **OODA loop** for incident response:

> observe cluster state → orient with logs and code context → decide remediation/escalation → act through bounded tools

This is my reference project for production-style agent design: scoped tools, session state, operator-facing UX, incident context, and safe action boundaries.

### [chaos-swarm](https://github.com/qicesun/chaos-swarm)

Synthetic user swarm for UX chaos testing.  
A TypeScript/Next.js agent workspace that sends browser-driven personas through public web flows and turns user friction into inspectable reports.

### [cna-racing](https://github.com/qicesun/cna-racing)

Product engineering contributions across auth, profiles, driver UX, Supabase-backed signup, iRacing result import, DB-first standings, admin workflows, and testing.

---

## Technical range

| Area | Stack |
| --- | --- |
| AI systems | LangChain4j, LangGraph, LlamaIndex, MCP, RAG, guardrails, tool calling |
| Backend | Java, Spring Boot, Python, REST APIs, Kafka, Redis |
| Product | TypeScript, Next.js, Tailwind CSS, Playwright, Vercel |
| Infra | Kubernetes, Docker, Azure AKS, Supabase, Prometheus, Grafana, OpenTelemetry |
| Knowledge systems | Jira, Confluence, GitLab, web ingestion, document loaders, query transformation |

---

## Engineering principles

- Build the **platform**, not just the demo.
- Prefer **clear contracts, test coverage, and operational visibility** over clever abstractions.
- Design agents with **bounded tools, graceful failures, and reviewable actions**.
- Keep interfaces simple; move complexity into well-tested infrastructure.

---

For collaboration on production LLM systems, Java AI infrastructure, MCP, enterprise RAG, or AI for SRE:  
**qicesun0401@gmail.com**
