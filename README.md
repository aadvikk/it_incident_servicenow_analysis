# IT Incident & Service Desk Performance Analysis (ServiceNow Simulation)

## 📌 Project Overview
This project simulates **enterprise IT Service Management (ITSM) incident data** to analyze **SLA compliance, resolution efficiency, and operational performance**.  
The analysis mirrors how Business Analysts work with **ServiceNow incident data** to support IT leadership decisions.

The project is built entirely using **Python, SQL, and data visualization**, and is designed to reflect **real corporate workflows**.

---

## Business Objective
IT leadership wants to understand:
- Are incidents being resolved within SLA?
- Which priorities and categories cause the most delays?
- Which support teams are overloaded?
- Where operational improvements can reduce downtime?

This analysis provides **data-backed insights and recommendations** to improve IT service delivery.

---

## 🏢 Corporate Context (ServiceNow Alignment)
In large enterprises, IT incidents are managed using **ServiceNow ITSM**.  
This project simulates the **ServiceNow `incident` table** and reproduces common KPIs used in ServiceNow dashboards.

| Project Column | ServiceNow Equivalent |
|--------------|----------------------|
| incident_id | number |
| opened_date | opened_at |
| resolved_date | resolved_at |
| priority | priority |
| category | category |
| assigned_team | assignment_group |
| sla_hours | SLA definition |
| sla_breached | breach |

---

## Key Business KPIs Analyzed
- **SLA Compliance Rate**
- **SLA Breach Percentage**
- **Mean Time to Resolution (MTTR)**
- **Incident Volume Distribution**
- **Team-Level Performance**

---

## Tools & Technologies Used
- **Python** (pandas, numpy)
- **SQL** (SQLite – in-memory database)
- **Seaborn & Matplotlib** (business-focused visualizations)
- **Google Colab** (cloud-based execution, no installation)

---

## Dataset Description
The dataset is **synthetically generated** but follows **realistic enterprise distributions**.

| Field | Description |
|----|----|
| incident_id | Unique incident number |
| priority | P1–P4 based on business impact |
| category | Network, Application, Hardware, Security |
| assigned_team | IT support group |
| sla_hours | Target resolution time |
| actual_resolution_hours | Calculated resolution time |
| sla_breached | Yes / No |

---

## Analysis Performed
1. **SLA breach rate by priority**
2. **MTTR by incident category**
3. **Incident workload by support team**
4. **SQL-based reporting for validation**
5. **Executive-friendly visualizations**

---

## Sample Insights
- P1 incidents show the **highest SLA breach rate**, despite lower volume.
- Network-related incidents have the **longest resolution times**.
- App Support handles the **highest ticket volume**, indicating potential workload imbalance.

---

## Business Recommendations
- Introduce a **dedicated on-call rotation for P1 incidents**
- Improve **proactive network monitoring**
- Rebalance workloads across support teams to reduce burnout and delays
