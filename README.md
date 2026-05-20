# 🔐 GRC Portfolio — SecureFinX Pvt. Ltd.

![GRC](https://img.shields.io/badge/Framework-ISO%2027001%3A2022-blue)
![Status](https://img.shields.io/badge/Status-Completed-green)
![Role](https://img.shields.io/badge/Role-GRC%20Consultant-orange)
![LinkedIn](https://img.shields.io/badge/LinkedIn-tusya-blue?logo=linkedin)
![College](https://img.shields.io/badge/VIT%20Chennai-Cybersecurity%20'29-red)

> A complete, end-to-end ISO 27001 GRC engagement conducted for a simulated 60-person fintech startup — built entirely from scratch as a self-directed learning project during a 2-month vacation by a first-year cybersecurity student.

---

## 👤 About This Project

| Field | Details |
|-------|---------|
| **Consultant** | Tusya Subramaniyan |
| **LinkedIn** | [linkedin.com/in/tusya](https://linkedin.com/in/tusya) |
| **College** | VIT Chennai — B.Tech Cybersecurity (2025–2029) |
| **Client** | SecureFinX Pvt. Ltd. *(simulated)* |
| **Duration** | 3 weeks |
| **Frameworks** | ISO 27001:2022, NIST CSF, DPDP Act 2023, RBI Guidelines, PCI-DSS |

---

## 🏢 Client Overview

**SecureFinX Pvt. Ltd.** is a simulated 60-person fintech startup based in Chennai, India.

- Mobile payment application with **200,000 active users**
- Stores **Aadhaar-linked KYC data** and payment transaction history
- Cloud-hosted on **AWS Mumbai region**
- Preparing for **ISO 27001 certification** ahead of Series A funding

They engaged me as their GRC Consultant to assess their security posture, identify risks, build their ISMS from scratch, write core security policies, and conduct a formal internal audit.

---

## 📁 Repository Structure

```
GRC-Portfolio-SecureFinX/
│
├── 📄 README.md
│
├── 📂 01-Company-Profile/
│   └── SecureFinX_Company_Profile.md
│
├── 📂 02-Risk-Register/
│   └── SecureFinX_Risk_Register.xlsx
│
├── 📂 03-Gap-Analysis/
│   └── SecureFinX_Gap_Analysis.xlsx
│
├── 📂 04-Statement-of-Applicability/
│   └── SecureFinX_SoA.xlsx
│
├── 📂 05-Security-Policies/
│   ├── 01_Acceptable_Use_Policy.docx
│   ├── 02_Access_Control_Policy.docx
│   ├── 03_Incident_Response_Policy.docx
│   ├── 04_Data_Classification_Policy.docx
│   └── 05_BYOD_Policy.docx
│
└── 📂 06-Audit-Report/
    └── SecureFinX_Internal_Audit_Report.docx
```

---

## 📊 Project Deliverables

### 1️⃣ Risk Register
- **20 identified risks** across technical, human, process & physical domains
- CVSS-aligned **Likelihood × Impact** scoring methodology
- Risk levels: **4 Critical · 8 High · 6 Medium · 2 Low**
- Risk treatment decision for every risk (**Treat / Tolerate / Transfer / Terminate**)
- Risk heat map for visual prioritisation
- Pre-populated with realistic fintech risks including:
  - S3 bucket misconfiguration exposing Aadhaar data
  - SQL injection on payment API
  - Insider threat via privileged admin accounts
  - Third-party payment gateway breach
  - AWS credentials accidentally committed to GitHub

### 2️⃣ ISO 27001:2022 Gap Analysis
- All **93 Annex A controls** assessed across 4 themes
- Status tracked per control: **Implemented / Partial / Not Implemented / N/A**
- Realistic findings and recommended actions for each gap
- Controls mapped across themes:
  - 🔵 Organisational (37 controls)
  - 🟢 People (8 controls)
  - 🟡 Physical (14 controls)
  - 🔴 Technological (34 controls)

### 3️⃣ Statement of Applicability (SoA)
- Documents which controls **apply, are excluded, and why**
- Justification for inclusion/exclusion of each selected control
- Implementation notes per control
- Required document for ISO 27001 certification — shows auditor-level thinking

### 4️⃣ Security Policies (5 documents)

| # | Policy | Document ID | ISO 27001 Reference |
|---|--------|-------------|---------------------|
| 1 | Acceptable Use Policy | SEC-POL-001 | A.5.10, A.6.2, A.8.1, A.8.19 |
| 2 | Access Control Policy | SEC-POL-002 | A.5.15, A.5.16, A.5.17, A.5.18, A.8.2, A.8.3, A.8.5 |
| 3 | Incident Response Policy | SEC-POL-003 | A.5.5, A.5.26, A.5.27, A.6.8, A.8.15, A.8.16 |
| 4 | Data Classification Policy | SEC-POL-004 | A.5.12, A.5.13, A.5.14, A.8.10, A.8.11 |
| 5 | BYOD Policy | SEC-POL-005 | A.5.10, A.6.7, A.7.9, A.8.1, A.8.5 |

Each policy includes: document ID, version number, ISO 27001 clause references, review date, approval authority, and full substantive content — not template filler.

### 5️⃣ Internal Audit Report
- Formal audit conducted against **ISO 27001:2022 Clauses 4–10**
- Structured audit methodology: Plan → Prepare → Fieldwork → Findings → Report → Follow-up
- Non-conformities documented with **Major / Minor / Observation** severity ratings
- Corrective action recommendations for each finding
- Executive summary written for management audience
- Evidence requirements documented per clause

---

## 🔥 Key Risks Identified

| Risk ID | Asset | Risk | Score | Level |
|---------|-------|------|-------|-------|
| R001 | KYC Data Store | S3 bucket misconfiguration — Aadhaar data exposed | 20 | 🔴 Critical |
| R002 | Payment API | SQL injection attack on payment endpoint | 15 | 🟠 High |
| R003 | Employee Devices | Malware via phishing — no MDM | 16 | 🟠 High |
| R006 | Admin Accounts | Insider threat — no PAM, unrestricted access | 10 | 🟡 Medium |
| R010 | CI/CD Pipeline | Vulnerable library via unscanned dependencies | 12 | 🟡 Medium |
| R015 | KMS Keys | Encryption keys never rotated since launch | 10 | 🟡 Medium |

---

## 🧠 Key Learnings

```
1. ISO 27001 doesn't tell you HOW to secure your org — it tells you WHAT to prove
2. The gap between policy and practice is where every non-conformity lives
3. Risk treatment is a business decision, not just a technical one
4. Writing 5 policies from scratch teaches more than reading 50 articles
5. Governance failures cause more breaches than technical failures
6. Compliance ≠ Security — you can pass every audit and still get breached
7. The creator of data is responsible for classifying it — not IT
8. Security awareness training reduces phishing click rate from 32% to under 5%
9. Your security posture = your weakest vendor's security posture
10. Learning in public forces genuine understanding — you can't fake clarity
```

---

## 🛠️ Tools & Resources Used

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Risk Register, Gap Analysis, SoA |
| Microsoft Word | Security Policies, Audit Report |
| ISO 27001:2022 Standard | Primary framework reference |
| NIST NVD | CVSS scoring reference |
| CERT-In Guidelines | Indian regulatory context |
| RBI Cybersecurity Framework | Fintech compliance reference |
| GitHub | Portfolio publishing |

---

## 📜 Certifications

| Certification | Issuer | Date | Credential ID |
|--------------|--------|------|---------------|
| Cybersecurity Consulting Job Simulation | PwC US via Forage | May 2026 | NDWPa7wHsdQEesBo9 |
| Cybersecurity Job Simulation | Mastercard via Forage | May 2026 | YZR4BBwznKyKPLrRY |
| Cyber Job Simulation | Deloitte via Forage | Jan 2026 | akPcjxEAP3pQBRoQt |

---

## 🏆 Achievements

- 🥉 **3rd Place** — CyberConverge CTF, Tamil Nadu CyberWing (2025)
- 📝 **60 Days of GRC** — Daily LinkedIn learning challenge documenting this entire journey
- 🎓 **8.8 CGPA** — VIT Chennai, B.Tech Cybersecurity (Semester 1 & 2)

---

## 🔗 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tusya%20Subramaniyan-blue?logo=linkedin)](https://linkedin.com/in/tusya)

**Part of:** [60 Days of GRC — LinkedIn Learning Challenge](https://linkedin.com/in/tusya)

> *"I started this with zero GRC knowledge and a 2-month vacation.*
> *Three weeks later I had built a complete ISO 27001 ISMS from scratch.*
> *This is what learning in public looks like."*
> — Tusya Subramaniyan

---

## ⚠️ Disclaimer

*This is a simulated GRC engagement created for educational and portfolio purposes. SecureFinX Pvt. Ltd. is a fictional company. All risks, findings, policies, and recommendations are hypothetical and designed to demonstrate GRC analyst competency. No real organisation's data is involved.*

---

<p align="center">
  <strong>⭐ If this project helped you, consider starring the repo!</strong><br>
  <em>It helps other cybersecurity students find it.</em>
</p>
