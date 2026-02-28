# Capslogue

<div align="center">

<img src="https://img.shields.io/badge/status-private-black?style=flat-square" />
<img src="https://img.shields.io/badge/python-3.12+-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/next.js-15-000000?style=flat-square&logo=next.js&logoColor=white" />
<img src="https://img.shields.io/badge/license-proprietary-red?style=flat-square" />

**Contextual Application Security Platform**

_Taint analysis · Attack path correlation · Exploit impact quantification · Runtime threat interception_

</div>

---

## Overview

Capslogue is an application security platform built for how software is actually written today.

Teams now rely heavily on AI coding tools to move fast. The problem is that speed comes with blind spots. AI-generated code often ships with subtle but serious issues unsafe SQL queries, overly broad cloud permissions, exposed APIs, insecure LLM prompts, and fragile data flows. Most existing security tools were not designed to catch these problems. They look at one layer at a time, generate huge volumes of alerts, and leave engineers to figure out what actually matters.

Capslogue takes a different approach. It looks at the system end-to-end: source code, CI/CD pipelines, cloud infrastructure, runtime behavior, and data paths. It combines static analysis with runtime protection and uses context from across the stack to understand which issues are truly reachable, exploitable, and impactful in production. Instead of thousands of warnings, Prism focuses on the small set of attack paths that can actually be abused and helps teams fix them without slowing down delivery.

Capslogue is designed to fit into real engineering workflows, not fight them.


Capslogue is an AI-native security platform that maps the full attacker path — from source code through CI/CD, cloud infrastructure, and runtime — to answer one question:

> _"Can an attacker actually get from the internet to my crown jewels, and how?"_

Not a scanner. Not a dashboard for alerts. A unified reasoning engine across 10 architectural layers that proves exploitability, quantifies attack scope, and fixes what matters.

---

## Architecture

**10-Layer System** — Data Platform → Ingestion → Normalization & Enrichment → Detection Engines → Security Graph → Risk & Prioritization → AI Reasoning → Orchestration → API Gateway → Presentation

---

## Detection Engines

19 engines + 5 cross-engine subsystems. Each is self-contained with its own rule set, test suite, and plugin interface.

---

## The Security Graph

The core differentiator. A unified knowledge graph that correlates entities across 9 domains to discover attack paths no single scanner can see.

---

## AI Reasoning Layer

10 specialized agents orchestrated via LangGraph state machine — not a single LLM wrapper.

---

## Compliance

Continuous control mapping across: **SOC 2 Type II** · **PCI-DSS v4.0** · **HIPAA** · **GDPR** · **DORA** · **EU AI Act** · **CIS Benchmarks** · **NIST 800-53** · **MITRE ATT&CK**

Auto-generated evidence per control. Real-time compliance scoring. Gap analysis. Board-ready PDF reports.

---

<div align="center">

**Private repository — not accepting contributions at this time.**

</div>
