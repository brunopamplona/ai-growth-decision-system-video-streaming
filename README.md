# AI Growth Decision System — Video Streaming platform

A **Staff‑level, multi‑agent AI framework** designed to support **responsible growth decision‑making** for large‑scale video streaming platforms.

This system operationalizes growth strategy into **roadmaps, technical designs, experiment backlogs, and QA/UAT plans**, ensuring that every growth initiative is:
- Evidence‑based
- Technically viable
- Privacy‑safe
- Ethically responsible
- Aligned to measurable business impact

> This repository focuses on **decision systems**, not feature automation.

---

## 🎯 Mission

Generate and continuously maintain:
- Quarterly Growth Roadmaps  
- Prioritized Growth Backlogs (Epics & User Stories)  
- Technical Design Documents (Tech Design Docs)  
- QA / UAT Validation Packages  

All outputs are directly aligned to core **growth KPIs**:
- Acquisition  
- Activation  
- Retention  
- Recurring Revenue  

Decisions are grounded in **observable signals from the platform value funnel**, including:
- Backend APIs (Video Streaming Service Platform)
- Data extractors, batches, and ingestion pipelines
- Aggregated UX and product interaction signals  

---

## 🧠 System Architecture (Agentic)

The system is implemented as a **governed multi‑agent architecture**, with strict separation of concerns and orchestrated accountability.

### Agents

**Agent 0 — Orchestrator / Growth Manager**
- Entry point for business objectives
- Context consolidation and agent orchestration
- Enforcement of quality gates
- Final coherence validation across strategy, data, and technology

**Agent 1 — Technical & Functional Architect**
- Video Streaming Platform backend APIs and system constraints
- Technical feasibility analysis
- NFRs, scalability, and platform impact assessment

**Agent 2 — Data Specialist**
- Data extractors, batch pipelines, and ingestion logic
- KPI definitions and evidential validation
- Privacy‑safe aggregation and metric provenance

**Agent 3 — Growth & Marketing Decision Scientist**
- Growth hypotheses and prioritization (e.g., RICE)
- Experiment design and evaluation logic
- Ethical growth assessment and trade‑off analysis

---

## ✅ Mandatory Quality Gates

No output can be generated unless **all gates are satisfied**:

1. **Data Evidence Gate**  
   All decisions must reference observable, aggregated signals from the platform funnel.

2. **Privacy & Security Gate**  
   - No PII or sensitive data in outputs  
   - Metrics only in aggregated or inferred form  
   - Privacy‑by‑design enforcement

3. **Technical Coherence Gate**  
   Validation of systemic impact across APIs, data pipelines, and downstream consumers.

4. **Responsible Growth & Ethics Gate**  
   Explicit rejection of:
   - Dark patterns  
   - Addiction‑driven mechanics  
   - Manipulative UX strategies  

5. **Quality Gate (Definition of Ready)**  
   Outputs must be implementation‑ready, reviewable, and auditable.

---

## 📦 Standardized Output Contracts

To minimize ambiguity, hallucination, and rework, all deliverables follow **fixed, versionable formats**:

- **Quarterly Roadmap**
  - Executive 1‑pager
  - Prioritized growth backlog

- **Tech Design Document**
  - Functional and technical architecture
  - Risks, assumptions, and NFRs
  - Observability and monitoring implications

- **Jira Package**
  - Epics → User Stories → Acceptance Criteria
  - Technical tasks and dependencies

- **QA / UAT Plan**
  - Test scope and critical scenarios
  - Test data requirements
  - Expected evidence and success criteria

---

## 🛡️ Responsible AI & Governance Principles

This system is designed under **enterprise‑grade AI governance standards**:

- **Least Privilege**  
  Each agent accesses only the minimum required data and context.

- **Full Auditability**  
  All data access, decisions, and generated outputs are traceable.

- **Human‑in‑the‑Loop**  
  Mandatory human approval for any official artifact:
  - Roadmaps
  - Backlogs
  - Jira artifacts
  - Design documents

- **Anti‑Dark‑Pattern Policy**  
  Growth is constrained by long‑term user trust and platform sustainability.

---

## 🗂️ Repository Structure

```text
avs-growth-team/
├── CLAUDE.md                  # Shared global context and principles
└── .claude/
    ├── agents/
    │   ├── agent0-orchestrator.md
    │   ├── agent1-tech-architect.md
    │   ├── agent2-data-specialist.md
    │   └── agent3-growth-scientist.md
    └── commands/
        ├── quarterly-roadmap.md
        ├── tech-design-doc.md
        ├── jira-package.md
        └── qa-uat-plan.md
