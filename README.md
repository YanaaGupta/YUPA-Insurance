# YUPA Insurance – Financial Risk Analytics & Scalable Student Health Insurance Model
> **By Yana Gupta**

This project investigates payout concentration risk and models the financial viability of a student health insurance product in Delhi. It includes a root cause analysis of fraud exposure (CityCare scam), a 3-year financial projection with subsidy structuring, and a phased GTM strategy with actuarial stress testing.
Here’s your **complete and detailed `README.md` file** for your GitHub repository: **`YUPA-Insurance-Financial-Risk-Analytics`**. It's structured to showcase the problem, methodology, findings, financial modeling, and strategic recommendations—perfectly aligned for a finance/consulting/analytics audience like J.P. Morgan or 180DC.

---

## Overview

This project investigates systemic flaws in an existing health insurance claims system and simultaneously explores the financial feasibility of launching a subsidized student health insurance product across Delhi NCR. It is divided into two critical tracks:

1. **Fraud Analytics in Health Insurance Claims**
2. **Designing a ₹386 Cr Revenue Student Insurance Model**

The project blends **actuarial projection**, **fraud risk analysis**, **data modeling**, and **strategic GTM planning**—a comprehensive financial research case study, similar to research conducted in Corporate & Investment Banking (CIB) firms.

---

## Problem Statement

**Claim Payouts were unusually high**, despite a stable insured population and average premium levels. A detailed audit revealed:

* **27% of payouts were linked to one hospital (CityCare) and one patient (P123)**.
* The same procedure (knee surgery) was repeated 7 times in unrealistic windows.
* Contracts lacked claim frequency limits and systemic flagging logic.

---

## Root Cause Analysis

Using pivot tables and cohort comparisons, the following systemic issues were diagnosed:

|  Issue                    |  Breakdown                                                           |
| ------------------------- | -------------------------------------------------------------------- |
| No Claim Limits           | Contracts allowed repeat procedures with no cooldown window.         |
| Duplicate Claim Loopholes | No deduplication engine for claims by patient-hospital pairs.        |
| Manual Audit Dependency   | No AI/ML validation for frequency, timing, cost spikes.              |
| Potential Fraud Collusion | Hospital and patient exploiting system via repeat high-value claims. |

---

## Student Insurance Market Feasibility

**Target:** Launch a high-coverage, low-risk insurance product for university students in Delhi (7L+ market).
**Pricing Strategy:** ₹7,000/year premium split 50-25-25 among Govt, University, Student.

### 3-Year Financial Projection (Baseline 60% Claim Ratio):

| Year | Students | Revenue (₹ Cr) | Claims (₹ Cr) | Admin (₹ Cr) | Net Profit (₹ Cr) |
| ---- | -------- | -------------- | ------------- | ------------ | ----------------- |
| Y1   | 7,00,000 | ₹490.00        | ₹294.00       | ₹73.50       | ₹122.50           |
| Y2   | 7,35,000 | ₹514.50        | ₹308.70       | ₹77.18       | ₹128.62           |
| Y3   | 7,71,750 | ₹540.23        | ₹324.14       | ₹81.03       | ₹135.06           |

*Profit holds even at 70% claim ratio, ensuring low actuarial risk and predictable revenue.*

---

## Risk Mitigation Strategy

**Short-term Operational Controls**

* Set 12-month cooldowns on high-value repeat procedures.
* Block claims with same CPT code from same patient-hospital pairs in <30-day windows.
* Mandatory second-opinion audits before approval.

**Medium-term Tech Stack**

* ML-based Red Flag Engine for:

  * Time-based clustering
  * Repetition pattern mining
  * Diagnosis-to-cost mismatches
* TPA Dashboard for real-time alerts and month-end compliance reporting.

---

## GTM Strategy – Student Insurance Product

**Year-wise Expansion Roadmap**

* **Y1**: Partner with Delhi Govt. + 50 universities
* **Y2**: Expand to Mumbai, Pune, Bangalore
* **Y3**: Launch in Tier-2 cities via regional university clusters

**Implementation**

* Digital onboarding via existing student portals
* Unified Health ID system for tracking policy usage

---

## Key Takeaways

* **Fraud costs can be systemic—not isolated.** Claim protocols need both actuarial and ML auditing layers.
* **Student insurance is highly profitable** if managed under a public-private split model with controlled claim ratios.
* **Data-backed recommendations enabled strategic decisions** around risk, pricing, and expansion.

---

## Tools & Techniques Used

| Category           | Stack Used                                                         |
| ------------------ | ------------------------------------------------------------------ |
| Financial Modeling | Excel (Pivot Tables, Scenario Modeling, Sensitivity Analysis)      |
| Risk Analysis      | Actuarial Forecasting, Ratio Stress Testing, Cohort Analysis       |
| Fraud Detection    | Time-based Claim Pattern Analysis, Hospital-Code Frequency Mapping |
| Strategic Planning | GTM Rollout, Cost Allocation, Public Subsidy Modeling              |

---

## Future Scope

> Build a working Python-based claims flagging system with adjustable parameters for frequency, amount, and procedure code combinations (WIP in `/scripts`).
> This model can be scaled to other emerging markets with:

* High student density
* Low insurance penetration
* Government interest in subsidized healthcare

---
