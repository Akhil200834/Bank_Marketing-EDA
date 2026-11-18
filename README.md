# Bank_Marketing-EDA
Bleep Education-Mini project 2


**Author:** Korra Akhil (`2026mcb1536@iitrpr.ac.in`)  
**Dataset:** UCI Machine Learning Repository — Bank Marketing Dataset (`bank-additional-full.csv`, Dataset #222)[cite: 4, 5]  
**Program:** Bleep Education Data Science & Analytics Mentorship

---

## 1. Project Overview & Business Objective
Direct telemarketing campaigns are a primary customer acquisition channel for retail banks promoting long-term deposit subscriptions (`y`)[cite: 4]. However, untargeted outbound calling leads to high operational costs and customer fatigue. This project conducts a comprehensive 35-question Exploratory Data Analysis (EDA) across **41,188 customer contact records** and **20 input attributes** to uncover the demographic, financial, campaign contact, and macroeconomic factors driving term-deposit conversions[cite: 4, 5].

---

## 2. Repository Structure
```text
Bank_Marketing-EDA/
├── data/
│   └── bank-additional-full.csv      # 41,188 records x 21 attributes (semicolon-delimited)
├── notebooks/
│   └── bank_marketing_eda.ipynb      # Complete 35-question EDA (Sections A–F) + visual insights
├── outputs/
│   └── graphs/                       # High-resolution (300 DPI) exported visualizations
├── README.md                         # Project documentation & key business findings
└── requirements.txt                  # Python dependencies
```

## Analytical Framework (Sections A–F)
Section A (Q1–Q6) — Data Inspection & Preprocessing: Verified schema integrity (41,188 × 21), memory footprint, feature cardinality, exact duplicates, and evaluated 'unknown' categories as informative behavioral non-disclosures rather than standard nulls.   
Section B (Q7–Q12) — Customer Demographics & Segmentation: Analyzed customer age distributions, occupational composition, marital status, education levels, and top customer demographic profiles.   
Section C (Q13–Q17) — Financial Behaviour & Banking Relationships: Examined housing loan and personal loan cross-tabulations, conditional adoption probabilities, credit default combinations, and segment-level financial exposure.   
Section D (Q18–Q24) — Campaign Subscription Outcome Analysis: Evaluated severe target class imbalance (~88.7% non-subscribers vs. ~11.3% subscribers) and calculated true conversion rates across occupations, age brackets, loan statuses, and a filtered customer-segment conversion matrix.   
Section E (Q25–Q30) — Contact Strategy & Temporal Patterns: Compared cellular vs. telephone conversion effectiveness, diminishing returns from repeated campaign calls, call duration separation, monthly/weekday seasonality, and prior campaign outcomes (poutcome).   
Section F (Q31–Q35) — Macroeconomic Indicators & Statistical Testing: Evaluated Pearson correlations and multicollinearity among macroeconomic indicators (emp.var.rate, cons.price.idx, cons.conf.idx, euribor3m, nr.employed), analyzed conversion rates across interest-rate/employment regimes, and performed formal hypothesis testing (Chi-Square and Mann-Whitney U tests). 

## How to run Locally
1. Clone the repository
git clone [https://github.com/Akhil200834/Bank_Marketing-EDA.git](https://github.com/Akhil200834/Bank_Marketing-EDA.git)
cd Bank_Marketing-EDA
2. Install dependies
pip install -r requirements.txt
3. Execute the Jupyter Notebook:
Open notebooks/bank_marketing_eda.ipynb in VS Code or Jupyter Lab and click Run All to reproduce all statistical outputs and export high-resolution figures to outputs/graphs/.