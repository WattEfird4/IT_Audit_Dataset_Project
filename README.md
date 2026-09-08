# IT Audit Project: Incident Management Process Review

## Project Overview

This project analyzes the `incident_event_log.csv` dataset to evaluate the effectiveness of the organization's IT Incident Management process. The objective is to identify control weaknesses, operational inefficiencies, and compliance risks related to incident handling, escalation, resolution, and closure activities.

The analysis supports an IT audit by providing data-driven insights into how incidents are managed throughout their lifecycle and whether established IT service management (ITSM) controls are operating effectively.

---

## Audit Objectives

The primary objectives of this IT audit are to:

- Assess the effectiveness of incident management controls.
- Evaluate whether incidents are resolved within expected service levels.
- Identify excessive reassignment or reopening of incidents.
- Detect potential process bottlenecks and operational inefficiencies.
- Review the completeness and consistency of incident records.
- Support risk assessment and control testing through data analytics.
- Provide recommendations for improving incident response and governance.

---

## Dataset Description

### File

`incident_event_log.csv`

### Dataset Size

- Approximately **120,000 records**
- Represents multiple status changes and lifecycle events for IT incidents

### Purpose

The dataset captures event-level information for incident tickets, allowing auditors to trace incident activity from creation through resolution and closure.

Because each incident can have multiple status updates, the same incident number may appear multiple times throughout the dataset.

---

## Key Fields

| Field | Description |
|---------|-------------|
| number | Unique incident identifier |
| incident_state | Current incident status (New, Resolved, Closed, etc.) |
| active | Indicates whether the incident is active |
| reassignment_count | Number of times the ticket was reassigned |
| reopen_count | Number of times the incident was reopened |
| sys_mod_count | Number of record updates |
| made_sla | Indicates whether SLA requirements were met |
| caller_id | User reporting the incident |
| opened_by | User who created the incident |
| opened_at | Incident creation timestamp |
| contact_type | Method used to report the incident |
| location | User or incident location |
| category | Incident category |
| subcategory | Incident subcategory |
| impact | Business impact rating |
| urgency | Urgency rating |
| priority | Calculated incident priority |
| assignment_group | Support group assigned to resolve the incident |
| assigned_to | Individual resolver assigned |
| knowledge | Indicates whether a knowledge article was used |
| resolved_by | Resolver of the incident |
| resolved_at | Resolution timestamp |
| closed_at | Closure timestamp |

---

## Audit Risks Addressed

### Operational Risk

- Delayed incident resolution
- Excessive ticket handoffs
- Incomplete incident documentation

### Compliance Risk

- Failure to meet Service Level Agreements (SLAs)
- Inadequate evidence supporting incident closure

### Technology Risk

- Recurring incidents indicating unresolved root causes
- High-impact incidents not prioritized appropriately

### Governance Risk

- Lack of accountability for incident ownership
- Inadequate monitoring of support group performance

---

## Planned Audit Analytics

### 1. Incident Volume Analysis

Evaluate:

- Total incidents created
- Incident trends over time
- Volume by category and location

Example Questions:

- Which categories generate the highest number of incidents?
- Are there seasonal spikes in incident activity?

---

### 2. SLA Compliance Testing

Evaluate:

- Incidents meeting SLA requirements
- SLA breach rates by category
- SLA breach rates by support group

Example Questions:

- Which support groups have the highest SLA failure rates?
- Do high-priority incidents receive timely resolution?

---

### 3. Reassignment Analysis

Evaluate:

- Incidents with multiple reassignments
- Average reassignment count
- Groups with the highest ticket transfers

Audit Concern:

Excessive reassignment may indicate unclear ownership or inadequate triage controls.

---

### 4. Reopened Incident Analysis

Evaluate:

- Frequency of reopened tickets
- Root causes of ticket reopening
- Resolver performance

Audit Concern:

High reopen rates may indicate insufficient problem resolution.

---

### 5. Priority and Impact Assessment

Review relationships among:

- Impact
- Urgency
- Priority

Audit Concern:

Incorrect prioritization may lead to delays in handling critical incidents.

---

### 6. Incident Lifecycle Analysis

Calculate:

- Time to resolution
- Time to closure
- Aging incidents
- Average handling duration

Audit Concern:

Extended resolution times may indicate process inefficiencies.

---

### 7. Assignment Group Performance

Evaluate:

- Incident volume by support team
- Resolution efficiency
- SLA performance
- Reopen frequency

Audit Concern:

Poor-performing groups may require additional oversight or resources.

---

## Expected Deliverables

- Incident Management Audit Dashboard
- SLA Compliance Report
- Reassignment and Reopen Analysis
- Support Group Performance Metrics
- Risk and Control Assessment
- Audit Findings and Recommendations

---

## Recommended Tools

- Python (Pandas, NumPy)
- SQL
- Power BI
- Tableau
- Excel
- Jupyter Notebook

---

## Success Criteria

The project will be considered successful if it:

- Identifies measurable control weaknesses.
- Quantifies process inefficiencies.
- Highlights SLA compliance issues.
- Provides actionable recommendations.
- Supports evidence-based audit conclusions.

---

## Author

**IT Audit Analytics Project**

Focused on leveraging incident management data to assess operational effectiveness, control compliance, and risk exposure within the IT service management process.


This README is suitable for a GitHub portfolio project and aligns well with an IT Audit or CISA-related analytics project.
