# University Admissions: Outreach & Enrollment Funnel Analysis

**Client:** Illinois Institute of Technology (IIT) — Academic Recruitment
**Complete Documentation:** [Read the Full Strategic Report (PDF)](https://github.com/butterboypy/university-admissions-outreach-enrollment-analysis/blob/main/University%20Admission%20Analysis%20Report.pdf)

## 1. Project Overview

### Business Problem

IIT ran a global recruitment campaign — 15,000+ applicants outreached and 33,000+ calls placed by BPO agents to enroll 100+ students (2023–2024). Leadership needed to know whether scaling outreach volume was actually driving enrollment, or just driving cost.

- **Primary Research Question:** Is raw outreach volume converting into enrollments, and which markets, campaigns, and agents are actually driving ROI?

### Interactive Dashboard Demonstration

![Dashboard Demo](4.%20assets/Dashboard.gif)

**Interactive Live Dashboard:** [Explore the Live Fabric Dashboard](https://app.fabric.microsoft.com/view?r=eyJrIjoiMDM0MzUzNTgtZWQ5Ni00Y2VlLWIyOGItZTVhNzNjYjhiNjZkIiwidCI6IjUzYTg5ZjhiLTY2ZmItNDkzOC05NzM5LTZkMjg4MjIwNWUyMyJ9)

---

## 2. Key Findings & Insights

### Outreach & Enrollment Dynamics — The "Volume Paradox"

![Pre vs Post Admission](assets/01_pre_post_admission.png)

- **Diminishing Returns:** Outreach surged to 22,700+ post-admission attempts in 2024, but enrollment failed to scale proportionally. Enrollment was driven by high-intent unique applicants and targeted follow-ups, not raw call volume.
- **Funnel Stage:** Pre-admission outreach converts far more efficiently than post-admission chasing, which is largely stalled by external blockers (visa delays, competing offers, unresolved technical queries).

### Strategic Market Performance — Concentration Risk

![Outreach Volume per Country](assets/07_outreach_volume_per_country.png)

- **The "Big Three":** India, Ghana, and Nigeria drive 70%+ of all outreach — but India's high volume (88 enrollments) comes at a weak 0.53% Call Efficiency and 1.19% Lead Conversion.
- **The Efficiency Leaders:** South Korea (6.25% Lead Conversion) and Turkey outperform on a per-call basis despite minimal outreach investment — signaling an underfunded high-yield segment.

### Campaign Lifecycle Evaluation — ROI

![Campaign Volume vs Performance Ratios](assets/10_campaign_roe.png)

- **Zero-Yield at Scale:** FA24IP, FA24SIC, and SP25IP together consume 57% of total call volume but produced **0% enrollment**.
- **Best-in-Class:** AND23 hit a 10.17% conversion rate and 8.22% Call Efficiency on just 73 calls — the most under-resourced campaign in the portfolio.

### Agent Efficacy & Talent Optimization

![Escalation vs Enrollment](assets/13_escalation_vs_enrollment.png)

- **Volume ≠ Efficiency:** Rudra drove the most enrollments (42) off 11,546 calls (~0.7% closing power). Jyoti matched close to half that output (21 enrollments) using a third of the call volume, with the lowest escalation rate on the team (<1%).
- **Operational Leakage:** 8,000+ calls across top agents were logged with "No Remarks," representing a major CRM data-integrity gap and lost business intelligence.

---

## 3. Strategic Business Recommendations

- **Synchronize Outreach Timing:** Mandate a 10 AM–7 PM prime-time calling window and shift from single-month peaks to a year-round diversified outreach cycle.
- **Shift Budget to High-Yield Markets:** Reallocate spend away from flatlined, high-effort markets (Iran, Pakistan) toward South Korea and Turkey, and diversify into developed markets (USA, Spain) to de-risk over-reliance on India.
- **Audit & Cap Campaigns:** Stop resource drain by capping underperforming campaigns (DNA24, FA24DNA) and auditing FA24IP, FA24SIC and SP25IP (57% of spend, 0% yield), while scaling high-ROE blueprints like AND23. 
- **Move from Volume to Quality Coaching:** Transition high-volume, low-efficiency callers toward callers like Jyoti, Palak & Isha (lower call load, higher closing power, lower escalation) and route high-intent leads to top closers.
- **Enforce CRM Integrity:** Implement a strict "No Remark, No Credit" policy to eliminate the 8,000+ documentation gap and recover lost business intelligence. 
- **Prioritize High-Yield Leads:** Shift focus to top-of-funnel new applicants and deploy a dedicated task force to clear "Conversion Blockers" like technical queries and visa delays. 
- **Isolate Enrollment Logging:** Migrate and maintain enrollment data in a dedicated section within CRM audit logs to 
ensure cleaner documentation and streamlined analysis. 
---

## 4. Methodology

1. **Data Cleaning & Standardization:** Corrected mismatched country names, invalid country/area codes, and missing country fields across the raw CRM export.
2. **Funnel Segmentation:** Split the dataset into Pre-Admission vs. Post-Admission cohorts to isolate where conversion actually happens in the lifecycle.
3. **Temporal Analysis:** Profiled monthly and hourly outreach vs. enrollment trends (2023 vs. 2024) to identify peak-performance windows and seasonal cycle shifts.
4. **Geographic & Campaign Auditing:** Calculated Lead Conversion Rate and Call Efficiency Rate by country and by campaign ID to separate high-volume markets/campaigns from high-yield ones.
5. **Agent Performance Auditing:** Built a Caller Outcome Matrix (calls vs. remark categories) and cross-referenced Escalation Rate against enrollment count to flag high performers vs. coaching candidates.

---

## 5. Skills Demonstrated

- **Data Cleaning & EDA:** Python (Pandas, NumPy, Matplotlib/Seaborn) — CRM data standardization, funnel segmentation, cohort analysis
- **Business Analytics:** Conversion funnel diagnostics, Lead Conversion Rate & Call Efficiency Rate modeling, Return on Recruitment Effort (RORE)
- **Dashboarding:** Microsoft Fabric/Power BI — interactive geographic, temporal, and agent-performance visualizations
- **Stakeholder Communication:** Translating raw CRM/call data into an executive-ready strategic roadmap

---

## 6. Repo Structure

```
├── assets/
│   ├── dashboard-demo.gif
│   └── chart visuals (referenced above)
├── datasets/
│   └── raw & cleaned CRM/outreach data
├── EDA/
│   └── exploratory analysis notebooks
├── scripts/
│   └── data cleaning & transformation scripts
├── dashboard/
│   └── Fabric/Power BI dashboard file
├── README.md
└── University Admission Analysis Report.pdf   # full strategic report
```
