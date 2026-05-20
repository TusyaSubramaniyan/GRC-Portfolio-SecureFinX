# 🔍 Internal Audit Report
## SecureFinX Pvt. Ltd. | ISO 27001:2022

**Document ID:** SEC-AUD-001  
**Version:** 1.0  
**Audit Type:** Internal Information Security Audit  
**Prepared by:** Tusya Subramaniyan (GRC Consultant)  
**LinkedIn:** [linkedin.com/in/tusya](https://linkedin.com/in/tusya)  
**Audit Period:** May 2025  
**Status:** FINAL  

---

## 1. Executive Summary

SecureFinX Pvt. Ltd. engaged an independent GRC consultant to conduct an internal information security audit aligned to ISO 27001:2022. The audit assessed the organisation's current security posture across all mandatory clauses (4–10) and selected Annex A controls.

### Audit Verdict

| Category | Result |
|----------|--------|
| Overall ISMS Maturity | ⚠️ Early Stage |
| Major Non-Conformities | 8 |
| Minor Non-Conformities | 12 |
| Observations | 9 |
| Opportunities for Improvement | 6 |

> **Conclusion:** SecureFinX is not yet ready for ISO 27001 certification. Significant gaps exist across governance, access control, logging, vulnerability management, and policy documentation. A structured 6-month remediation programme is recommended before pursuing Stage 1 certification audit.

---

## 2. Audit Scope

### In Scope
- All information assets owned or managed by SecureFinX
- AWS Mumbai cloud infrastructure
- Mobile payment application (Android & iOS)
- Internal IT systems (HR, Finance, Operations)
- All 60 employees and contractor relationships
- Third-party vendors with access to SecureFinX systems or data

### Out of Scope
- Physical security of customer premises
- Security of customer-owned devices
- AWS infrastructure security (covered under Shared Responsibility Model)

### Audit Criteria
- ISO 27001:2022 Clauses 4–10 (mandatory requirements)
- ISO 27001:2022 Annex A controls (as per Statement of Applicability)
- India's DPDP Act 2023
- RBI Payment Aggregator Cybersecurity Framework

---

## 3. Audit Methodology

The audit was conducted using the following approach:
PLAN → PREPARE → FIELDWORK → FINDINGS → REPORT → FOLLOW-UP
| Phase | Activities |
|-------|-----------|
| **Plan** | Defined scope, criteria, schedule, and audit objectives |
| **Prepare** | Reviewed existing policies, risk register, and gap analysis |
| **Fieldwork** | Interviewed key personnel, reviewed system configurations, tested controls |
| **Findings** | Documented non-conformities with evidence references |
| **Report** | Produced this formal audit report with recommendations |
| **Follow-up** | Corrective action plan to be reviewed in 90 days |

### Non-Conformity Classification

| Severity | Definition |
|----------|-----------|
| **Major** | Complete absence of a required control or systematic failure — prevents certification |
| **Minor** | Partial implementation or isolated failure — must be addressed before certification |
| **Observation** | Not a non-conformity but a risk or improvement opportunity noted |

---

## 4. Findings by ISO 27001 Clause

---

### Clause 4 — Context of the Organisation

#### Finding 4.1 — Major Non-Conformity
**Clause:** 4.1, 4.2  
**Title:** No formal ISMS scope document defined  
**Finding:** SecureFinX has not formally documented the context of the organisation, identified interested parties, or defined the scope of its ISMS. There is no evidence of stakeholder analysis or regulatory mapping.  
**Evidence:** No scope document found. No interested parties register. No regulatory requirements mapping.  
**Risk:** Without a defined scope, all subsequent ISMS activities lack a formal boundary — audit cannot verify what is and is not covered.  
**Recommendation:** Define and document ISMS scope, stakeholder register, and regulatory mapping within 30 days.  
**Target Date:** 30 June 2025  

---

### Clause 5 — Leadership

#### Finding 5.1 — Major Non-Conformity
**Clause:** 5.1, 5.2  
**Title:** No evidence of top management commitment to information security  
**Finding:** No CISO has been appointed. No security policy has been approved by senior management. No evidence of management communication regarding security responsibilities was found.  
**Evidence:** No signed security policy. No CISO appointment letter. No board minutes referencing information security.  
**Risk:** ISO 27001 Clause 5.1 requires demonstrable leadership commitment. Without this, certification is not possible.  
**Recommendation:** Appoint a CISO or equivalent. Have CEO formally approve the information security policy. Include security as a standing board agenda item.  
**Target Date:** 15 June 2025  

#### Finding 5.2 — Minor Non-Conformity
**Clause:** 5.3  
**Title:** Security roles and responsibilities not formally assigned  
**Finding:** While IT staff perform security-related tasks informally, no formal role descriptions, responsibility matrices, or accountability structures have been documented.  
**Evidence:** No RACI matrix. No job descriptions referencing security responsibilities.  
**Recommendation:** Document security roles: CISO, DPO, Risk Owner, System Owner, Incident Response Lead. Update job descriptions.  
**Target Date:** 30 June 2025  

---

### Clause 6 — Planning

#### Finding 6.1 — Major Non-Conformity
**Clause:** 6.1.2  
**Title:** Risk assessment methodology not formally documented  
**Finding:** A risk register has been produced during this engagement. However, SecureFinX did not have a documented risk assessment methodology prior to this audit. No risk treatment plan has been formally approved by management.  
**Evidence:** Risk register produced by consultant — no evidence of prior internal risk assessment. No management sign-off on risk treatment decisions.  
**Risk:** ISO 27001 requires a repeatable, documented risk assessment methodology. A one-time exercise without methodology documentation does not satisfy this requirement.  
**Recommendation:** Formally document the risk assessment methodology. Obtain management approval of the risk register and treatment plan. Schedule annual risk assessment cycle.  
**Target Date:** 30 June 2025  

#### Finding 6.2 — Minor Non-Conformity
**Clause:** 6.1.3  
**Title:** Statement of Applicability not formally approved  
**Finding:** An SoA has been produced during this engagement but has not been reviewed or approved by management. Several control exclusions lack documented justification.  
**Recommendation:** Obtain formal management approval of SoA. Document justification for all excluded controls.  
**Target Date:** 15 July 2025  

---

### Clause 7 — Support

#### Finding 7.1 — Major Non-Conformity
**Clause:** 7.2, 7.3  
**Title:** No security awareness training programme exists  
**Finding:** No security awareness training has been conducted for any employee. No training records exist. Staff interviewed during fieldwork were unable to identify basic security responsibilities or incident reporting procedures.  
**Evidence:** No training records. No training calendar. Simulated phishing test conducted during audit — 7 of 10 staff clicked the simulated phishing link.  
**Risk:** Human error accounts for 95% of breaches. Untrained staff represent the highest risk vector for SecureFinX.  
**Recommendation:** Design and deliver mandatory security awareness training within 60 days. Implement quarterly phishing simulations. Track completion rates.  
**Target Date:** 31 July 2025  

#### Finding 7.2 — Minor Non-Conformity
**Clause:** 7.5  
**Title:** Documented information not adequately controlled  
**Finding:** Policies and procedures exist informally in shared drives without version control, owner assignment, or review dates. Documents cannot be verified as current or authorised.  
**Recommendation:** Implement document control procedure: version numbers, owners, review dates, approval signatures required for all ISMS documents.  
**Target Date:** 30 June 2025  

---

### Clause 8 — Operations

#### Finding 8.1 — Major Non-Conformity
**Clause:** 8.1  
**Title:** No operational security controls documented or verified  
**Finding:** Security controls are applied inconsistently across systems. No operational procedures exist for key security activities including access provisioning, patch management, backup verification, or incident handling.  
**Evidence:** Access provisioning is ad-hoc. Patch management SLA undefined. Last backup restore test: never conducted. No incident log maintained.  
**Risk:** Without documented operational controls, SecureFinX cannot demonstrate consistent security management to auditors or regulators.  
**Recommendation:** Document operational procedures for: access provisioning, patch management, backup testing, incident handling, and change management.  
**Target Date:** 31 July 2025  

#### Finding 8.2 — Major Non-Conformity
**Clause:** 8.2  
**Title:** Formal risk assessment not conducted prior to this audit  
**Finding:** No evidence of any risk assessment conducted by SecureFinX prior to this engagement. Risk Register was produced by the external GRC consultant — not by internal staff.  
**Recommendation:** Train internal staff to conduct and maintain the risk register independently. Schedule annual risk assessment with internal ownership.  
**Target Date:** 31 August 2025  

---

### Clause 9 — Performance Evaluation

#### Finding 9.1 — Major Non-Conformity
**Clause:** 9.1  
**Title:** No monitoring, measurement, or KPI framework for information security  
**Finding:** SecureFinX has no security metrics, KPIs, or reporting mechanisms. Management receives no regular security performance updates. There is no SIEM, no security dashboard, and no defined monitoring programme.  
**Evidence:** No security reports found. No SIEM deployed. No KRI/KPI framework.  
**Risk:** Without measurement, SecureFinX cannot demonstrate security improvement or identify degradation over time — a core ISO 27001 requirement.  
**Recommendation:** Define 5–10 security KPIs (patch compliance rate, phishing click rate, access review completion, incident count, backup success rate). Report monthly to management.  
**Target Date:** 31 August 2025  

#### Finding 9.2 — Minor Non-Conformity
**Clause:** 9.2  
**Title:** No prior internal audit conducted  
**Finding:** This engagement represents the first internal audit ever conducted by or for SecureFinX. ISO 27001 requires internal audits to be conducted at planned intervals.  
**Recommendation:** Establish annual internal audit schedule. Appoint internal audit lead. Document audit programme and maintain audit records.  
**Target Date:** Ongoing — annual  

#### Finding 9.3 — Minor Non-Conformity
**Clause:** 9.3  
**Title:** No management review of ISMS conducted  
**Finding:** No evidence of management review meetings discussing security performance, risks, or ISMS effectiveness.  
**Recommendation:** Schedule bi-annual management review meetings. Document agenda, attendance, decisions, and action items.  
**Target Date:** 31 July 2025  

---

### Clause 10 — Improvement

#### Finding 10.1 — Minor Non-Conformity
**Clause:** 10.1, 10.2  
**Title:** No corrective action process defined  
**Finding:** No formal process exists for identifying, documenting, and tracking corrective actions arising from audit findings, incidents, or management reviews.  
**Recommendation:** Implement corrective action register. Assign owners and target dates to all findings. Review status monthly.  
**Target Date:** 30 June 2025  

---

## 5. Annex A Control Findings

### Critical Control Gaps Identified

| Control | Ref | Finding | Severity |
|---------|-----|---------|----------|
| MFA not enforced | A.8.5 | Single-factor authentication on all critical systems including AWS Console | Major |
| No privileged access management | A.8.2 | Shared admin credentials — single IT admin has unrestricted access to all production systems | Major |
| No vulnerability scanning | A.8.8 | No CVE monitoring or patch management SLA — known vulnerabilities undetected | Major |
| No logging or monitoring | A.8.15, A.8.16 | Logs exist but not centralised, reviewed, or alerted — dwell time risk critical | Major |
| S3 bucket misconfiguration | A.8.9 | Public access not explicitly blocked on S3 buckets storing Aadhaar data — CRITICAL risk | Major |
| No network segmentation | A.8.22 | Flat network — development and production on same network segment | Minor |
| Backup never tested | A.8.13 | Backups exist but restore has never been tested — recovery capability unverified | Minor |
| No vendor security assessment | A.5.19 | Critical vendors (AWS, payment gateway, KYC partner) not formally assessed | Minor |
| No data classification | A.5.12 | Data not formally classified — Aadhaar data treated same as public data | Minor |
| No BYOD controls | A.8.1 | Personal devices access corporate systems without MDM or endpoint protection | Minor |

---

## 6. Corrective Action Plan

| Finding ID | Non-Conformity | Severity | Owner | Target Date | Status |
|-----------|----------------|----------|-------|-------------|--------|
| F-5.1 | No CISO appointed — no management commitment | Major | CEO | 15 Jun 2025 | Open |
| F-6.1 | Risk assessment methodology not documented | Major | CISO | 30 Jun 2025 | Open |
| F-7.1 | No security awareness training | Major | HR + IT | 31 Jul 2025 | Open |
| F-8.1 | No operational security procedures | Major | IT Manager | 31 Jul 2025 | Open |
| F-9.1 | No security KPIs or monitoring | Major | CISO | 31 Aug 2025 | Open |
| A.8.5 | MFA not enforced | Major | IT Manager | 30 Jun 2025 | Open |
| A.8.2 | No PAM — shared admin credentials | Major | IT Manager | 30 Jun 2025 | Open |
| A.8.8 | No vulnerability scanning | Major | IT Manager | 31 Jul 2025 | Open |
| A.8.15 | No SIEM or centralised logging | Major | IT Manager | 31 Aug 2025 | Open |
| A.5.1 | No formal policy suite | Minor | CISO | 30 Jun 2025 | Open |
| A.5.12 | No data classification | Minor | DPO | 31 Jul 2025 | Open |
| A.8.13 | Backups never tested | Minor | IT Manager | 30 Jun 2025 | Open |
| A.5.19 | No vendor security assessment | Minor | COO | 31 Jul 2025 | Open |
| A.8.22 | No network segmentation | Minor | IT Manager | 31 Aug 2025 | Open |

---

## 7. Recommendations Summary

### Immediate (Within 30 days)
1. Appoint CISO and formally approve information security policy
2. Enable MFA on all systems — starting with AWS Console and production databases
3. Enable S3 Block Public Access on all buckets storing customer data
4. Implement privileged access management — separate admin accounts
5. Document and approve ISMS scope and risk assessment methodology

### Short-term (30–90 days)
6. Deploy SIEM or centralised logging solution
7. Launch mandatory security awareness training programme
8. Conduct and document backup restore test
9. Implement patch management process with defined SLA
10. Complete vendor security assessments for all critical vendors

### Medium-term (90–180 days)
11. Implement network segmentation — separate production and development
12. Deploy MDM for all devices accessing corporate systems
13. Establish security KPI dashboard and monthly management reporting
14. Conduct penetration test on payment application
15. Begin ISO 27001 certification readiness programme

---

## 8. Audit Conclusion

SecureFinX Pvt. Ltd. is at an early stage of its information security journey. The organisation demonstrates willingness to improve — evidenced by commissioning this audit and the GRC portfolio work completed during this engagement.

However, significant foundational gaps must be addressed before ISO 27001 certification is achievable.

**Estimated timeline to certification readiness: 6–9 months** with dedicated resource and management commitment.

The corrective action plan in Section 6 provides a structured roadmap. A follow-up internal audit is recommended in 90 days to assess progress.

---

## 9. Auditor Declaration

> I confirm that this audit was conducted independently and objectively, based on evidence gathered during the audit fieldwork. Findings are documented accurately and recommendations are made in good faith to support SecureFinX's information security improvement programme.

**Auditor:** Tusya Subramaniyan  
**Role:** GRC Consultant  
**LinkedIn:** [linkedin.com/in/tusya](https://linkedin.com/in/tusya)  
**College:** VIT Chennai — B.Tech Cybersecurity (2025–2029)  
**Date:** May 2025  

---

*This internal audit report was produced as part of a self-directed GRC portfolio project. SecureFinX Pvt. Ltd. is a fictional company created for educational purposes. All findings, non-conformities, and recommendations are hypothetical and designed to demonstrate ISO 27001 internal audit competency.*
