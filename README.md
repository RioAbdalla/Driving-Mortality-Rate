# Policy Evaluation and Public Health Analysis (FIN 550 Problem Set 2)

## 📌 Project Overview
This repository contains solutions and code for **Problem Set 2 of FIN 550: Big Data Analytics**. The project covers two major case studies:

1. **Medical Liability Reform in Texas (Bill 4, 2003)**  
   - Investigates whether capping malpractice damages affected the number of doctors practicing in Texas relative to neighboring states.  
   - Uses **Difference-in-Differences (DiD)** methodology to estimate causal impacts.  

2. **Teenage Driving and Mortality**  
   - Explores the relationship between teenage driving laws and mortality outcomes.  
   - Applies econometric and data science methods to evaluate policy effectiveness.  

---

## 📊 Methodology

### Medical Malpractice Reform Case
- **Approach**: Difference-in-Differences (DiD) comparing Texas (treatment group) with neighboring states (control group).  
- **Steps**:
  1. Compare pre-treatment trends (1998–2002) between Texas and neighbors.  
  2. Estimate changes in doctors per 100,000 residents from 2002–2006.  
  3. Adjust for possible spillover effects and confounders.  
- **Result**: Bill 4 is estimated to have **increased doctors per 100,000 by ~26** relative to neighboring states, though the parallel trends assumption appears weak.

### Teenage Driving and Mortality Case
- Uses regression analysis and policy evaluation techniques.  
- Explores causal impact of teenage driving restrictions on mortality rates.  
- Details provided in the **executive summary** and R script.

---

## 📈 Key Insights
- **Bill 4 Results**:  
  - Texas-only estimate suggests an increase of ~17 doctors (2002–2006).  
  - Cross-sectional comparison in 2006 suggests no clear effect relative to neighbors.  
  - DiD estimate indicates an increase of ~26 doctors, but assumptions may be violated.  

- **Teenage Driving Case**:  
  - Pending analysis results (see `Case-Executive-Summary.pdf`).  
  - Focused on estimating mortality reduction attributable to driving restrictions.  

---

## 🛠️ Tech Stack
- **R** (primary language)  
- Libraries: `tidyverse`, `dplyr`, `ggplot2`, `lmtest`, `sandwich`  

---

## 📂 Repository Structure
```
├── Problem Statement 2 (1).Rmd         # R Markdown with code and analysis
├── PS2-FIN550.docx                     # Problem set write-up with answers
├── Case-Executive-Summary.pdf          # Executive summary for Teenage Driving case
├── Case-Code.R                         # R script for Teenage Driving case
├── .gitattributes                      # Git configuration
└── README.md                           # Project documentation
```

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/fin550-problemset2.git
   cd fin550-problemset2
   ```
2. Open the R Markdown file:
   ```R
   rmarkdown::render("Problem Statement 2 (1).Rmd")
   ```
3. Run the analysis for the Teenage Driving case using:
   ```R
   source("Case-Code.R")
   ```

---

## 🤝 Contributors
- Damario Abdalla  
- Drew Levitt  
- Si Thu Aung  

---
