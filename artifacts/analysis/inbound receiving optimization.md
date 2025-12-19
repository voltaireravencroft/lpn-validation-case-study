Business Context
Inbound receiving operations rely on accurate LPN (License Plate Number) scans to confirm inventory into a Warehouse Management System (WMS). In high-volume warehouse environments, associates often scan pallets in close proximity under time pressure. When LPN formats are visually similar and the system does not validate input, incorrect scans can be accepted and committed into inventory, creating downstream reconciliation work and operational inefficiencies.
This case study demonstrates how a Business Analyst can identify a recurring operational issue and propose a targeted system enhancement that improves accuracy without disrupting standard workflows.
________________________________________
Problem
The current receiving process accepts any scanned alphanumeric LPN without validating whether it matches expected inbound patterns. As a result, associates may unintentionally scan the wrong pallet, especially during peak receiving periods. These mis-scans are often detected only after inventory has been confirmed, leading to rework, delayed putaway, and inventory integrity issues.
________________________________________
Constraints
•	No replacement or migration of the existing WMS
•	No system downtime or data migration
•	Minimal impact to associate workflows
•	No changes to staffing, schedules, or throughput targets
•	Solution must be configurable and limited in scope
________________________________________
Solution Overview
This project proposes a lightweight WMS enhancement that validates scanned LPN prefixes against expected inbound syntax patterns. When an LPN fails validation, the system prompts the associate to re-scan for confirmation. If the scans do not match, the transaction is canceled to prevent incorrect inventory confirmation.
The enhancement activates only on exception scenarios. For valid scans, the standard receiving (“happy path”) workflow remains unchanged.
________________________________________
Artifacts Included
•	Current-State Process Map — inbound receiving workflow before enhancement
•	Future-State Process Map — workflow with LPN validation and re-scan logic
•	Problem Statement & Background
•	Root Cause Analysis
•	Business Requirements
•	Functional Requirements
•	Acceptance Criteria
•	Change Impact Summary
•	KPI & Expected Impact Analysis
All artifacts are documented using WMS-agnostic terminology and standard BA practices.
________________________________________
Metrics Intended
•	Receiving accuracy percentage
•	Mis-scan incident count
•	Rework and correction hours
•	Training time required for new associates
•	Exception frequency by associate or shift
These metrics are intended to measure both immediate error reduction and long-term behavioral reinforcement.
________________________________________
Tools
•	Process Mapping: diagrams.net (draw.io)
•	Documentation: Google Docs / Microsoft Word
•	Analysis Frameworks: BABOK v3 concepts (process analysis, requirements analysis)
•	System Design: WMS-agnostic logic and pseudocode
No proprietary tools or systems are required to understand or apply the proposed solution.
________________________________________
Notes
This project is a fictionalized case study based on common warehouse operations and does not reference any specific company, dataset, or proprietary system. It is intended to demonstrate Business Analyst thinking, documentation, and solution framing.

