# 📊 Star Digital A/B Testing Analysis

This project presents a causal inference analysis of an online display advertising campaign conducted by **Star Digital**, aiming to assess the effectiveness of digital ads on subscription purchases and website visits. The experiment used a randomized A/B test design across six websites and was analyzed using statistical models in R.

> 📁 Part of the coursework for **MSBA 6441 – Causal Inference**, Spring 2025

---

## 🧪 Experiment Overview

- **Company**: Star Digital (disguised name)
- **Objective**: Evaluate whether online display ads lead to more subscriptions
- **Design**:
  - **Test group**: Shown Star Digital ads
  - **Control group**: Shown unrelated charity ads
  - **Randomization**: Users assigned before any ads were served
- **Ad cost**: 
  - $25 per 1000 impressions on Sites 1–5
  - $20 per 1000 impressions on Site 6
- **Revenue**: $1,200 lifetime contribution per conversion

---

## 📈 Key Research Questions

1. **Ad Effectiveness**  
   Does showing Star Digital ads lead to a higher conversion rate compared to the control group?

2. **Frequency Effects**  
   How does the number of ad impressions relate to the likelihood of a user purchasing?

3. **Optimal Site Allocation**  
   Should Star Digital invest more in Site 6 or in the ad network (Sites 1–5) for better ROI?

---

## 🧠 Analysis Summary

### ✅ Effectiveness of Ads
- Conversion rate was slightly higher in the test group.
- **Chi-square test** and **logistic regression** showed weak but positive impact.
- P-values hovered around 0.06, indicating marginal significance.

### 📊 Frequency Effects
- Ads on **imp_2**, **imp_4**, and **imp_6** were positively associated with conversion.
- **Diminishing returns** observed—suggesting a need for frequency capping.

### 💡 ROI-Based Recommendation
- Calculated ROI per user for Sites 1–5 and Site 6.
- **Site 6 had higher average ROI** → Recommended to allocate more budget there.

---

## 🛠️ Tech Stack

- **Language**: R
- **Libraries**: `dplyr`, `ggplot2`, `glmnet`, `car`, `readxl`
- **Statistical Methods**: Chi-squared test, Logistic Regression, ROI analysis, VIF

---

## 📂 Files
```
star-digital-ab-test/
├── Assignment 2_Casual_Inference.Rmd # RMarkdown analysis script
├── Assignment-2_Casual_Inference.pdf # Final rendered report
├── M347-PDF-ENG.pdf # Star Digital case study document
└── README.md # Project overview (this file)
```

---

## 👥 Authors

- **Ujjwal Khanna**
- **Aurosikha Mohanty**

---

## 📚 Reference

- Case Study: *Star Digital: Assessing the Effectiveness of Display Advertising* (M347-PDF-ENG)
- MSBA 6441 – University of Minnesota, Spring 2025

---
