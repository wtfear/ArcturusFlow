<p align="center">
  <img src="assets/arcturus-logo.svg" alt="ArcturusFlow Logo" width="760" />
</p>

<p align="center">
  <strong>Enterprise Autonomous AI Content &amp; Workflow Automation Engine</strong><br>
  <em>400+ Enterprise Connectors, Autonomous Multi-Channel Auto-Posting, and Zero Per-Task SaaS Taxes</em>
</p>

<p align="center">
  <a href="https://github.com/wtfear/ArcturusFlow/actions/workflows/ci.yml"><img src="https://github.com/wtfear/ArcturusFlow/actions/workflows/ci.yml/badge.svg" alt="CI Status" /></a>
  <img src="https://img.shields.io/badge/License-MIT-amber.svg" alt="License: MIT" />
  <img src="https://img.shields.io/badge/Connectors-400+_Pieces-orange.svg" alt="400+ Pieces" />
  <img src="https://img.shields.io/badge/Stack-TypeScript_+_Node.js-blue.svg" alt="TypeScript + Node.js" />
  <img src="https://img.shields.io/badge/Database-PostgreSQL_+_Redis-emerald.svg" alt="PostgreSQL + Redis" />
  <img src="https://img.shields.io/badge/Constellation-Bo%C3%B6tes_%CE%B1-red.svg" alt="Boötes Alpha Star" />
</p>

---

## 🌟 Executive Overview

**ArcturusFlow** is an institutional-grade, self-hosted workflow automation and autonomous AI content engine designed for digital agencies, modern enterprises, and high-volume operations. Named after **Arcturus**, the blazing golden-red alpha star of the Boötes constellation (the 4th brightest star in the night sky), ArcturusFlow replaces exorbitant per-task SaaS platforms (Zapier, Make.com) with a completely sovereign, unlimited automation environment.

Featuring over **400+ pre-built integrations ("pieces")**, native **MCP (Model Context Protocol)** servers, and deep support for multi-model AI agents (OpenAI, Anthropic, Gemini, Ollama), ArcturusFlow powers autonomous content pipelines, cross-platform social publishing, lead routing, and ERP/CRM data synchronization under a 100% permissive open-source license.

---

## 🏛️ Agency & Enterprise Capabilities

### 1. 📢 Autonomous Social Content & Auto-Posting Pipelines
- Automatic RSS, blog, and YouTube monitoring: instantly converts published content into platform-optimized LinkedIn carousels, X (Twitter) threads, and Instagram/Facebook captions.
- Automated media formatting, hashtag group injection, and visual scheduling queues.
- Synchronizes with **CastorChat** (for inbound comment/DM triage) and **PolarisERP** (for social lead attribution).

### 2. ⚡ 400+ Enterprise Connectors & Custom Pieces
- Turnkey connections to Google Workspace, Microsoft 365, Slack, Discord, HubSpot, Salesforce, Stripe, Shopify, GitHub, and Jira.
- Native **MCP (Model Context Protocol)** integration: exposes all 400+ connectors directly as tools to Claude, ChatGPT, and autonomous coding agents.
- Custom piece CLI (`npm run create-piece`) for building proprietary, client-specific API connectors in minutes.

### 3. 🤖 Visual Multi-Agent Flow Canvas
- Intuitive drag-and-drop visual interface for orchestrating multi-step conditional workflows, loops, and parallel executions.
- Embedded LLM nodes for intelligent summarization, sentiment extraction, document parsing, and dynamic decision-making.
- Human-in-the-loop review gates: require client approval via Slack, email, or webhook before publishing high-stakes content.

### 4. 🔒 Enterprise Data Sovereignty & Zero Task Penalties
- Runs entirely inside your private VPC (Docker, Render, AWS, GCP, Bare-Metal) with zero third-party telemetry.
- No per-operation or per-task pricing tiers: process 10,000 or 10,000,000 events monthly for the exact same deterministic infrastructure cost.
- Full compliance readiness: keeps sensitive customer PII and enterprise records strictly within your regulatory boundary (GDPR, HIPAA, SOC-2).

---

## 🛠️ Technology Stack

| Layer | Technologies |
| :--- | :--- |
| **Backend & Engine** | Node.js 20+, TypeScript, Fastify, BullMQ, TurboRepo |
| **Frontend UI** | Angular / React, Tailwind CSS, SVG Visual Flow Canvas |
| **Data & Storage** | PostgreSQL 14+ (with `pgvector` semantic tool search), Redis 7 (BullMQ task queue) |
| **Integrations** | 400+ Pieces, Model Context Protocol (MCP) Server, Webhooks, REST API |
| **Orchestration** | Docker, Docker Compose, Render Blueprint (`render.yaml`) |

---

## 🚀 Instant Deployment

### Local / Production Docker Compose

Ensure Docker and Docker Compose are installed:

```bash
git clone https://github.com/wtfear/ArcturusFlow.git
cd ArcturusFlow

# Launch the complete automation engine (App + Worker + Postgres + Redis)
docker compose up -d
```

Open your browser to `http://localhost:8080` to configure your first autonomous flow.

---

### Cloud 1-Click Deployment (Render)

Deploy high-availability ArcturusFlow with managed PostgreSQL and Redis using Render:

1. Fork or push this repository to your GitHub organization.
2. In Render, select **Blueprints** -> **New Blueprint Instance**.
3. Select this repository; Render will parse [`render.yaml`](./render.yaml) and launch:
   - `arcturus-flow-app` (Web UI & API Server)
   - `arcturus-flow-worker` (High-Throughput Execution Worker)
   - `arcturus-flow-db` (Managed PostgreSQL Database)
   - `arcturus-flow-redis` (Managed Redis Task Queue)

---

## 📂 Repository Structure

```
ArcturusFlow/
├── packages/             # Modular TurboRepo packages
│   ├── engine/           # Flow execution runtime & isolated sandbox
│   ├── pieces/           # 400+ pre-built integration pieces (social, CRM, storage)
│   ├── server/           # API backend, auth, webhooks, and worker dispatchers
│   └── ui/               # Visual flow canvas & administrative dashboard
├── assets/               # Brand vectors and ArcturusFlow logos
├── docker-compose.yml    # 1-Click production multi-container orchestration
├── render.yaml           # Turnkey Render Infrastructure-as-Code blueprint
├── package.json          # Root workspace configuration
└── README.md             # Institutional documentation
```

---

## 📜 Licensing

ArcturusFlow Community is open-source software licensed under the permissive **[MIT License](LICENSE)**.

---

<p align="center">
  Built with pride by the <strong>WTFear</strong> Open-Source Enterprise Initiative.
</p>
