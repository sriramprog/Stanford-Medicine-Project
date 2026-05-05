# 🏥 Nephrology Clinical Workflow Intelligence — Stanford Medicine

![Root Cause Analysis](https://img.shields.io/badge/Method-Root_Cause_Analysis-00A67E)
![Decision Support](https://img.shields.io/badge/Output-Decision_Support_Dashboard-0057A8)
![Change Management](https://img.shields.io/badge/Framework-Kotter's_Change_Model-6C3483)
![License](https://img.shields.io/badge/License-Portfolio-lightgrey)

> **Extern × Stanford Medicine**  
> A clinical workflow analytics project analyzing nephrology lab escalation failures, translating complex clinical guidelines into role-aware decision logic, and prototyping a decision-support dashboard to reduce critical lab review delays and patient safety risk.

---

## 📋 Table of Contents

- [Problem Statement](#-problem-statement)
- [What It Does](#-what-it-does)
- [System Architecture](#-system-architecture)
- [Methodology Walkthrough](#-methodology-walkthrough)
- [Results & Impact](#-results--impact)
- [Skills](#-skills)
- [Design Decisions & Trade-offs](#-design-decisions--trade-offs)
- [Limitations & Next Steps](#-limitations--next-steps)
- [Repository Structure](#-repository-structure)

---

## 🎯 Problem Statement

Nephrology clinics manage high-risk chronic kidney disease patients who require timely review of lab results and rapid clinical escalation. In practice, critical lab values — such as severely elevated potassium — may be reviewed late or escalated inconsistently due to unclear role ownership, fragmented workflows, and competing clinical priorities. These gaps delay intervention and increase patient safety risk.

| Pain Point | How This Project Addresses It |
|---|---|
| Unclear escalation ownership | Mapped role-specific responsibilities across physicians, nurses, APPs, and care coordinators |
| No standardized escalation thresholds | Translated clinical guidelines into explicit, time-bound decision logic |
| Alert fatigue from undifferentiated notifications | Designed urgency-stratified dashboard views that prioritize critical cases |
| Delayed lab-to-action times | Established 1-hour review / 2-hour intervention benchmarks with accountability tracking |

---

## ✅ What It Does

1. **Maps** nephrology clinic roles to understand how lab review, escalation, and follow-up responsibilities are distributed — surfacing role boundaries and coordination gaps
2. **Analyzes** a representative high-risk hyperkalemia case using root cause analysis (Fishbone / Ishikawa) to identify systemic failure points across people, process, technology, and operations
3. **Translates** complex clinical guidelines into step-by-step decision logic defining escalation timing, risk stratification, and role-specific actions
4. **Visualizes** the decision logic as a flowchart enabling fast, consistent escalation decisions during time-constrained clinical work
5. **Prototypes** a role-aware decision-support dashboard surfacing urgent lab results, recommended actions, and documentation requirements
6. **Plans** adoption using Kotter's Change Model, including role-based training, resistance mitigation, and success metrics

---

## 🏗️ System Architecture

```
CLINICAL WORKFLOW PROBLEM
         │
         ▼
┌─────────────────────────────┐
│  Stakeholder & Role Mapping │
│  (Physicians, RNs, APPs,    │
│   Care Coordinators)        │
└─────────────┬───────────────┘
              │
              ▼
┌─────────────────────────────┐
│  Root Cause Analysis        │
│  Fishbone Diagram           │
│  (People / Process /        │
│   Technology / Operations)  │
└─────────────┬───────────────┘
              │
              ▼
┌─────────────────────────────┐
│  Clinical Guideline →       │
│  Decision Logic Translation │
│  (Escalation Flowchart)     │
└─────────────┬───────────────┘
              │
              ▼
┌──────────────────────────────────────────────────────────┐
│                    DECISION SUPPORT LAYER                 │
│                                                          │
│  Role-Aware Dashboard → Lab Urgency Stratification       │
│    → Escalation Timeline View                            │
│      → Documentation Prompts                             │
│        → Adoption Plan (Kotter's Change Model)           │
└──────────────────────────────────────────────────────────┘
```

### Component Overview

| Component | Approach | Output |
|---|---|---|
| Role Mapping | Stakeholder interviews & workflow tracing | Responsibility matrix across 4 role types |
| Root Cause Analysis | Fishbone (Ishikawa) diagram | Systemic contributors across 4 domains |
| Decision Logic | Clinical guideline translation | Step-by-step escalation flowchart |
| Risk Stratification | Hyperkalemia severity banding | Urgency tiers: Critical / Elevated / Normal |
| Dashboard Prototype | Role-aware decision-support design | 3-panel UI: priorities, lab table, escalation view |
| Adoption Planning | Kotter's 8-Step Change Model | Training plan, resistance mitigation, KPIs |

---

## 🔬 Methodology Walkthrough

**Step 1 — Stakeholder & Role Mapping**  
Mapped core nephrology clinic roles — physicians, registered nurses, advanced practice providers, and care coordinators — to understand how responsibilities for lab review, escalation, and follow-up were distributed. This surfaced role boundaries, workload pressures, and coordination gaps contributing to delayed action on abnormal lab results.

**Step 2 — Workflow Breakdown & Root Cause Analysis**  
Analyzed a representative high-risk case involving severe hyperkalemia (>6.2 mmol/L) to identify failure points in the existing workflow. A Fishbone (Ishikawa) root cause analysis revealed systemic contributors across four domains:

| Domain | Key Contributors |
|---|---|
| People | Role ambiguity in time-based accountability for lab review |
| Process | Absence of standardized escalation protocols for critical potassium values |
| Technology | Limited EHR support for urgency differentiation and acknowledgment tracking |
| Operations | High patient volume reducing follow-up capacity; no feedback loops for repeated missed alerts |

**Step 3 — Clinical Guideline to Decision Logic Translation**  
Translated established nephrology and patient safety guidelines into explicit, step-by-step decision logic defining escalation timing, clinical risk stratification, and role-specific responsibilities. The logic was visualized as a flowchart to enable fast, consistent escalation decisions during time-constrained clinical work.

**Step 4 — Decision-Support Design & Adoption Planning**  
Prototyped a role-aware decision-support dashboard to surface urgent lab results, recommended actions, and documentation requirements. Developed an adoption plan using Kotter's Change Model, including role-based training, resistance mitigation, and success metrics focused on escalation timeliness and error reduction.

---

## 📊 Results & Impact

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/56961f2d-17d8-447f-aa1b-cd1e0c91521d"
    alt="Role-aware nephrology decision-support dashboard"
    style="max-width: 90%; height: auto;"
    />
</p>
<p align="center"><em>Role-aware nephrology decision-support dashboard highlighting clinician priorities, quick actions, and active lab alerts.</em></p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/2e0301c1-5a89-4a6e-8fac-98df4d86f6fd"
    alt="Centralized potassium monitoring table"
    style="max-width: 90%; height: auto;"
    />
</p>
<p align="center"><em>Centralized potassium monitoring table surfacing critical, elevated, and normal lab values with timestamps and recommended protocol access.</em></p>

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/7f846dbc-da9d-4e1c-9762-551d1f69710c"
    alt="Escalation view — Patient A, hyperkalemia 6.2 mmol/L"
    style="max-width: 90%; height: auto;"
    />
</p>
<p align="center"><em>Guideline-driven escalation view for Patient A (hyperkalemia 6.2 mmol/L): urgency level, escalation timeline, and role-appropriate clinical actions.</em></p>

### Outcomes

| Outcome | Detail |
|---|---|
| Standardized escalation framework | Guideline-driven protocol for hyperkalemia management established across all role types |
| Role clarity | Ownership and timing of lab review and escalation clarified across physicians, nurses, APPs, and care coordinators |
| Reduced decision ambiguity | Complex clinical rules translated into actionable, role-aware decision pathways |
| Alert fatigue mitigation | Dashboard surfaces urgency-stratified cases without increasing notification volume |

**Key Business Recommendations:**
- Deploy role-aware decision-support views to align escalation actions with scope of practice, reducing hesitation and informal workarounds during critical lab events
- Use time-based escalation thresholds (lab review within 1 hour, intervention within 2 hours) to improve accountability and reduce delays in high-risk cases
- Leverage centralized lab monitoring tables to prioritize clinician attention toward critical and overdue results without increasing alert fatigue
- Standardize documentation prompts within the workflow to support auditability, quality improvement, and patient safety reporting
- Pilot the dashboard with a small subset of nephrology teams to validate usability, adoption, and escalation timeliness before broader rollout

---

## 🛠️ Skills

| Category | Skill |
|---|---|
| Workflow Analysis | Clinical workflow mapping and process design |
| Stakeholder Work | Role-based responsibility modeling and stakeholder mapping |
| Root Cause Analysis | Fishbone (Ishikawa) diagram, 5 Whys |
| Clinical Translation | Guideline-to-decision-logic translation for time-constrained clinical environments |
| Decision Support Design | Role-aware, time-bound escalation system prototyping |
| Healthcare Operations | Patient safety analysis, EHR workflow assessment |
| Change Management | Kotter's 8-Step Change Model, adoption and resistance planning |
| Dashboard Prototyping | Data-informed UI design for clinical decision support |

---

## ⚖️ Design Decisions & Trade-offs

| Decision | Rationale | Trade-off |
|---|---|---|
| Focused on hyperkalemia as the primary case | High-risk, high-frequency scenario that clearly illustrates escalation failure patterns | Other nephrology abnormalities (creatinine trends, fluid overload) not modeled in this phase |
| Prototype dashboard over EHR integration | Faster iteration and stakeholder feedback without EHR access constraints | Real-time validation under production constraints not possible at this stage |
| Fishbone over quantitative failure analysis | Appropriate for workflow-level root cause discovery without longitudinal outcome data | Improvements demonstrated through scenario walkthroughs, not measured longitudinally |
| Kotter's Change Model for adoption | Proven framework with clear, sequenced steps for clinical environment adoption | Actual behavioral adoption and alert adherence not measured through live clinician usage |

---

## ⚠️ Limitations & Next Steps

**Current Limitations**

1. **Prototype-level decision support** — The dashboard and decision logic were developed as a conceptual and workflow-level prototype. While grounded in real clinic workflows and guidelines, the solution was not integrated into the live EHR environment, limiting real-time validation under production constraints
2. **Focused clinical scope** — Analysis and decision logic centered primarily on hyperkalemia escalation. Other nephrology-related abnormalities (creatinine trends, fluid overload indicators) were not modeled in this phase
3. **Workflow simulation over longitudinal measurement** — Improvements in escalation timeliness and error reduction were demonstrated through workflow analysis and scenario walkthroughs rather than longitudinal outcome data or controlled pilots
4. **Change adoption assumptions** — Adoption planning accounted for role-based training and resistance mitigation, but actual behavioral adoption, alert adherence, and workload impact were not measured through live clinician usage

**Roadmap**

| Timeline | Enhancement |
|---|---|
| Short-term (2 weeks) | Pilot integration within the EHR environment to evaluate real-world usability and escalation timeliness |
| Medium-term (1 month) | Expand decision logic to additional nephrology risks (creatinine trends, fluid overload) |
| Long-term | Implement feedback and audit loops to track missed alerts, delayed escalations, and override patterns; measure time-to-escalation and intervention delays before and after deployment |

---

## 📁 Repository Structure

```
Stanford-Medicine-Project/
├── Stanford Medicine Externship.pdf   # Final stakeholder presentation
└── README.md                                # This file
```

---
