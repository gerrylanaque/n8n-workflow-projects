# AI & Enterprise Automation Portfolio

A curated collection of production-ready automation workflows, AI agent pipelines, and business integration specs built primarily using **n8n**, **LLM integrations**, and enterprise software APIs.

---

## 🏗️ Architecture & Operational Philosophy

All automation workflows in this repository are built around core enterprise principles:

* **Strict Determinism & Governance:** AI components are strictly isolated to structured data extraction and draft generation. Critical business operations, downstream database writes, and external communications are always governed by explicit rule-based gatekeeping.
* **Human-in-the-Loop (HITL) Validation:** High-stakes workflows incorporate mandatory approval steps via Slack, email, or webhooks before external payloads are dispatched.
* **"One Node, One Task" Isolation:** Modular node design ensures decoupled execution, simplified logging, precise error handling, and robust fault tolerance.
* **Data Privacy & Compliance (GDPR / Minimal Risk):** Data pipelines are designed with data minimization, local environment isolation, and payload anonymization prior to external API consumption.

---

## 📁 Repository Structure & Projects

Each automation project is organized in its own self-contained folder containing its exported n8n workflow file, documentation/briefs, and canvas visual representations.

```text
.
├── enquiry-ingestion-automation/   # Multi-channel order ingestion pipeline
├── [future-workflow-name]/         # Reserved for next workflow project
└── README.md                       # Main portfolio overview
