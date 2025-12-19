# Inbound Receiving Optimization — LPN Syntax Validation

## TL;DR
This case study demonstrates how a Business Analyst can identify an operational breakdown in inbound receiving, design a low-risk WMS enhancement, and define measurable outcomes without disrupting standard workflows.

---

## Business Context
Inbound receiving operations rely on accurate LPN (License Plate Number) scans to confirm inventory into a Warehouse Management System (WMS). In high-volume environments, visually similar barcodes and time pressure increase the likelihood of mis-scans. When incorrect LPNs are confirmed, errors propagate downstream, resulting in rework, delayed putaway, and inventory integrity issues.

This project models how a Business Analyst can formalize a recurring operational issue into a structured system improvement using standard BA artifacts and practices.

---

## Problem
The current receiving workflow accepts any scanned alphanumeric string as a valid LPN. There is no validation step to confirm that the scanned value matches expected inbound syntax patterns. As a result, incorrect pallets may be confirmed into inventory, particularly during peak receiving periods or when multiple pallets are staged together.

---

## Constraints
- No replacement or migration of the existing WMS
- No system downtime or data migration
- Minimal impact to associate workflows
- No changes to staffing, schedules, or throughput targets
- Solution must remain configurable and limited in scope

---

## Solution Overview
The proposed solution introduces a lightweight LPN prefix validation step during inbound receiving. When a scanned LPN does not match an approved prefix pattern, the system prompts the associate to re-scan for confirmation. If the mismatch persists, the transaction is canceled to prevent incorrect inventory confirmation.

The enhancement activates **only on exception scenarios**. Valid scans follow the existing “happy path” workflow without added steps.

---

## Repository Structure
This repository is organized to reflect the lifecycle of a business analysis engagement:

1. **Analysis** – problem definition, background, and root cause analysis  
2. **Requirements** – business and functional requirements, RTM, and user stories  
3. **Process Flows** – current and future state workflow diagrams  
4. **Change Management** – impact analysis and operational risk considerations  
5. **Metrics** – KPIs used to measure success post-implementation  

---

## Artifacts Included
- Problem Statement & Background  
- Root Cause Analysis (5 Whys)  
- Business Requirements  
- Functional Requirements  
- Acceptance Criteria  
- Requirements Traceability Matrix (RTM)  
- User Stories  
- Current-State Process Flow  
- Future-State Process Flow  
- Change Impact Summary  
- KPI & Expected Impact Analysis  

All artifacts are documented using WMS-agnostic terminology and standard Business Analyst practices.

---

## Metrics Intended
- Receiving accuracy percentage  
- Mis-scan incident count  
- Rework and inventory correction hours  
- Training time required for new associates  
- Exception frequency by associate or shift  

These metrics are intended to measure both immediate error reduction and longer-term behavioral reinforcement.

---

## Tools & Methods
- **Process Mapping:** diagrams.net (draw.io)  
- **Documentation:** Markdown (GitHub-rendered)  
- **Analysis Frameworks:** BABOK v3 concepts (process analysis, requirements analysis)  

No proprietary systems, datasets, or tools are required to understand or apply the proposed solution.

---

## Notes
- This is a fictionalized case study based on common warehouse operations patterns.
- No proprietary systems, data, or processes are referenced.
- Metrics are illustrative and intended to demonstrate analytical framing rather than actual performance.

---

## Next Iteration (Future Work)
- Add reporting to track validation exceptions by associate and shift  
- Introduce configurable prefix management for operations teams  
- Surface KPIs through a leadership-facing dashboard (e.g., Power BI)  
