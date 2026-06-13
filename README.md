<div align="center">

<img src="https://img.shields.io/badge/status-private-black?style=flat-square" />
<img src="https://img.shields.io/badge/python-3.12+-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/fastapi-0.115+-009688?style=flat-square&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/next.js-15-000000?style=flat-square&logo=next.js&logoColor=white" />
<img src="https://img.shields.io/badge/neo4j-security_graph-4581C3?style=flat-square&logo=neo4j&logoColor=white" />
<img src="https://img.shields.io/badge/license-BSL_1.1-red?style=flat-square" />

# Capslogue

**Code-to-Cloud-to-Runtime Security Intelligence Platform**

_Security Graph · Attack Path Correlation · Runtime Forensics · AI-Agent Security · Event Timeline Intelligence_

</div>

---

## Overview

Capslogue is a graph-driven security intelligence platform built for modern software teams shipping code, cloud infrastructure, APIs, data pipelines, and AI agents at high speed.

Modern engineering has changed. Teams now rely on AI coding tools, cloud automation, CI/CD pipelines, MCP servers, non-human identities, and autonomous AI agents. That speed creates new blind spots: unsafe SQL queries, exposed APIs, overly broad IAM roles, poisoned prompts, risky MCP tools, sensitive data flowing into model context, ephemeral runtime evidence, and agent workflows that can act before a human ever sees the alert.

Most security tools still look at one layer at a time.

Capslogue looks at the full attacker path:

```text
source code -> dependency -> secret -> CI/CD -> container -> cloud asset
-> identity -> API -> workload -> runtime event -> data store -> AI agent action
```

The goal is to answer one question better than everyone else:

> _Can an attacker actually get from the internet to my crown jewels, and how?_

Capslogue is not just a scanner and not just an alert dashboard. It is a contextual security reasoning system that correlates code, cloud, identity, data, runtime behavior, AI systems, investigations, and business impact into a unified Security Graph.

---

## What Capslogue Does

Capslogue unifies AppSec, CNAPP, runtime defense, identity security, data security, AI/LLM security, agentic AI security, forensics, compliance, resilience, and event intelligence into one security operating system.

It helps teams determine:

- Whether a vulnerability is reachable from the internet.
- Whether it is exploitable in the deployed runtime.
- Which identity or non-human principal can amplify the attack.
- Which data, workloads, APIs, or business systems are exposed.
- Whether runtime activity confirms exploitation.
- Which team owns the fix.
- What evidence is needed for incident response, governance, and audits.

---

## Architecture

Capslogue is organized as a 10-layer platform:

| Layer | Name | Purpose |
| --- | --- | --- |
| L1 | Data Platform | PostgreSQL, Redis, Neo4j, pgvector, object storage, event stores |
| L2 | Ingestion | GitHub, GitLab, cloud accounts, Kubernetes, CI/CD, SaaS, runtime, MCP, sensors |
| L3 | Normalization & Enrichment | Universal entity model, CVE/EPSS/KEV, asset ownership, cloud/data context |
| L4 | Detection Engines | 35 specialized engines across AppSec, CNAPP, runtime, AI, governance, and resilience |
| L5 | Security Graph | Neo4j-powered attack path graph and blast-radius model |
| L6 | Risk & Prioritization | Exploitability, exposure, impact, confidence, business criticality |
| L7 | AI Reasoning | Agentic workflows, RAG, investigation reasoning, remediation planning |
| L8 | Orchestration | Scan workflows, policy gates, investigations, forensics, remediation handoffs |
| L9 | API & Gateway | FastAPI, WebSocket, MCP server, tenant isolation, policy APIs |
| L10 | Presentation | Next.js dashboard, CLI, VS Code extension, browser extension, reports |

---

## Detection Engine System

Capslogue has grown into a 35-engine security platform spanning 2026-ready security domains:

| Domain | Representative Engines |
| --- | --- |
| Code Security | SAST, SCA, Secrets, IaC, CI/CD, DAST, API Security |
| Cloud Security | CSPM, CIEM, CWPP, KSPM, ASM, Exposure Validation |
| Runtime Defense | RASP, WAAP, DDR, ITDR, CIRA, behavioral baselining |
| Data Security | DSPM, data access trail, data residency, sovereignty enforcement |
| Identity Security | Non-human identity security, cloud identity graph, privilege paths |
| AI Security | AI/LLM security, agentic AI security, MCP security, AgentSec Scan |
| Governance | AI governance, compliance mapping, auditor reports, evidence packs |
| Forensics & IR | Detection-time forensics, investigation workbench, OpenSRE-style RCA |
| Event Intelligence | Event Timeline Intelligence, incident stories, risk deltas, board packs |
| Strategic Engines | MCDR, DSCE, EDIE, CWSE, AIRE, firmware, IoT/OT, crypto/PQC |

Every engine is designed to emit normalized findings into the Security Graph so risks can be correlated across layers instead of triaged in isolation.

---

## Security Graph

The Security Graph is the core differentiator.

It models code, packages, repositories, APIs, secrets, containers, workloads, Kubernetes resources, cloud assets, IAM identities, non-human identities, SaaS apps, data stores, runtime events, AI agents, MCP servers, tools, memories, policy decisions, forensics packages, and investigation sessions.

This enables questions like:

- What attack paths connect this public endpoint to sensitive data?
- Which code vulnerability is deployed into which container and cloud workload?
- Which identity can turn a medium code issue into a critical cloud breach?
- Which AI agent can mutate production resources?
- Which MCP tool can expose secrets or execute shell commands?
- What changed since yesterday that increased risk?
- Which runtime detection has enough evidence for IR handoff?

---

## Event Timeline Intelligence

Event Timeline Intelligence, ETI, turns noisy security events into connected incident stories.

It ingests findings, runtime events, cloud logs, SaaS logs, deployments, identity activity, forensics packages, investigations, policy decisions, and AI-agent actions into a canonical event lake with fingerprinting, deduplication, correlation, risk deltas, and narrative generation.

ETI is designed to produce:

- Top story and risk delta.
- Timeline graph APIs for UI.
- Incident story builder.
- Attack path and blast-radius enrichment.
- Investigation handoffs.
- Forensics evidence links.
- Owner, fix, SLA, and remediation progress.
- Daily, weekly, executive, compliance, and board-ready reports.

---

## Investigation Workbench

Capslogue includes an OpenSRE-inspired Investigation Workbench for bounded, evidence-driven security investigations.

The workflow is:

```text
alert/finding/event -> gather evidence -> form hypotheses -> validate
-> diagnose root cause -> report confidence -> recommend remediation
-> hand off to operator
```

It supports structured investigation state, audit lineage, follow-up sessions, streaming events, root-cause reports, blast-radius analysis, remediation plans, and next actions.

---

## Detection-Time Runtime Forensics

When a high-confidence runtime detection fires, Capslogue can capture evidence before the workload disappears.

Forensics packages include:

- Artifact manifests.
- Process and workload context.
- Cloud identity and audit trail.
- Network, DNS, file, image, SBOM, Kubernetes, and runtime metadata contracts.
- Chain-of-custody hashes.
- Retention and legal-hold states.
- Deterministic verdict, AI verdict, evidence confidence, reasoning confidence, and final verdict.
- IR-ready reports and investigation handoff.

---

## AI And Agentic Security

Capslogue treats AI agents as real non-human principals.

```text
Agent -> tool call -> process -> cloud API -> identity -> data/resource
```

The DE-34 Agentic AI Security Engine secures:

- AI agents, copilots, coding agents, SOC agents, and SaaS automation agents.
- MCP servers, tools, prompts, resources, transports, and tool metadata.
- Agent memories, skills, plugins, model gateways, and action chains.
- Cloud identities, service accounts, API tokens, and non-human identities.
- Sensitive data flows into model context and external output sinks.
- Runtime policy decisions, approvals, quarantines, and kill switches.
- Cost anomalies, retry loops, sub-agent fanout, and expensive model misuse.

---

## AgentSec Scan

AgentSec Scan is the open-source, developer-facing edge of Capslogue DE-34.

It runs locally inside any AI-agent codebase and generates a portable `.agentsec/security-graph.json` that captures agentic AI risks before agents receive production authority.

```text
AI-agent repo
-> /agentsec-scan
-> deterministic discovery
-> semantic review task packets
-> security graph
-> reviewable patch diffs
-> Capslogue import
```

AgentSec Scan detects:

- Prompt-injection and goal-hijacking paths.
- Unsafe LLM calls across OpenAI, Anthropic, Bedrock, Gemini, Cohere, LangChain, LangGraph, LlamaIndex, Semantic Kernel, CrewAI, AutoGen, and custom agents.
- Missing authorization on agent tools.
- Memory poisoning surfaces.
- MCP supply-chain risk and tool-description injection.
- Sensitive data reaching model context or external sinks.
- Shell/eval/subprocess execution surfaces.
- Secrets and credential-like material.
- AI governance evidence gaps.

It produces:

- `.agentsec/security-findings.json`
- `.agentsec/security-graph.json`
- `.agentsec/report.md`
- `.agentsec/data-flow-findings.json`
- `.agentsec/ai-system-card.json`
- `.agentsec/governance-findings.json`
- `.agentsec/runtime-instrumentation-plan.json`
- `.agentsec/policy-pack.json`
- `.agentsec/governance-approval-packet.json`
- `.agentsec/patches.patch`
- `.agentsec/capslogue-import.json`

AgentSec Scan is intentionally local/static. It does not claim runtime exploitability or legal approval by itself. Instead, it generates the evidence and handoff artifacts Capslogue needs for runtime enforcement, investigations, forensics, and AI governance.

---

## AI Governance

DE-35 AI Governance, Risk & Compliance Engine sits above DE-14, DE-27, DE-30, DE-33, and DE-34.

It is designed for:

- AI system registry: models, agents, RAG apps, copilots, workflows, MCP servers, gateways.
- Risk classification: EU AI Act, NIST AI RMF, ISO/IEC 42001, SOC 2 AI controls.
- Model cards, system cards, and agent cards.
- Lifecycle evidence: data provenance, evals, monitoring, rollback, human oversight, incidents.
- Approval workflows for AI system deployment.
- Continuous monitoring for prompt leakage, drift, unsafe tool use, data access, abuse, and cost runaway.
- Auditor reports: AI Act readiness, high-risk AI inventory, agent authority review, model risk register.

---

## MCP Integration

Capslogue includes a FastMCP server that exposes security capabilities to AI assistants and developer tools.

It also designs toward an MCP security proxy/interceptor model:

```text
AI host -> Sentra MCP proxy -> policy validation -> upstream MCP server
```

Target controls include pre-call validation, post-call evidence capture, tool-output quarantine, tool-description hashing, manifest scanning, dangerous tool detection, allowlist/denylist enforcement, and Sentra self-security checks.

---

## Compliance And Reporting

Capslogue maps findings, investigations, runtime evidence, forensics packages, policies, and governance artifacts to controls across:

**SOC 2 Type II** · **PCI DSS v4.0** · **HIPAA** · **GDPR** · **DORA** · **EU AI Act** · **NIST AI RMF** · **ISO/IEC 42001** · **CIS Benchmarks** · **NIST 800-53** · **MITRE ATT&CK**

The platform is designed to generate:

- Control evidence.
- Gap analysis.
- Risk movement reports.
- AI governance reports.
- Incident timelines.
- Board-ready summaries.
- Exportable JSON/HTML/PDF evidence packs.
- SHA-256 artifact integrity hashes.

---

## Technology Stack

| Area | Stack |
| --- | --- |
| Backend | Python 3.12+, FastAPI, SQLAlchemy 2.0 async, Alembic, Celery |
| Frontend | Next.js 15, React 19, TypeScript, Tailwind CSS v4 |
| Graph | Neo4j security graph |
| Datastores | PostgreSQL, Redis, pgvector, object storage contracts |
| AI | LangGraph-style orchestration, RAG, OpenAI, Anthropic, local-model ready architecture |
| Integrations | MCP, CLI, VS Code extension, browser extension, WebSocket APIs |
| Infrastructure | Docker, Kubernetes, Terraform, GitHub Actions |


---

## Development

```bash
make dev          # Start local infrastructure/services
make test         # Run tests
make lint         # Run linting
make migrate      # Run database migrations
make seed         # Seed sample data
```

AgentSec Scan local test:

```bash
node agentsec-scan/agentsec-scan-plugin/skills/agentsec-scan/run-agentsec-scan.mjs agentsec-scan/examples/vulnerable-agent --full
```

---

## Positioning

Capslogue is built around one belief:

> The alert is not the product. The connected investigation is the product.

The winning security platform is the one that can connect exposure, code, identity, cloud, data, runtime, AI agents, forensics, ownership, and remediation into a single explainable story.

---

## Status

This repository is private and under active development.

The architecture is intentionally broad. Engines are built incrementally, but the contracts, graph model, and orchestration patterns are designed for the full platform vision from day one.

---

## License

Business Source License 1.1. See [LICENSE](LICENSE).

<div align="center">

**Private repository — not accepting contributions at this time.**

</div>
