# AI-Powered Automated Order Ingestion Pipeline

An automated ingestion workflow built in n8n. The system processes incoming order payloads, uses Google Gemini to extract structured JSON entities, applies conditional routing, and features human-in-the-loop review before dispatching outputs.

![n8n Workflow Canvas](screenshots/n8n%20enquiry%20ingestion%20automation.png)

## 📌 Project Overview
- **Trigger:** Webhooks / Incoming API Payloads
- **AI Engine:** Google Gemini Structured Output Parser
- **Core Automation:** n8n
- **Error Handling:** Conditional branching & human approval via Slack

## 🏗️ Key Architecture & Features
- **"One Node, One Task" Isolation:** Decoupled execution steps for scalable logging and deterministic error handling.
- **Structured Output Parsing:** Enforces strict JSON schema validation to guarantee reliable database writes.
- **Human-in-the-Loop Validation:** Route notifications to Slack requiring manual approval prior to dispatching external communications.

## 📁 Repository Structure
- [`workflows/n8n-workflow.json`](workflows/n8n-workflow.json) : Exported n8n workflow file (sanitized).
- - [`docs/Automation_Agent_Brief_EN.pdf`](docs/Automation_Agent_Brief_EN.pdf) : Full AI Brief Proposal & System Spec (English).
- [`docs/Automation_Agent_Brief_DE.pdf`](docs/Automation_Agent_Brief_DE.pdf) : AI-Briefing-Vorschlag & Systemspezifikation (Deutsch).

## 🚀 How to Import into n8n
1. Download `workflows/n8n-workflow.json`.
2. Open your n8n instance and navigate to **Workflows**.
3. Click **Import from File** and select `n8n-workflow.json`.
4. Re-bind your local API credentials and environment variables.
