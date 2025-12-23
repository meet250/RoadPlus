
RoadPlus

Operational Orchestration Platform for Urban Road Maintenance (B2G)

RoadPlus is a B2G product concept designed to reduce the cost, delay, and repeat failures in urban road maintenance.
It operates as a middle-layer platform between citizen-reported road issues and contractor execution, enabling cities to shift from reactive patching to performance-based maintenance.

The project was developed during my time at Nirma University Institute of Design, with a strong focus on product strategy, KPIs, unit economics, and incentive alignment rather than UI or visual design.



Problem Summary 

Cities like Ahmedabad spend crores annually on road repairs, yet:

* The same potholes reappear multiple times within a single monsoon
* Repair timelines stretch from days to weeks
* Contractors are paid per repair, not per outcome
* There is no single source of truth for road health or repair quality

Core issue:
The system rewards *speed and volume of patches*, not *durability or lifecycle cost reduction*.



Product Goal

Reduce the “Cost per Durable Patch” while improving SLA adherence and public trust.

RoadPlus reframes road repair as an operational and financial optimization problem, not just a civic complaint workflow.



 Target Users & Stakeholders

* Primary Buyer: City Government / AMC
* Primary Operators: Zonal Engineers, Supervisors
* Supply Side: Road Repair Contractors
* Demand Side: Citizens (reporting + verification)

Product Strategy (MVP Scope)

The MVP focuses on operational efficiency and accountability, not advanced AI or hardware.

 1. Intake Engine (Low-CAC Reporting)

* WhatsApp Business API + IVR
* Auto-capture of GPS, timestamp, and photos
* Attachment limits to control storage and verification costs

Why:
WhatsApp ensures high adoption with near-zero citizen onboarding cost.


 2. Dispatch & Prioritization Engine

* Rule-based priority queue (not ML in MVP)
* Inputs:

  * Road Tier (arterial / local)
  * Severity (water-filled, depth, width)
  * Traffic volume
* Zonal load balancing to maximize crew utilization

Why:
Predictable, auditable logic is critical for government adoption.



3. Trust & Accountability Layer

* Geo-fenced before/after photo verification
* Payment milestones linked to proof-of-work
* Warranty Lock:
  A portion of contractor payment is held for 90 days
  → forfeited if the same patch fails (re-reported)

Note:
This mirrors existing retention clauses used by civic bodies.

---

 System Architecture 

* Inputs: WhatsApp, IVR, AMC helpline
* Core System: Incident Management System + GIS
* Outputs:

  * Contractor Field App (task execution)
  * Admin Dashboard (SLA, cost, recurrence analytics)



Physical Layer (Phygital Component)

* Standardized on-site repair signage with job ID + QR
* Supervisor quality checklist
* GPS-tracked zonal repair crews

Insight:
Field signage and visibility increase citizen trust more than backend dashboards.



Key Metrics (North Star & Supporting KPIs)

North Star Metric:
Cost per Durable Patch

| Metric              | Definition                              | Target     |
| ------------------- | --------------------------------------- | ---------- |
| SLA Adherence       | % of issues fixed < 48 hrs              | > 90%      |
| Recurrence Rate     | % of patches failing within one monsoon | < 5%       |
| Operational Savings | Reduction in ad-hoc emergency tenders   | 25% YoY    |
| Citizen NPS         | Trust in civic response                 | +30 points |



 Unit Economics (Illustrative)

* Avg patch today: ₹10,000
* Avg repeat rate: ~3 times per monsoon → ₹30,000
* RoadPlus target:

  * 1 durable fix at ~₹12,000
* Net saving per location: ~₹18,000

This saving compounds across thousands of repairs annually.




 Incentive Alignment (Why Contractors Participate)

RoadPlus shifts contractors from:

* Repair Contracts → Maintenance Contracts

If a contractor keeps a road pothole-free for a defined period:

* They earn performance bonuses
* Bonuses exceed profits from repeated low-quality patches

Outcome:
Quality becomes more profitable than rework.



 Risks & Mitigation

* Government Change Management:
  Positioned as a budget leakage reduction tool, not “new tech”
* Data Manipulation:
  Multi-layer verification (Exif + geo-fence + citizen recheck)
* Adoption Friction:
  Integrates with existing AMC workflows, not replacements





 Why This Project Matters

RoadPlus treats civic infrastructure as a product with users, costs, incentives, and outcomes.


