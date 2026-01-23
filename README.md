# Improving Nephrology Clinical Workflow Operations Project

<p align="center">
  <img
    src="https://github.com/user-attachments/assets/de5abf8c-3fdc-4026-9929-0f89f1dd58c7"
    alt="Stanford Medicine"
    style="max-width: 70%; height: auto;"
    />
</p>

*Conducted as part of a consulting externship in collaboration with Stanford Medicine through Extern.*

## Executive Summary:
Nephrology clinics manage high-risk patients who require timely review of lab results and rapid clinical escalation. This project analyzed real nephrology clinic workflows to identify breakdowns in lab review, role clarity, and escalation processes that can delay care and increase patient safety risk. Using root cause analysis, clinical guideline mapping, and process design principles, the project translated complex clinical rules into clear decision pathways and a role-aware decision-support dashboard. The goal was to improve care coordination, reduce escalation delays, and support safer, more reliable clinical decision-making in busy nephrology clinic environments at Stanford Medicine.

### Business Problem:
The primary goal was to design clearer workflows and decision-support mechanisms that ensure critical lab results are reviewed, escalated, and acted upon promptly—without overburdening clinical staff or disrupting existing clinic operations. This is crucial as nephrology clinics handle patients with chronic kidney disease who are especially vulnerable to abnormal lab results such as elevated potassium levels. In practice, lab values requiring urgent action may be reviewed late or escalated inconsistently due to unclear role ownership, fragmented workflows, and competing clinical priorities. These gaps can delay intervention and increase the risk of patient harm. 

### Methodology:
_**1. Stakeholder & Role Mapping**_<br>
Mapped core nephrology clinic roles—physicians, registered nurses, advanced practice providers, and care coordinators—to understand how responsibilities for lab review, escalation, and follow-up were distributed. This surfaced role boundaries, workload pressures, and coordination gaps that contributed to delayed action on abnormal lab results.

_**2. Workflow Breakdown & Root Cause Analysis**_<br>
Analyzed a representative high-risk case involving severe hyperkalemia (>6.2 mmol/L) to identify failure points in the existing workflow. Root cause analysis (Fishbone diagram - see figure below) revealed systemic contributors across people, process, technology, and operations, including unclear ownership, alert fatigue, and lack of standardized escalation thresholds.

<img width="1442" height="492" alt="image" src="https://github.com/user-attachments/assets/128a9ead-e769-4dc3-9f7b-3cf08a0ea67d" />
<figcaption>Fishbone (Ishikawa) analysis identifying systemic contributors to delayed hyperkalemia escalation across people, process, technology, and management factors.</figcaption> <br>

_Key Root Causes Identified:_<br>
- Role ambiguity in time-based accountability for lab review
- Absence of standardized escalation protocols for critical potassium values
- Limited EHR support for urgency differentiation and acknowledgment tracking
- High patient volume reducing follow-up capacity
- Lack of feedback loops to detect repeated missed alerts
  
_**3. Clinical Guideline to Decision Logic Translation**_<br>
Translated established nephrology and patient safety guidelines into explicit, step-by-step decision logic defining escalation timing, clinical risk stratification, and role-specific responsibilities. The logic was visualized as a flowchart to enable fast, consistent escalation decisions during time-constrained clinical work.

_**4. Decision-Support Design & Adoption Planning**_<br>
Prototyped a role-aware decision-support dashboard to surface urgent lab results, recommended actions, and documentation requirements. Developed an adoption plan using Kotter’s Change Model, including role-based training, resistance mitigation, and success metrics focused on escalation timeliness and error reduction.

### Skills:<br>
- Clinical workflow analysis and process design  
- Stakeholder mapping and role-based responsibility modeling  
- Root cause analysis (Fishbone, 5 Whys)  
- Translation of clinical guidelines into decision logic  
- Decision-support system design (role-aware, time-bound escalation)  
- Healthcare operations and patient safety analysis  
- Change management and adoption planning  
- Data-informed dashboard prototyping for clinical use cases  

### Results:<br>
- Established a standardized, guideline-driven escalation framework for hyperkalemia management in nephrology clinics.
- Clarified ownership and timing of lab review and escalation across physicians, nurses, APPs, and care coordinators.
- Translated complex clinical rules into actionable, role-aware decision pathways that reduce ambiguity and escalation delays.
- Demonstrated how decision-support tools can surface urgent cases, recommended actions, and documentation needs without increasing alert fatigue.

<img width="1310" height="708" alt="image" src="https://github.com/user-attachments/assets/56961f2d-17d8-447f-aa1b-cd1e0c91521d" />
<figcaption>Role-aware nephrology decision-support dashboard highlighting clinician priorities, quick actions, and active lab alerts.</figcaption>

<img width="1272" height="468" alt="image" src="https://github.com/user-attachments/assets/2e0301c1-5a89-4a6e-8fac-98df4d86f6fd" />
<figcaption>Centralized potassium monitoring table surfacing critical, elevated, and normal lab values with timestamps and recommended protocol access.</figcaption>

<img width="1270" height="840" alt="image" src="https://github.com/user-attachments/assets/7f846dbc-da9d-4e1c-9762-551d1f69710c" />
<figcaption>Guideline-driven escalation view for Patient A of hyperkalemia level at 6.2 mmol/L: including urgency level, escalation timeline, and role-appropriate clinical actions.</figcaption>

<img width="1262" height="841" alt="image" src="https://github.com/user-attachments/assets/f156e350-7b71-4baf-99cf-3febaa74934c" />
<figcaption>Guideline-driven escalation view for Patient D of hyperkalemia level at 5.3 mmol/L: including urgency level, escalation timeline, and role-appropriate clinical actions.</figcaption>

<img width="1250" height="772" alt="image" src="https://github.com/user-attachments/assets/aa518ebd-2f15-4652-a36d-5e6859997f8e" />
<figcaption>Guideline-driven escalation view for Patient C of hyperkalemia level at 4.5 mmol/L: including urgency level, escalation timeline, and role-appropriate clinical actions.</figcaption>

**Key Business Recommendations:**
- Deploy role-aware decision-support views to align escalation actions with scope of practice, reducing hesitation and informal workarounds during critical lab events.
- Use time-based escalation thresholds (e.g., lab review within 1 hour, intervention within 2 hours) to improve accountability and reduce delays in high-risk cases.
- Leverage centralized lab monitoring tables to prioritize clinician attention toward critical and overdue results without increasing alert fatigue.
- Standardize documentation prompts within the workflow to support auditability, quality improvement, and patient safety reporting.
- Pilot the dashboard with a small subset of nephrology teams to validate usability, adoption, and escalation timeliness before broader rollout.

## Limitations & Next Steps
**Current Limitations**

Prototype-level decision support: The dashboard and decision logic were developed as a conceptual and workflow-level prototype. While grounded in real clinic workflows and guidelines, the solution was not integrated into the live EHR environment, limiting real-time validation under production constraints.

Focused clinical scope: The analysis and decision logic centered primarily on hyperkalemia escalation to illustrate high-risk lab handling. Other nephrology-related abnormalities (e.g., creatinine trends, fluid overload indicators) were not modeled in this phase.

Workflow simulation over longitudinal measurement: Improvements in escalation timeliness and error reduction were demonstrated through workflow analysis and scenario walkthroughs rather than longitudinal outcome data or controlled pilots.

Change adoption assumptions: Adoption planning accounted for role-based training and resistance mitigation, but actual behavioral adoption, alert adherence, and workload impact were not measured through live clinician usage.

**Next Steps**

Pilot integration within the EHR environment: Integrate the decision-support logic into existing EHR workflows to evaluate real-world usability, alert responsiveness, and impact on escalation timelines without increasing clinician burden.

Expand decision logic to additional nephrology risks: Extend the framework to cover other high-risk lab patterns and longitudinal trends, enabling a more comprehensive safety monitoring system for chronic kidney disease management.

Implement feedback and audit loops: Add mechanisms to track missed alerts, delayed escalations, and override patterns to support continuous quality improvement and patient safety reporting.

Evaluate outcomes and operational impact: Measure key metrics such as time-to-escalation, intervention delays, and clinician workload before and after deployment to quantify safety and efficiency gains.

Scale role-aware decision support across specialties: Apply the same role-mapped, guideline-driven design approach to other clinical domains where time-sensitive lab interpretation and escalation are critical.

