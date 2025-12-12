<p align="center">
  <img src="assets/Codeon logo02.png" alt="Codeon Logo" width="1000" style="border-radius:50px;"/>
</p>

# Codeon

Codeon is a **smart contract auditing and analysis tool** designed to help developers evaluate the **security, performance, and compliance** of their smart contracts before deployment.  

It provides:
- **Multi-language support** (Solidity, Vyper, Rust, Move, Cairo). 
- **Automated vulnerability scanning** and performance checks.
- **Professional PDF audit reports** with charts, severity levels, and recommendations.
- **Simple and intuitive frontend** for uploading contracts and downloading results.  

> ⚡ Codeon’s mission is to make **security and transparency** in smart contract development **accessible, automated, and developer-friendly**.  

---

## ✨ Features

- **Smart Contract Analysis**
  - Reentrancy, overflow/underflow, external call checks, access control, DoS, etc.
  - Gas & performance optimization suggestions.
  - Compliance with ERC-20, ERC-721, ERC-1155 standards.
  - Logic flaws and unreachable code detection.
  - Upgradeability and deployment safety checks.

- **Multi-Language Support**
  - Solidity (Ethereum, EVM-compatible)
  - Vyper (Ethereum)
  - Rust (Solana, Polkadot)
  - Move (Aptos, Sui)
  - Cairo (StarkNet)

- **Audit Report Generation**
  - Export analysis results in **sleek PDF format**.
  - Charts & graphs (vulnerability breakdown, gas usage).
  - Severity levels (Critical, High, Medium, Low, Info).
  - Recommendations.

---

## 🏗️ System Architecture

### 1. Frontend (User Interface)
- Upload contract files (`.sol`, `.vy`, `.rs`, `.move`, etc.).
- Select contract language.
- Trigger audit → display results + PDF download option.
- **Stack:** React + Tailwind CSS.

### 2. Backend (Analysis Engine)
- Handles parsing, analysis, and tests.
- Integrates with static analysis tools (Slither, Move Prover, Clippy, etc.).
- Generates JSON output of findings.
- Converts results to styled PDF.
- **Stack:** Node.js (TypeScript) or Python.

### 3. Report Engine
- Converts backend JSON → PDF with charts & branding.
- **Stack:** ReportLab (Python) or Puppeteer (Node.js).

---

## 🔄 User Flow
1. Developer visits Codeon web app.  
2. Uploads smart contract file.  
3. Selects programming language.  
4. Backend runs analysis.  
5. Results displayed in frontend.  
6. Developer downloads a **PDF Audit Report**.  

---

## 🎯 MVP Deliverables
- Simple web interface (one-page app).  
- Solidity support (first integration).  
- Basic vulnerability + gas checks.  
- PDF report generation.  

_Future scope:_ support more languages, advanced security tests, AI-powered suggestions, etc.

---

## 🛠️ Tech Stack Summary
- **Frontend:** React, Tailwind CSS, Chart.js  
- **Backend:** Node.js (TypeScript) or Python  
- **Static Analysis Tools:** Slither, Move Prover, Clippy, etc.  
- **Database:** PostgreSQL 
- **Report Engine:** ReportLab (Python) / Puppeteer (Node.js)  
- **Deployment:** Docker 

---

### Clone Repository
```bash
git clone https://github.com/DevAsmodeus07/Codeon.git
cd Codeon
