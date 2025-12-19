Business Requirements (BR)

•	BR-01: The system shall validate LPN syntax before confirmation.

•	BR-02: The system shall prevent confirmation of invalid LPN scans.

•	BR-03: Supervisors shall have override capability when appropriate.
________________________________________
Functional Requirements (FR)

•	FR-01: System compares scan prefix to an approved list.

•	FR-02: If mismatch → trigger warning.

•	FR-03: System requires second scan.

•	FR-04: If mismatch on second scan → cancel transaction.
________________________________________
Acceptance Criteria (AC)

•	AC-01: Valid LPNs confirm successfully on first scan.

•	AC-02: Invalid prefixes trigger “mis-scan” warning.

•	AC-03: Two mismatched scans cause cancellation.
________________________________________
Risks / Trade-Offs

•	Slight increase in scan time on exception cases

•	Risk of false positives if prefix list is outdated

•	Supervisor overrides could be overused if not governed


