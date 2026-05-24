<!-- ANIMATED WAVE HEADER -->
<div align="center">

[![SentinelGraph](https://capsule-render.vercel.app/api?type=waving&color=0:0F2D5C,50:1B4F8C,100:4A90D9&height=280&section=header&text=SentinelGraph&fontSize=88&fontColor=ffffff&animation=fadeIn&fontAlignY=42&desc=Proactive%20Fraud%20Syndicate%20Detection%20for%20PSU%20Bank%20Underwriters&descAlignY=64&descSize=19&descColor=C8E6FF)](https://github.com/threatpilots/sentinelgraph)

<!-- TYPING ANIMATION -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=1B4F8C&center=true&vCenter=true&random=false&width=650&lines=🔍+Detects+fraud+rings%2C+not+just+documents;🧠+Fraud+Knowledge+Graph+that+learns+over+time;🔒+Local+AI+—+data+never+leaves+the+bank;⚡+Verdict+in+under+2+minutes;🏆+SuRaksha+Cyber+Hackathon+2.0+·+Canara+Bank)](https://git.io/typing-svg)

<br/>

<!-- SHIELD BADGES -->
![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-5.x-008CC1?style=for-the-badge&logo=neo4j&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-Llama_3.1_8B-FF6B35?style=for-the-badge&logo=meta&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)

<br/>

![Hackathon](https://img.shields.io/badge/🏆_SuRaksha_Cyber_Hackathon_2.0-Canara_Bank-1B4F8C?style=for-the-badge)
![Theme](https://img.shields.io/badge/Theme_1-Real--Time_Anomaly_Detection-5B21B6?style=for-the-badge)
![Team](https://img.shields.io/badge/Team-ThreatPilots-FF6B35?style=for-the-badge)

</div>

---

<div align="center">

### *"Every other system detects fraud after reviewing the file."*
### *"Ours recognises the fraud ring before the underwriter opens page one."*

</div>

---

<!-- STAT CARDS -->
<div align="center">
<table>
<tr>
<td align="center" width="175">
<h2>⏱️</h2>
<h2><b>2 min</b></h2>
<sub>Verdict Time<br/>vs 45 min manual</sub>
</td>
<td align="center" width="175">
<h2>📉</h2>
<h2><b>90%</b></h2>
<sub>Token Reduction<br/>vs full-file LLM</sub>
</td>
<td align="center" width="175">
<h2>🕸️</h2>
<h2><b>6-Node</b></h2>
<sub>Syndicate Graph<br/>not single doc check</sub>
</td>
<td align="center" width="175">
<h2>⚖️</h2>
<h2><b>BSA 2023</b></h2>
<sub>Court-Ready Output<br/>human signs off</sub>
</td>
<td align="center" width="175">
<h2>🔒</h2>
<h2><b>Zero</b></h2>
<sub>Cloud Exposure<br/>data never leaves bank</sub>
</td>
</tr>
</table>
</div>

---

## 📖 Table of Contents

<div align="center">

[🚨 The Problem](#-the-problem) · [💡 The Solution](#-the-solution) · [✨ Features](#-features) · [🏗️ Architecture](#️-architecture) · [🔐 Authentication](#-authentication) · [🤖 Local AI Engine](#-local-ai-engine) · [🛡️ Privacy & Security](#️-privacy--security) · [🚀 Quick Start](#-quick-start) · [🧱 Tech Stack](#-tech-stack) · [📁 Project Structure](#-project-structure) · [👥 Team](#-team)

</div>

---

## 🚨 The Problem

> Indian PSU banks lose **₹30,252 crore** to fraud annually. **98% of that, by value, is credit fraud.** Land-backed loan fraud is almost never caught at underwriting. It surfaces 2–5 years later when the bank tries to recover the property — and finds it doesn't exist.

Meet **Priya** — a loan underwriter at a PSU bank RACPC.

```
📋 15–30 loan files per day
⏱️ 20–45 minutes to review each file
🌐 Manually checks 4–5 government portals per file
👥 Trusts external lawyer & valuer to verify title & value
⚠️  Fear: approve a fraud → CBI inquiry, career over
⚠️  Fear: wrongly reject → branch manager pressure, missed targets
```

The result? **Priya approves files she's unsure about** — because rejecting without solid evidence is professionally dangerous. She goes home every evening not knowing if she just approved a ₹50 lakh fraud.

**The critical insight from our research:** Fraud is never committed by one person. It's always a **coordinated 6-person syndicate.**

<div align="center">

```
Promoter/Broker ──── recruits all members, stays invisible
     │
     ├──► Straw Buyer ────── clean CIBIL, provides identity
     │
     ├──► Panel Advocate ─── certifies forged title deed
     │
     ├──► Empanelled Valuer ─ inflates property value 30–40%
     │
     ├──► Bank Insider ────── bypasses EWS flags
     │
     └──► Shell Company ───── pays EMIs for 12–24 months to delay suspicion
```

</div>

No single document check catches a fraud where every document has been carefully prepared by a **professional 6-person operation.**

---

## 💡 The Solution

**SentinelGraph** maps every entity in a loan file — borrower, advocate, valuer, property, phone numbers, document fingerprints — as **nodes in a persistent Fraud Knowledge Graph.**

When a new file arrives, we check if those nodes already exist in confirmed fraud clusters. **The fraud ring is flagged before the underwriter opens page one.**

<div align="center">

```
REACTIVE  (everyone else):  File arrives → scan → detect → alert
PROACTIVE (SentinelGraph):  File arrives → graph match → "already know this ring" → flag
```

</div>

---

## ✨ Features

<div align="center">
<table>
<tr>
<td width="50%" valign="top">

### 🕸️ Fraud Knowledge Graph
Every confirmed fraud case adds nodes and edges. The system gets smarter with every file it processes. Syndicates that reuse the same broker, advocate, or phone number get caught immediately on their next attempt — regardless of which documents they forge.

</td>
<td width="50%" valign="top">

### 📄 Document Forensics Engine
PDF metadata timestamp analysis, font size anomaly detection invisible to the human eye, cross-document value contradiction engine (sale deed vs stamp duty vs market rate vs loan amount), and a growing Forgery Pattern Library of known fraud artifacts.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏛️ Real-Time Government API Verification
Live queries to DILRMP (land records), CERSAI (mortgage registry), ULI framework (income, identity, GST), and eCourts (litigation). Bypasses the forged document entirely — goes straight to the government source.

</td>
<td width="50%" valign="top">

### 🤖 Local AI — Privacy by Architecture
Ollama + Llama 3.1 8B runs entirely on bank hardware. Sensitive data never reaches any cloud service. GGUF quantization delivers results in under 5 seconds. The LLM receives only 300–400 token compressed graph context — not 30,000+ raw document tokens.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 Behavioral Authentication
Continuous keystroke and mouse dynamics monitoring catches insider threats mid-session. WebAuthn passwordless login eliminates credential theft. JWT revoked automatically on behavioral anomaly.

</td>
<td width="50%" valign="top">

### ⚖️ Legally Defensible Output
Plain-language Risk Card with specific, citable evidence — not a probability score. Human signs off on every decision. SHA-256 immutable audit trail. Compliant with Bharatiya Sakshya Adhiniyam 2023, RBI FMR mandates, and DPDP Act 2023.

</td>
</tr>
</table>
</div>

---

## 🏗️ Architecture

<div align="center">
<img width="1484" height="1060" alt="image" src="https://github.com/user-attachments/assets/7c38eb01-7c78-4978-9d20-938a87f85fdd" />

</div>

---

## 🔐 Authentication

SentinelGraph's authentication layer directly solves the **insider threat** — the bank employee who bypasses fraud checks.

<div align="center">
<table>
<tr>
<th width="33%">🔑 Passwordless Login</th>
<th width="33%">🧠 Behavioral Auth</th>
<th width="33%">🚨 Session Monitor</th>
</tr>
<tr>
<td valign="top">

- **WebAuthn** — biometric or hardware key
- **Aadhaar OTP** integration
- Phishing-resistant by design
- No password to steal or forget
- Aligns with RBI strong auth mandate

</td>
<td valign="top">

- **Keystroke dynamics** — typing rhythm
- **Mouse movement** pattern analysis
- Score recalculated every 60 seconds
- Invisible to user, zero friction
- Catches imposters mid-session

</td>
<td valign="top">

- Behavioral anomaly → JWT revoked
- Supervisor alert triggered
- Event logged to audit trail
- Session locked pending re-auth
- **Catches the insider threat**

</td>
</tr>
</table>
</div>

---

## 🤖 Local AI Engine

> *"Local LLM equals slow"* — this is outdated thinking. Here's why we're faster and more private:

<div align="center">
<table>
<tr>
<th>Dimension</th>
<th>☁️ Cloud API</th>
<th>🏦 SentinelGraph Local</th>
</tr>
<tr>
<td><b>Data leaving bank</b></td>
<td>❌ Sent to cloud vendor</td>
<td>✅ Stays on bank hardware</td>
</tr>
<tr>
<td><b>RBI Data Localization</b></td>
<td>❌ At risk</td>
<td>✅ Fully compliant</td>
</tr>
<tr>
<td><b>Token cost at scale</b></td>
<td>❌ ₹X per token × 10K files/day</td>
<td>✅ Fixed hardware cost, zero per-token</td>
</tr>
<tr>
<td><b>Input size</b></td>
<td>30,000+ tokens (full file)</td>
<td>300–400 tokens (graph nodes only)</td>
</tr>
<tr>
<td><b>Response time</b></td>
<td>Cloud RTT + inference</td>
<td>< 5 seconds (GGUF quantized)</td>
</tr>
<tr>
<td><b>DPDP Act 2023</b></td>
<td>❌ Complex data agreements</td>
<td>✅ Compliant by architecture</td>
</tr>
<tr>
<td><b>Activation</b></td>
<td>Always running</td>
<td>Only on HIGH-risk detection</td>
</tr>
</table>
</div>

**The graph does the heavy lifting. The LLM just explains what the graph already found.**

---

## 🛡️ Privacy & Security

```
┌─────────────────────────────────────────────────────────────┐
│                  FIVE-LAYER SECURITY SHIELD                  │
├──────────────────────────────────────────────────────────────┤
│  Layer 1  │  PII Hashing         │  SHA-256 before storage  │
│           │                      │  Raw Aadhaar/PAN never   │
│           │                      │  stored in any database  │
├──────────────────────────────────────────────────────────────┤
│  Layer 2  │  Consent-Based       │  ULI Framework — data    │
│           │  Access              │  queried, not retained   │
├──────────────────────────────────────────────────────────────┤
│  Layer 3  │  Data Minimization   │  Only anomalous nodes    │
│           │                      │  reach the LLM engine    │
├──────────────────────────────────────────────────────────────┤
│  Layer 4  │  RBAC + Encryption   │  Role-limited access,    │
│           │                      │  AES-256 at rest,        │
│           │                      │  TLS 1.3 in transit      │
├──────────────────────────────────────────────────────────────┤
│  Layer 5  │  Immutable Audit     │  SHA-256 hash chain,     │
│           │  Trail               │  RBI FMR compliant,      │
│           │                      │  DPDP Act 2023 aligned   │
└──────────────────────────────────────────────────────────────┘
```

---

## 🚀 Quick Start

### Prerequisites

```bash
# Python 3.11+
python --version

# Node.js 18+ (for frontend)
node --version

# Docker (for Neo4j)
docker --version

# Ollama
curl -fsSL https://ollama.com/install.sh | sh
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/threatpilots/sentinelgraph.git
cd sentinelgraph

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Start Neo4j Knowledge Graph
docker run -d \
  --name sentinelgraph-neo4j \
  -p 7474:7474 -p 7687:7687 \
  -e NEO4J_AUTH=neo4j/sentinelgraph \
  neo4j:5

# 5. Pull the local LLM
ollama pull llama3.1:8b

# 6. Configure environment
cp .env.example .env
# Edit .env with your DILRMP, CERSAI, ULI API credentials

# 7. Seed the Knowledge Graph with fraud patterns
python scripts/seed_fraud_graph.py

# 8. Start the API
uvicorn app.main:app --reload --port 8000

# 9. Start the frontend (new terminal)
cd frontend && npm install && npm run dev
```

### First Run

```bash
# Upload a sample loan file for analysis
curl -X POST http://localhost:8000/api/analyze \
  -H "Authorization: Bearer <your-jwt-token>" \
  -F "file=@sample_loan_file.pdf"

# Response:
{
  "risk_level": "HIGH",
  "confidence": 0.92,
  "fraud_pattern_match": "Pattern #17",
  "issues": [
    {
      "type": "LAND_RECORD_MISMATCH",
      "severity": "CRITICAL",
      "detail": "Submitted 2400 sqft. DILRMP shows 1200 sqft.",
      "source": "DILRMP API"
    },
    {
      "type": "ADVOCATE_NPA_HISTORY",
      "severity": "HIGH",
      "detail": "Advocate has 6/8 recent approvals turned NPA.",
      "source": "Knowledge Graph"
    },
    {
      "type": "PDF_MODIFICATION",
      "severity": "HIGH",
      "detail": "Statement modified 1 day before application.",
      "source": "PDF Forensics"
    }
  ],
  "risk_card": "...",
  "audit_trail_id": "sha256:a3f..."
}
```

---

## 🧱 Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **Document Forensics** | ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-2.x-orange?style=flat-square) ![Tesseract](https://img.shields.io/badge/Tesseract-5.x-blue?style=flat-square) | PDF metadata analysis, OCR, font forensics |
| **Knowledge Graph** | ![Neo4j](https://img.shields.io/badge/Neo4j-5.x-008CC1?style=flat-square&logo=neo4j) | Fraud syndicate node-relationship storage |
| **Government APIs** | ![ULI](https://img.shields.io/badge/ULI-RBI-1B4F8C?style=flat-square) ![CERSAI](https://img.shields.io/badge/CERSAI-Gov-1B4F8C?style=flat-square) | DILRMP, CERSAI, ULI, eCourts, GSTN |
| **Local AI** | ![Ollama](https://img.shields.io/badge/Ollama-Llama_3.1_8B-FF6B35?style=flat-square) | On-premise LLM, GGUF quantized |
| **Authentication** | ![WebAuthn](https://img.shields.io/badge/WebAuthn-Passkeys-5B21B6?style=flat-square) ![TypingDNA](https://img.shields.io/badge/TypingDNA-Behavioral-5B21B6?style=flat-square) | Passwordless + continuous behavioral auth |
| **Backend** | ![FastAPI](https://img.shields.io/badge/FastAPI-0.110-009688?style=flat-square&logo=fastapi) ![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python) | REST API, async processing |
| **Frontend** | ![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react) ![TailwindCSS](https://img.shields.io/badge/Tailwind-3.x-06B6D4?style=flat-square&logo=tailwindcss) | Underwriter dashboard, Risk Card UI |
| **Audit Trail** | ![SHA-256](https://img.shields.io/badge/SHA--256-Hash_Chain-166534?style=flat-square) | Immutable action log, RBI compliance |
| **Privacy** | ![AES-256](https://img.shields.io/badge/AES--256-At_Rest-166534?style=flat-square) ![TLS](https://img.shields.io/badge/TLS_1.3-In_Transit-166534?style=flat-square) | DPDP Act 2023 + RBI compliance |

</div>

---

## 📁 Project Structure

```
sentinelgraph/
│
├── 📂 app/
│   ├── 📂 api/
│   │   ├── analyze.py          # Main loan file analysis endpoint
│   │   ├── auth.py             # WebAuthn + behavioral auth
│   │   └── audit.py            # Audit trail endpoints
│   ├── 📂 core/
│   │   ├── forensics.py        # PDF metadata + font analysis
│   │   ├── graph_engine.py     # Neo4j Knowledge Graph operations
│   │   ├── contradiction.py    # Cross-document contradiction engine
│   │   ├── pattern_library.py  # Forgery Pattern Library
│   │   └── llm_engine.py       # Ollama + Llama 3.1 8B integration
│   ├── 📂 integrations/
│   │   ├── dilrmp.py           # Land record API
│   │   ├── cersai.py           # Mortgage registry API
│   │   ├── uli.py              # Unified Lending Interface
│   │   └── ecourts.py          # Litigation check API
│   └── 📂 security/
│       ├── pii_hasher.py       # SHA-256 PII anonymization
│       ├── audit_chain.py      # Immutable hash chain
│       └── rbac.py             # Role-based access control
│
├── 📂 frontend/
│   ├── 📂 src/
│   │   ├── 📂 components/
│   │   │   ├── RiskCard.jsx    # Main verdict card component
│   │   │   ├── GraphView.jsx   # Fraud network visualization
│   │   │   └── AuditLog.jsx    # Audit trail viewer
│   │   └── 📂 pages/
│   │       └── Dashboard.jsx   # Underwriter dashboard
│
├── 📂 scripts/
│   ├── seed_fraud_graph.py     # Seed Neo4j with fraud patterns
│   └── import_patterns.py     # Import Forgery Pattern Library
│
├── 📂 docs/
│   ├── ARCHITECTURE.md
│   └── API_REFERENCE.md
│
├── docker-compose.yml
├── requirements.txt
└── .env.example
```

---

## 🔍 How The Knowledge Graph Works

<details>
<summary><b>Click to expand — The graph explained simply</b></summary>

<br/>

Every confirmed fraud case leaves behind a "fingerprint" in the graph:

```
[Broker Ram Prasad]
      │
      │ recruited
      │
[Straw Buyer Suresh] ──── used phone ────► [+91-98XXXXXXXX]
      │                                           │
      │ applied at                                │ also used in
      │                                           ▼
[Canara Bank Nashik]               [3 other loan applications]
      │
      │ certified by
      ▼
[Advocate Sharma] ─────── cleared 6 files ──────► [5 became NPAs]
      │
      │ valued by
      ▼
[Valuer Mehta] ──────── consistent 40% overvaluation pattern
      │
      │ property at
      ▼
[Survey No. 142, Nashik] ─── DILRMP shows different owner
```

When a **new file** comes in with Advocate Sharma → **instant flag**, before any documents are reviewed.

Over time, the graph reveals patterns no single-file check would ever find:
- Same broker always uses the same valuer
- Same shell company structure across 12 applications in 3 districts
- Same stamp paper batch number appearing in fraudulent files across 2 states

</details>

---

<details>
<summary><b>Click to expand — Why local LLM is smarter, not slower</b></summary>

<br/>

The graph pre-filters everything before the LLM is called:

```
Without SentinelGraph:
[30,000 token full document] ──► LLM ──► generic output
Cost: HIGH | Speed: SLOW | Privacy: ❌

With SentinelGraph:
[Knowledge Graph matching] ──► 3 anomalous nodes extracted
[300-400 token compressed context] ──► LLM ──► precise risk card
Cost: 90% LOWER | Speed: < 5 seconds | Privacy: ✅
```

GGUF quantization shrinks Llama 3.1 8B by 90%+ with imperceptible quality loss.
On a standard bank server GPU, inference takes **under 5 seconds** for our task.

</details>

---

## 📊 Impact

<div align="center">

| Metric | Before SentinelGraph | With SentinelGraph |
|--------|---------------------|-------------------|
| **Fraud detection timing** | Post-NPA: 23–63 months after disbursal | Pre-disbursal: at the underwriting desk |
| **Underwriter verdict time** | 45 min manual review | Under 2 minutes |
| **Syndicate detection** | Not possible with per-doc checking | Graph maps 6-person rings across applications |
| **LLM cost per file** | 30,000 tokens to cloud API | 300–400 tokens to local model |
| **Legal defensibility** | Gut feeling, hard to document | SHA-256 audit trail, BSA 2023 compliant |
| **Data privacy** | PII processed by cloud vendor | Zero third-party exposure |
| **System improvement** | Static rules, manual updates | Graph compounds — smarter per fraud caught |
| **Underwriter confidence** | Anxious — "am I missing something?" | Protected — evidence-backed, documented |

</div>

---

## 👥 Team

<div align="center">

### 🛩️ ThreatPilots

*SuRaksha Cyber Hackathon 2.0 · Canara Bank · Theme 1: Real-Time Anomaly Detection*

<br/>

We are a team of builders who believe the best fraud detection systems are not built by looking at documents — they are built by looking at **people and their patterns.**

</div>

---

## 🗺️ Roadmap

- [x] Fraud Knowledge Graph core engine
- [x] Document Forensics (PDF metadata, font analysis)
- [x] Cross-document contradiction engine
- [x] Government API integration (DILRMP, CERSAI, ULI)
- [x] Local LLM (Ollama + Llama 3.1 8B) with graph compression
- [x] WebAuthn passwordless authentication
- [x] Behavioral auth (keystroke + mouse dynamics)
- [x] SHA-256 immutable audit trail
- [x] Underwriter Risk Card dashboard
- [ ] Multi-state document format support (all 28 states)
- [ ] Cross-bank syndicate detection (National Hunter integration)
- [ ] Mobile app for field officers
- [ ] Post-disbursal continuous monitoring module
- [ ] RBI regulatory reporting automation (FMR filing)

---

## 📄 License

```
MIT License — Copyright (c) 2025 ThreatPilots

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software to deal in the Software without restriction, including the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell copies of the Software.
```

---

<div align="center">

### Built with 🔥 for SuRaksha Cyber Hackathon 2.0

*Canara Bank · Theme 1: Real-Time Anomaly Detection*

---

**The underwriter currently goes home every evening unsure whether she missed something.**
**SentinelGraph gives her the evidence to be certain — and the documentation to prove it.**

---

[![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:4A90D9,50:1B4F8C,100:0F2D5C&height=120&section=footer)](https://github.com/threatpilots/sentinelgraph)

</div>
