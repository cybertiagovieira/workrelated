# Comprehensive Meeting Minutes & Strategic Guidance Summary

**Meeting Title:** EASM Support Mission — Methodology, Findings & Reporting Guidance  
**Date & Time:** September 18, 2026 | ~14:00 – 15:00  
**Meeting Purpose:** Guidance session with Charlotte (Senior Advisor) to discuss the Cyber Risk Intelligence team's External Attack Surface Management (EASM) mission, refining audit methodologies, asset reconciliation strategies, empirical testing frameworks, and executive presentation deliverables.  
**Mission Duration:** ~3 to 3.5 months (Initiated late August / early September; target completion by end of Q4 / end of year).

---

## 1. Attendees & Stakeholder Map

### Active Meeting Participants
* **Charlotte** – Senior Advisor / Knowledge Provider (Sharing audit methodologies, past lessons learned from Detection & Response assessments, L'Oréal CMDB ownership experience, and standardized reporting frameworks).
* **Tiago** – EASM Mission Team Member (Cyber Risk Intelligence).
* **Jules** – EASM Mission Team Member (Cyber Risk Intelligence).
* **Thomas** – EASM Mission Team Member (Cyber Risk Intelligence).

### Key Organizational Stakeholders & Roles
* **Gerard** – Sponsor / Management Lead who initiated the EASM mission to address historical inventory oversight gaps and regulatory expectations.
* **Sharif** – Management Lead / Principal Reviewer of assessment deliverables prior to broad distribution.
* **Frank & Olivia** – Key internal executive stakeholders and primary report recipients.
* **Grégoire** – Former Head of Cyber Security under whom historical inventory responsibilities shifted to the 1st Line of Defense (1LoD).

---

## 2. Mission Background, Context & Regulatory Rationale

### A. Historical Governance Shift (3-Year Context)
* **Central Oversight to 1LoD:** Approximately three years ago (under Grégoire's tenure), management shifted responsibility for asset inventory management and security tooling costs from central Cyber Security to the **First Line of Defense (1LoD)** entities.
* **Tool Adoption & Limitations (Qualys):** To minimize cost, 1LoD entities relied heavily on **Qualys**. However, Qualys operates strictly on a **user-defined target model**—it only scans assets explicitly specified and submitted by the entity.
* **The Perimeter Blind Spot:** If an entity owns 200 external assets but only inputs 150 into Qualys, the remaining 50 assets exist as unmonitored, unmanaged blind spots (Shadow IT).

### B. European Central Bank (ECB) Rationale
* **Regulatory Inquiries:** The ECB repeatedly raised audit points regarding asset inventory completeness, unmanaged external perimeter assets, and attack surface visibility.
* **Mission Origin:** Although previous ECB points were formally closed with past evidence, structural gaps remained. **Gerard** commissioned this dedicated EASM mission within Cyber Risk Intelligence to establish full visibility and validate perimeter completeness across all bank entities.

---

## 3. Current Mission Status & Early Work Completed

* **Mission Letter & Kickoff:** The formal Mission Letter has been officially approved by management. Official dispatch by Sharif/Gerard is occurring immediately. The formal kickoff meeting with audited 1LoD teams will follow shortly.
* **Work Completed Pre-Kickoff:**
  1. **Documentation Review:** Extensive background research across internal SharePoint repositories and RefWeb.
  2. **External Reconnaissance Data:** Initial ingestion and analysis of external threat intelligence exposure data via **BitSight** to measure visible external perimeter coverage.
  3. **Cloud Security Alignment:** Preliminary informal alignment with the internal **Cloud Security team** (within the Cyber Risk Intelligence unit) to gauge known cloud perimeter gaps.
* **Scope Definition:** The mission is fundamentally a **Process and Governance Assessment**, complemented by rigorous **passive data analytics** and structural verification.

---

## 4. Technical Guidance & Methodology (Charlotte's Insights)

### A. CMDB Reconciliation & Asset Discovery (Lessons from L'Oréal)
Drawing from her experience as a former CMDB Product Owner at L'Oréal, Charlotte highlighted key principles for identifying Shadow IT:
1. **"Monitoring Starts with Inventorying":** Security monitoring is ineffective if asset scope is unknown.
2. **Reconciliation via Security Tool Inventories:** CMDB records are rarely exhaustive. Cross-reference CMDB data against the internal **Cyber Tool Map** and individual security platform registries. Assets often exist inside security tooling portals even when omitted from the central CMDB.
3. ** Granular CMDB Discrepancies:** "The devil is always in the details." A higher-level category or server title existing in the CMDB does not mean all sub-assets, database instances, or network routers under it are cataloged.
4. **Addressing Discovery Tool Overwhelm (e.g., Tanium):**
   * Organizations often deploy discovery engines like **Tanium Discovery**, but these tools frequently uncover vast quantities of unmanaged assets.
   * Operational teams often feel overwhelmed by the volume and "close the window," ignoring discovery outputs.
   * **Audit Focus:** Assess whether 1LoD possesses a formal **governance, prioritization, and onboarding framework** to systematically integrate discovered assets into the CMDB via a structured roadmap.

### B. Assessment Approach: Data Analytics vs. Exploitation
1. **Passive Reconnaissance & Pantera Usage:**
   * Management expects empirical validation. Where management requests testing via **Pantera**, leverage it for **passive data analytics and asset coverage checks** (counting exposed endpoints, comparing directly against CMDB entries) rather than active exploitation.
   * **Resource Workaround:** If Pantera license credits are limited, supplement with **open-source intelligence (OSINT) reconnaissance tools** to achieve complete perimeter discovery.
2. **Value of Concrete Practical Checks (Detection & Response Case Study):**
   * Charlotte shared an example from her *Detection & Response Assessment*: To test SIEM coverage for vital services, she had an administrator click on a designated honeypot asset.
   * **Finding:** ITG and CIB systems reacted differently; one failed to raise an alert. Presenting this practical, concrete finding delivered immense value to management without requiring a full Red Team penetration test.
3. **Operational Walkthroughs vs. Manager Interviews:**
   * High-level managers provide an idealized governance view.
   * **Core Directive:** Schedule **hands-on tool walkthroughs and live demonstrations directly with technical experts and tool operators**. Operational specialists will candidly demonstrate actual tool workflows, manual workarounds, and real-world gaps.

### C. Governance Artifacts & Audit Trail Investigation
1. **Prior CMDB Permanent Control Actions (PCAs):** Identify and request all prior PCAs related to inventory management to evaluate past remediation commitments and verify whether past issues were truly resolved.
2. **ServiceNow Risk Acceptances:**
   * Request formal **Risk Acceptance records** registered in ServiceNow.
   * When entities cannot meet standards (e.g., unsynchronized databases, missing discovery scans, unpatched assets), they formally log risk acceptances. Reviewing these reveals known, management-approved operational gaps.
3. **CMDB Audit Sensitivity:** Check political sensitivity with leadership before deep-diving into CMDB coverage, as previous ECB remediation closures make CMDB scope politically delicate in certain entities.

---

## 5. Reporting Framework & Deliverable Architecture

Charlotte presented a standardized report structure optimized for both executive oversight and granular technical replication:

```
┌─────────────────────────────────────────────────────────┐
│                    EXECUTIVE SUMMARY                    │
│ Perimeter Scope | Recap Table (Scope/Target/PCA) | Roadmap│
└────────────────────────────┬────────────────────────────┘
                             │
                             ▼
┌─────────────────────────────────────────────────────────┐
│              OBSERVATION SLIDES (1-PAGERS)              │
│ Scope | Risk Statement | Context | Description | PCAs   │
└────────────────────────────┬────────────────────────────┘
                             │
                             ▼
┌─────────────────────────────────────────────────────────┐
│                  TECHNICAL APPENDICES                   │
│   Methodology | Sampling | Screenshots | Data Analytics │
└────────────────────────────┬────────────────────────────┘
```

### Key Components of the Deliverable Architecture:
1. **Executive Summary Deck:**
   * **Perimeter Scope Slide:** Clear visual boundary of assessed entities and assets.
   * **Observation Recap Table:** Summary table listing all observations (e.g., 13 total findings), applicable entities, target completion dates, and scope breakdown.
   * **Executive Timeline & Roadmap:** High-level remediation schedule.
2. **Standardized 1-Page Observation Slides:**
   * **Structure:** Single-page format containing *Scope*, *Risk Statement*, *Context*, *Synthesized Observation Description*, and *Permanent Control Action (PCA) Plans*.
   * **Drill-Down Links:** Executive summary lines hyper-link directly to the 1st paragraph synthesis on the respective observation slide.
3. **Technical Appendices (Audit Evidence):**
   * Detailed test objectives, sampling sizes, step-by-step methodologies, software screenshots, data analysis results, and explicit conclusions.
4. **Excel Replicability Principle (Header Sheet Mandate):**
   * Every analytical Excel workbook created during testing **MUST** include a dedicated front header sheet defining:
     * **Test Objective**
     * **Sampling Methodology**
     * **Step-by-Step Execution Procedure**
   * *Rule:* Any independent auditor or team member reading the workbook must be able to replicate the exact analysis and achieve identical results.

---

## 6. Communication Governance & Confidentiality Protocols

* **Management Review Sequence:** Report drafts and strategic findings must be reviewed by **Sharif** and **Gerard** prior to distribution to external executive stakeholders (such as Frank). Senior management must not be surprised by findings circulated prematurely.
* **Template Reuse vs. Confidential Data:** Draft assessment decks marked "Do Not Distribute" contain sensitive operational data and must remain restricted. Report layout structure and design templates are extracted for mission reuse.

---

## 7. Action Item Summary & Roadmap

| # | Action Item | Primary Owner | Target / Status |
|---|---|---|---|
| **1** | Finalize distribution of official Mission Letter to 1LoD entities | Management (Sharif / Gerard) | Immediate (Today/Monday) |
| **2** | Extract reporting slide templates and Excel header sheet frameworks | Jules / Charlotte | Completed |
| **3** | Formulate interview and walkthrough schedule focusing on operational tool specialists | Tiago / Jules / Thomas | Post-Kickoff |
| **4** | Request historical **CMDB PCAs** and **ServiceNow Risk Acceptance** repositories | EASM Mission Team | Upcoming Sprint |
| **5** | Execute passive data analytics combining **BitSight**, **Cyber Tool Maps**, and **OSINT tools** | EASM Mission Team | Ongoing |
| **6** | Review 1LoD **Tanium Discovery** implementation and asset onboarding governance | EASM Mission Team | Assessment Phase |
