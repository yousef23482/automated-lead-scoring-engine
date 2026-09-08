# Automated Lead Cleaning & Scoring Engine

A Python-powered data pipeline built with **Pandas** to sanitize messy lead inputs, normalize email domains, drop duplicates, and output a prioritized **Master Daily Call Sheet** for B2B sales teams.

---

## 🎯 Project Objective
Eliminate sales rep inefficiency by automating raw data cleaning and applying a rule-based scoring matrix to prioritize outbound calls based on buyer authority, company size, and domain quality.

---

## 🔑 Key Findings & Business Impact
* **Data Sanitization:** Processed 300 raw lead records, stripping white space, standardizing job title authority, normalizing domains, and eliminating 164 duplicate entries.
* **Domain Qualification:** Automatically penalized free webmail domains (`gmail.com`, `yahoo.com`) while prioritizing verified corporate email domains.
* **Actionable Tiering:** Classified 136 unique leads into 3 prioritized call tiers without discarding lower-tier leads:
  * **Priority A (Hot):** 39 Leads (Morning Peak Calling)
  * **Priority B (Warm):** 61 Leads (Mid-Day Outreach)
  * **Priority C (Cold):** 36 Leads (Batch Emailing / EOD Calling)

---

## 🛠️ Tech Stack & Methodology
* **Python (Pandas, NumPy):** Automated text parsing, domain extraction, and string normalization.
* **Custom Scoring Logic:** Implemented weighted scoring rules evaluating job titles, target industries, and company size.
* **CSV Export:** Outputted a ranked `master_daily_call_sheet.csv` sorted by `lead_score` descending.

---

## 🚀 How to Run

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/automated-lead-scoring-engine.git](https://github.com/YOUR_USERNAME/automated-lead-scoring-engine.git)
   cd automated-lead-scoring-engine
Install Dependencies:

Bash
pip install pandas numpy
Run the Engine:

Bash
python project2_lead_scoring.py
