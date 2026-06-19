Here is the finalized README with your live GitHub Pages demo link seamlessly integrated.

---

# 🌌 NEXUS | Cloud Intelligence Platform

**NEXUS** is a next-generation Cloud FinOps and Site Reliability Engineering (SRE) command center. Built specifically for Google Cloud Platform (GCP) and Kubernetes environments, it fuses real-time infrastructure metrics, cost allocation data, and predictive intelligence into a single, seamless glassmorphism interface.

---

## 💡 Why I Built NEXUS

During my cloud and data engineering learning journey, I noticed that infrastructure monitoring, cost analytics, and observability data were scattered across multiple, disjointed platforms. Engineers are often forced to context-switch between cloud billing consoles, Grafana dashboards, and raw Prometheus metrics.

NEXUS was built to solve this by unifying these systems into a single data platform that improves visibility, reduces operational overhead, and cultivates proactive cloud cost awareness.

---

## 🛑 Problem Statement

Modern cloud teams use multiple disconnected tools for monitoring, cost management, observability, and infrastructure analytics. Switching between Prometheus, Grafana, cloud billing consoles, and alerting systems creates operational overhead and slows decision-making.

NEXUS provides a unified intelligence platform that combines infrastructure monitoring, FinOps analytics, and observability into a single command center.

---

## 💼 Business Impact

Traditional monitoring and cost management require navigating a fragmented ecosystem of tools. NEXUS reduces operational overhead by providing a single observability and FinOps command center, drastically improving visibility into infrastructure performance and cloud expenditure for engineering teams and stakeholders alike.

---

## 🎥 Live Demo & Deployment

**Live Frontend Deployment:** [View on GitHub Pages](https://invalid-52.github.io/cloud-intelligence-platform/)

**Backend API:** Hosted on Render

**Demonstration Video:** *Coming Soon*

*Explore the live deployment to see NEXUS monitor infrastructure metrics, visualize costs, and display real-time observability data via its integrated dashboard.*

---

## 🏗️ System Architecture

```text
       Client (Browser / GitHub Pages)
              │
              ▼
   NEXUS Frontend (Vanilla JS / Three.js / Chart.js)
              │
              ▼
   API Layer (Node.js hosted on Render) ◄───► AI Engine (Python / ML Models)
              │
 ┌────────────┼────────────┐
 │            │            │
 ▼            ▼            ▼
Prometheus OpenCost     Grafana
 │            │            │
 └────────────┼────────────┘
              │
              ▼
       Cloud Resources
      (GCP / Kubernetes)

```

---

## 📸 Screenshots

### Infrastructure Monitoring Dashboard

### Grafana Integration

 *(Note: Replace with your actual Grafana image path if uploaded)*

---

## 🏆 Key Engineering Achievements

* Built a unified observability platform integrating Prometheus, Grafana, and OpenCost into a single pane of glass.
* Implemented a real-time infrastructure monitoring dashboard using highly responsive Chart.js visualizations.
* Designed a cloud-native deployment architecture bridging a static frontend with a live Render Node.js backend.
* Developed a dedicated Python AI Engine (`anomaly_model.py`, `predict.py`) to process telemetry data for predictive insights.
* Created a scalable FinOps visibility layer for cloud cost analysis, tracking metrics like cost per vCPU-hour and idle waste.

---

## 📈 Project Statistics

* **3** Core Infrastructure Integrations (Prometheus, OpenCost, Grafana)
* **1** Unified Observability Dashboard
* **Real-Time** Metrics Collection and API Polling
* **Decoupled** Microservice Architecture (JS Frontend + Node Backend + Python AI Engine)

---

## 🧠 Core Features

* **Command Center Dashboard:** A real-time, unified view of your GCP infrastructure tracking CPU/Storage loads, DB QPS, and rolling SLA uptimes.
* **Live Prometheus Mesh & PromQL Explorer:** Execute live `PromQL` queries (e.g., `rate(node_cpu_seconds_total[5m])`) directly from the UI.
* **FinOps Engine:** Deep Kubernetes and cloud cost allocation. Tracks idle waste, cost per vCPU-hour, and cross-references them against budget ceilings.
* **Grafana Embedding:** Seamlessly embed any Grafana instance using anonymous auth or API keys for real-time visualization directly inside NEXUS.
* **Alert Matrix:** Centralized AlertManager feed tracking response metrics (MTTD, MTTR) across notification channels.

---

## 📐 Design Decisions

### Why Prometheus?

Chosen for robust time-series metric collection and highly flexible PromQL support.

### Why Grafana?

Provides industry-standard, rich dashboarding and visualization capabilities that embed cleanly via iframe.

### Why OpenCost?

Enables Kubernetes-native cost allocation, providing accurate FinOps analysis and cost intelligence.

### Why Render?

Provides lightweight, reliable deployment for the Node.js API layer with minimal operational overhead, perfect for proxying monitoring data.

---

## 🛠️ Tech Stack & Integrations

**Frontend (Client-Side):**

* Vanilla HTML5, CSS3, JavaScript (Hosted via GitHub Pages).
* **Chart.js** for responsive, real-time metric streams.
* **Three.js** powering the animated "Neural Mesh" background environment.

**Backend (API & Proxy Layer):**

* **Node.js / Express** deployed natively on **Render** (Handles cross-origin request proxying and data aggregation).

**Intelligence Layer (AI Engine):**

* **Python 3** utilizing custom models for anomaly detection and metric prediction.

**Monitoring & FinOps Stack:**

* Prometheus, Node Exporter, Grafana, OpenCost (CNCF).

---

## 📂 Repository Structure

```text
├── ai-engine/
│   ├── anomaly_model.py          # Isolation Forest & EWMA models
│   ├── predict.py                # Linear/Seasonal regression forecasting
│   └── requirements.txt
├── backend/
│   ├── src/
│   │   ├── controllers/          # Metrics aggregation logic
│   │   ├── routes/               # API endpoints
│   │   ├── services/             # External API integration
│   │   └── server.js             # Express application entry
│   └── package.json
├── monitoring-stack/
│   └── prometheus/
│       └── prometheus.yml        # Scrape configs and AlertManager rules
├── index.html                    # Main UI entry point
├── local deployment.png          # UI Screenshot
└── README.md

```

---

## 🚧 Challenges Solved

* Handling strict CORS restrictions between a static frontend and distributed monitoring APIs.
* Integrating dispersed Prometheus metrics into a visually cohesive, single-pane-of-glass dashboard.
* Managing dynamic, real-time data refresh pipelines without blocking the main UI thread.
* Embedding Grafana dashboards securely while managing varying authentication states.
* Structuring a multi-language monolithic repo (JS + Python) cleanly.

---

## 📚 Key Learnings

* Prometheus architecture, PromQL syntax, and metric scraping mechanics.
* Grafana dashboard management and secure `iframe` embedding practices.
* Core cloud observability and telemetry pipeline engineering.
* FinOps fundamentals, resource allocation mapping, and cloud billing analysis.
* Bridging distinct microservices (Node.js API communicating with a Python AI Engine).

---

## ⚠️ Current Limitations

* Requires a pre-existing Prometheus configuration to stream live infrastructure data.
* OpenCost functionality explicitly requires a Kubernetes cluster to track namespace-level allocations.
* Multi-cloud support is not yet fully realized (currently optimized for GCP environments).

---

## 🔬 Future Research Directions

* Integrating Claude AI (Anthropic LLM) for natural language incident analysis and automated remediation suggestions.
* Expanding the Python `ai-engine` with reinforcement learning for dynamic, automated cloud cost optimization.
* Enhancing time-series forecasting models for higher-accuracy predictive cost intelligence.
* Multi-cloud observability intelligence scaling (AWS/Azure integration).

---

## 🚀 Quick Start (Local Setup)

Run the entire NEXUS open-source intelligence stack locally.

### 1. Start Prometheus & OpenCost

```bash
docker run -p 9090:9090 prom/prometheus
kubectl apply -f https://raw.githubusercontent.com/opencost/opencost/main/kubernetes/opencost.yaml

```

### 2. Start Grafana

```bash
docker run -p 3000:3000 grafana/grafana

```

*Note: Set `GF_SECURITY_ALLOW_EMBEDDING=true` in Grafana to enable UI embedding.*

### 3. Launch the Backend API & AI Engine

```bash
# In the backend/ directory
npm install
npm start

# In the ai-engine/ directory (optional for predictive features)
pip install -r requirements.txt
python predict.py

```

### 4. Launch the NEXUS UI

Serve `index.html` from the repository root using any local web server:

```bash
python -m http.server 3000
# or
npx serve -p 3000

```

Navigate to `http://localhost:3000`. The frontend auto-detects the local environment and routes API calls to `localhost:5000`, falling back to the Render backend in production.
