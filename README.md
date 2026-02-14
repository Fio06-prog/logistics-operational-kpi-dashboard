# Logistics Operational KPI Dashboard  
Power BI | Business Analysis + Data Analytics


## Project Overview

This project analyzes operational logistics performance using a KPI-driven framework to identify service inefficiencies, delay drivers, and operational risk patterns.

The dashboard integrates business logic with data modeling best practices to provide executive-level visibility and analytical depth for operational decision-making.


## Business Context

In logistics operations, on-time performance and SLA compliance directly impact:

- Customer satisfaction  
- Contractual penalties  
- Operational cost efficiency  
- Carrier evaluation  
- Strategic capacity planning  

Delays and detention time generate measurable financial risk and service instability.  

A structured KPI framework is necessary to translate raw operational data into actionable performance intelligence.


## Business Problem Statement

The organization lacks a centralized analytical framework to:

- Monitor On-Time performance across regions
- Identify high-risk operational states
- Compare Delivery vs Pickup efficiency
- Understand delay root causes
- Evaluate SLA adherence vs target performance

Without a structured model, decision-making remains reactive rather than strategic.


## KPI Framework Definition

The following KPIs were selected based on operational relevance:

- **On-Time %** → Service reliability indicator  
- **SLA Compliance %** → Contract adherence measurement  
- **Delay Rate %** → Operational failure frequency  
- **Avg Delay (min)** → Severity of service deviation  
- **Avg Detention (min)** → Facility-level inefficiency indicator  
- **Target Variance (pp)** → Gap-to-goal measurement  

These metrics enable multi-layer analysis:

- Performance monitoring  
- Risk detection  
- Operational benchmarking  
- Strategic planning  


## Data Model Architecture

The model follows star-schema logic with a dedicated Date dimension.

Detailed modeling explanation available here:

 [Data Model Architecture](documentation/data-model-architecture.md)


## Dashboard Structure

### Page 1 – Executive Overview
- High-level KPI monitoring
- Monthly target comparison
- Performance trend vs SLA

### Page 2 – Event Type Performance
- Delivery vs Pickup comparison
- Operational delay segmentation
- Trend variance analysis

### Page 3 – Root Cause & Operational Risk
- Worst-performing regions
- State-level risk identification
- Delay vs On-Time relationship analysis


## Analytical Findings

Key insights extracted from the dashboard:

[Analytical Findings](documentation/analytical-findings.md)


## Business Implications

The analysis reveals:

- Significant regional performance variation  
- Higher average delay impact on On-Time % degradation  
- Operational imbalance between Delivery and Pickup processes  
- Risk concentration in specific states  

These patterns indicate structural operational inefficiencies rather than isolated events.


## Strategic Recommendations

1. Implement regional performance monitoring routines  
2. Introduce SLA risk alerts for underperforming states  
3. Optimize detention time through facility process audits  
4. Deploy KPI-based monthly operational reviews  
5. Establish variance-based escalation thresholds  

The framework supports scalable performance governance.


## Technical Stack

- Power BI Desktop
- DAX Measures
- Star-Schema Data Modeling
- Custom Date Dimension
- KPI-Based Analytical Design
- Conditional Formatting for Risk Segmentation


## Analytical Profile Positioning

This project reflects a hybrid profile:

- Business Analysis (problem framing, KPI selection, decision logic)
- Data Analytics (modeling, transformation, visualization, insight extraction)

Designed for operational performance environments within logistics and supply chain industries.

