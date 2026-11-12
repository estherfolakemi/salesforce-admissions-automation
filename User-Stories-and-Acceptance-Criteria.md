# User Stories and Acceptance Criteria

## Project: Salesforce Admissions & Student Performance Automation

**Role:** Business Analyst  
**Platform:** Salesforce CRM  
**Document Type:** Illustrative Portfolio Examples

---

### User Story 1: Automated Admissions Routing

**Story ID:** US-001

**As an** Admissions Officer,  
**I want** submitted application forms to be automatically routed to the appropriate team,  
**So that** applications can be processed efficiently without manual reassignment.

**Acceptance Criteria**

**Scenario 1: Successful Routing**

- **Given** a valid admissions form has been submitted,
- **When** Salesforce processes the form,
- **Then** the application should be assigned to the appropriate team according to configured routing rules.

**Scenario 2: Missing Routing Information**

- **Given** an application does not contain sufficient information to determine the correct team,
- **When** the routing process runs,
- **Then** the application should be flagged for manual review.

*Scenario 2 is an illustrative exception-handling requirement, not a confirmed feature of the deployed solution.*

---

### User Story 2: Student Performance Monitoring

**Story ID:** US-002

**As a** Teacher,  
**I want** Salesforce to compare a student's current and previous grades,  
**So that** I can identify significant academic performance declines.

**Acceptance Criteria**

**Scenario 1: Performance Decline**

- **Given** a student has previous and current grade records,
- **When** the system calculates the percentage decline,
- **Then** a decline of 25% or more should be flagged.

**Scenario 2: Performance Within Threshold**

- **Given** a student has previous and current grade records,
- **When** the calculated decline is below 25%,
- **Then** the student should not be flagged under this rule.

**Scenario 3: Missing Previous Grade**

- **Given** a student does not have a previous grade,
- **When** the comparison is attempted,
- **Then** the record should be excluded from the comparison and identified for review.

*Scenario 3 is a proposed testable requirement and should not be presented as implemented unless verified.*

---

### User Story 3: Academic Performance Dashboard

**Story ID:** US-003

**As a** Department Director,  
**I want** to view student performance information in Salesforce dashboards,  
**So that** I can monitor academic trends and identify students who may require support.

**Acceptance Criteria**

- **Given** relevant student performance data is available,
- **When** an authorised user opens the dashboard,
- **Then** the dashboard should display the configured performance metrics.
- **And** the information should reflect the underlying Salesforce reports.

---

### Requirements Traceability

| User Story | Business Requirement | Feature |
|---|---|---|
| US-001 | BR-001 | Admissions routing |
| US-002 | BR-002, BR-003 | Grade comparison and flagging |
| US-003 | BR-004 | Reporting and dashboards |

---

**Portfolio Note:** These are anonymised, illustrative business analysis artefacts created to demonstrate requirements documentation and acceptance criteria. They are not original client records.
