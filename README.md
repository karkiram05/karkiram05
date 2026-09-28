<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=120&section=header" width="100%" alt=""/>

<h1 align="center">Hi, I'm Ram Karki 👋</h1>
<p align="center"><b>Cybersecurity</b> · <b>Detection Engineering</b> · <b>OT/ICS Security</b></p>

<p align="center">
  <a href="https://www.linkedin.com/in/ram-karki-434753255/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:karkiram3207@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://gettoknowram.vercel.app"><img src="https://img.shields.io/badge/Website-0F766E?style=for-the-badge&logo=vercel&logoColor=white" alt="Website"></a>
  <img src="https://img.shields.io/badge/Copenhagen,%20Denmark-2E7D32?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location: Copenhagen, Denmark">
</p>

---

### 🧭 About me

I build detection systems and test them the way attackers and real networks would, not the way a benchmark would like.

- 🎓 **MSc Computer Science and Engineering (Cybersecurity)** @ Technical University of Denmark (DTU), 2026 to present
- 🎓 **BEng General Engineering (Cyber Systems)** @ DTU, graduated 2026
- 🏭 Industry experience at **NorthQ** building security automation and anomaly detection for a fleet of 2,000+ IoT devices
- 🛡️ Focus: intrusion detection, blue team monitoring, OT/ICS security, CI/CD and supply-chain security
- 💼 Open to **full-time** roles in Security Engineering, SOC / Detection Engineering and OT Security (my MSc is part-time)

> **How I work:** a model that scores 99% on a random split usually learned the dataset, not the attack. I use temporal and cross-dataset splits, check for leakage, and report what my detectors **miss**, not just what they catch.

---

### 🚀 Featured projects

#### 🔎 [Flow-Based Intrusion Detection with MITRE ATT&CK Mapping](https://github.com/karkiram05/bsc-thesis-ids) &nbsp;·&nbsp; `BEng thesis`
A reproducible ML pipeline for network intrusion detection on **CICIDS2017** (2.31M flows) with cross-dataset validation on **UNSW-NB15**. Compares Logistic Regression, Random Forest, XGBoost and LightGBM under three evaluation protocols, plus adversarial robustness testing and live packet scoring. The key finding: XGBoost macro-F1 drops from **0.863 on a stratified split to 0.440 on a day-based split**, showing how much random splits overstate real performance.
<br>`Python` · `scikit-learn` · `XGBoost` · `LightGBM` · `pandas`

#### 🛰️ [SentinelFlow: Network/IoT Threat Detection Backend](https://github.com/karkiram05/sentinelflow)
A FastAPI backend that ingests connection records, runs them through an explainable rule engine and an **Isolation Forest** model, maps alerts to **MITRE ATT&CK** and scores risk from 0 to 100, with a live dashboard. Reports **96.2% precision and 46.9% recall** on the held-out NSL-KDD test split, with a per-attack breakdown of what it catches and misses.
<br>`Python` · `FastAPI` · `PostgreSQL` · `scikit-learn` · `Docker` · `33 pytest tests` · `CI with Bandit + pip-audit`

#### 🔗 [TrustGraph: CI/CD Attack-Path Analysis](https://github.com/karkiram05/trustgraph)
Static analysis of **GitHub Actions workflows** and **AWS IAM trust policies** that builds a trust graph (repo → workflow → cloud role) to find real exploitation paths, not isolated misconfigurations. Checks OIDC federation, permissions and action pinning, with severity based on reachability. Run against 12 public workflows (Django, Flask, pip and others): 11 clean, 1 with 3 genuine medium findings.
<br>`Python` · `networkx` · `OIDC` · `AWS IAM` · `31 pytest tests`

#### 🌬️ [OffshoreShield: OT/ICS Security Lab](https://github.com/karkiram05/offshore-shield)
An isolated critical-infrastructure lab that replays real **Kelmarsh Wind Farm SCADA** data over Modbus TCP, segmented with Linux network namespaces and nftables. A network tap feeds **7 detection rules mapped to MITRE ATT&CK for ICS**, and an OT-aware prioritiser ranks vulnerabilities by operational risk instead of CVSS alone. Five purple-team scenarios measure real detection latency.
<br>`Python` · `Modbus TCP` · `nftables` · `Linux namespaces` · `ATT&CK for ICS`

---

### 🏭 Industry work

#### 🔒 IoT Anomaly Detection Pipeline &nbsp;·&nbsp; `NorthQ · Security Automation Intern · 2025` &nbsp; ![Private](https://img.shields.io/badge/code-private-555?style=flat-square&logo=lock&logoColor=white)
A production-style Python pipeline processing **31M+ feature rows from 2,244 IoT devices**. Combines **Isolation Forest** with rule-based thresholds, and decodes device status registers into fault indicators such as leak, burst and reverse flow so alerts are actionable for operations.
<br>`Python` · `pandas` · `scikit-learn` · `SQL`
<br><sub>The code belongs to NorthQ and is confidential, so the repository stays private. I am happy to walk through the approach in an interview.</sub>

Before that I worked as an **IoT Deployment Engineer** at NorthQ (2024 to 2025), installing and commissioning gateways and repeaters in the field and diagnosing connectivity and data-integrity issues.

---

### 🧰 More projects

- **🎮 MiniCraft: Java sandbox game** &nbsp;·&nbsp; `DTU · grade 10`<br>
  2D sandbox game in JavaFX with procedural terrain, inventory, combat, mobs and save/load. Built test-first with JUnit and Cucumber BDD (12+ feature specs).
  <br>`Java 21` · `JavaFX` · `Maven` · `Cucumber`
- **⚙️ Guarded Command Language toolchain** &nbsp;·&nbsp; `DTU · grade 10`<br>
  F# implementation of the full pipeline from parser and pretty-printer to program-graph compiler and interpreter, plus program verification, sign analysis, information-flow security analysis and model checking.
  <br>`F#` · `Formal methods` · `Program analysis`
- **🎲 [Kalaha / Mancala game AI](https://github.com/Pratyush2012/Kalaha-Mancala-_game_AI)** (adversarial search) &nbsp;·&nbsp; **🧠 [Belief-revision engine](https://github.com/Pratyush2012/Belief_revision_group45)** (logic-based) &nbsp;·&nbsp; `DTU team projects`
- **🏋️ [Workout tracker](https://github.com/karkiram05/ram-workout-tracker)** &nbsp;·&nbsp; [live demo](https://ram-workout-tracker.vercel.app)<br>
  React 19 + Vite app for logging workouts, nutrition and bodyweight trends. Runs fully in the browser with local storage and CI-tested builds.

---

### 🛠️ Tech stack

**Languages**
<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![F#](https://img.shields.io/badge/F%23-378BBA?style=flat-square&logo=fsharp&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Security**
<br>
![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-B31B1B?style=flat-square)
![OWASP](https://img.shields.io/badge/OWASP%20Top%2010-000000?style=flat-square&logo=owasp&logoColor=white)
![STRIDE](https://img.shields.io/badge/STRIDE%20threat%20modelling-5A5A5A?style=flat-square)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Bandit](https://img.shields.io/badge/Bandit%20%2F%20pip--audit-FFB000?style=flat-square)
![Modbus](https://img.shields.io/badge/Modbus%20TCP-0B3D91?style=flat-square)

**ML & Data**
<br>
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-2C7A3F?style=flat-square)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Backend & DevOps**
<br>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)

---

<p align="center"><sub>Always up for talking detection engineering, OT security or a good football match. ✉️ <a href="mailto:karkiram3207@gmail.com">karkiram3207@gmail.com</a></sub></p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=90&section=footer" width="100%" alt=""/>
