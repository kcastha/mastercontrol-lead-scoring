
# MasterControl Lead Scoring

## Interactive Dashboard

View the full dashboard here:

[Open MasterControl Lead Scoring Dashboard](https://kcastha.github.io/mastercontrol-lead-scoring/dashboard.html)

## Project Overview

Built a machine learning–driven lead scoring system to help MasterControl improve conversion rates for its underperforming Manufacturing (Mx) product line.

The goal was to **identify high-value leads and prioritize sales outreach**, enabling Sales Development Representatives (SDRs) to focus on prospects most likely to convert.

**Key Result:** Developed a predictive ranking model that identifies high-conversion leads, enabling more efficient SDR targeting and improved pipeline quality.

---

## Business Problem

MasterControl provides quality and manufacturing software to life sciences companies. While the Quality (Qx) product converts well (19.7%), the Manufacturing (Mx) product significantly underperforms (12.7%).

This creates two key risks:

* Targeting low-quality leads → wasted SDR effort and missed opportunities
* Missing high-value leads → lost revenue and pipeline inefficiency

SDRs have limited capacity and currently lack a **data-driven prioritization system**.

**Target Variable:**
Binary classification

* 1 = Lead progresses to SQL/SQO/Won
* 0 = Lead does not progress

**Challenge:**
Build a model that ranks leads by conversion likelihood and improves sales prioritization.

---

## Data Preparation

* Dataset: ~16,000+ leads across multiple attributes (account, title, channel, priority)
* Feature Engineering:

  * Processed categorical-heavy CRM data
  * Extracted insights from job titles (seniority, function)
  * Captured lead intent signals (priority levels, channels)
* Data Challenges:

  * High cardinality (thousands of job titles)
  * Missing values in title field
  * Imbalanced conversion rate (~18% positive)

---

## Models Developed

### Logistic Regression

* Baseline model for interpretability
* Result: Limited ability to capture complex relationships

---

### Tree-Based Models

* Random Forest
* Gradient Boosting
* XGBoost / LightGBM / CatBoost

**Result:** Stronger performance due to handling of categorical and nonlinear patterns

---

### Ensemble Models

* Stacking & Voting classifiers

**Result:** Improved overall predictive performance and robustness

---

## Why Tree-Based Models?

* Handle categorical-heavy data effectively
* Capture nonlinear relationships
* Provide feature importance insights
* Balance performance and interpretability

---

## Results and Business Impact

### Model Performance

* Successfully ranked leads by likelihood of conversion
* Improved identification of high-probability prospects

### What This Means for MasterControl

**Before Model:**

* SDRs contact leads without prioritization
* High-value leads may be missed

**With Model:**

* Focus outreach on top-ranked leads
* Increase conversion efficiency
* Reduce wasted effort on low-quality prospects

---

## Key Technical Decisions

### 1. Focused on Ranking, Not Just Accuracy

The goal was not just prediction, but **prioritization**.

**Key Insight:**
A good model should answer: *Who should we contact first?*

---

### 2. Feature Engineering Was Critical

* Transformed raw CRM data into meaningful signals
* Extracted value from unstructured job titles

**Key Insight:**
Better features mattered more than model complexity

---

### 3. Ensemble Models Improved Stability

Combining models helped capture different patterns in the data.

**Key Insight:**
No single model dominates — ensembles improve robustness

---

### 4. Explainability Was Essential

Used SHAP analysis to explain predictions.

**Key Insight:**
Business users need to trust and understand the model

---

## What I Would Do Differently

Given more time, I would:

* Use external data sources (e.g., ZoomInfo) for enrichment
* Improve NLP processing for job titles
* Optimize model thresholds using profit-based metrics
* Deploy model into a real-time CRM system

---

## Technical Skills Demonstrated

* Machine Learning: Logistic Regression, Random Forest, Gradient Boosting, Ensembles
* Model Evaluation: AUC-ROC, Precision, Recall
* Feature Engineering: Categorical encoding, NLP for text fields
* Explainability: SHAP analysis
* Data Processing: Pandas, Scikit-learn

---

## Business Impact Summary

* Enabled data-driven lead prioritization
* Improved sales efficiency and targeting
* Increased potential conversion rates
* Bridged gap between analytics and business decision-making

---

## Approach Walkthrough

Started with business understanding the Mx product’s low conversion rate.

Built baseline models, then advanced to tree-based and ensemble methods. Focused heavily on feature engineering and ranking performance. Evaluated models not just on accuracy, but on their ability to **prioritize high-value leads for SDRs**.

---

## Contact

Astha KC

📧 [asthakc.us@gmail.com](mailto:asthakc.us@gmail.com)
💼 LinkedIn

Open to opportunities in Data Analytics, Business Analytics, Data Science, and ML roles

---

## Acknowledgments

This project was completed as part of the MSBA Capstone 2026 Spring Program at the University of Utah.

Special thanks to **Professor Jeff Webb** and **Professor David Agogo** for their guidance, mentorship, and support throughout the project.

We also thank the **MasterControl team**, especially **Eric Bowen**, for providing the business context, data, and valuable feedback that made this project practical and impactful.

The repository includes modeling, analysis, and business insights developed for the MasterControl lead scoring project.

---

## Last Updated

April 2026
