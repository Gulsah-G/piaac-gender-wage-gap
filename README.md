# Another Look at U.S. Gender-Based Wage Disparities: Insights from PIAAC

This repository contains the replication code and data analysis for the white paper:  
**"Another Look at U.S. Gender-Based Wage Disparities: Insights from PIAAC"** *Authors: Henry Braun & Gulsah Gurkan* *Published by: ETS Research Institute (2024)*

[**Read the Full White Paper Here**](https://www.ets.org/s/research/pdf/another-look-us-gender-based-wage-disparities-insights-piaac.pdf)

---

## 📌 Project Overview
While the gender wage gap is often discussed in terms of educational attainment and years of experience, this study leverages the **OECD’s Programme for the International Assessment of Adult Competencies (PIAAC)** to introduce a critical third variable: **measured cognitive skills** (literacy and numeracy). 

By analyzing prime-age workers (25–54), this research examines how these skills impact the probability of being a "top earner" and highlights persistent disparities that remain even when accounting for high cognitive proficiency.

### Key Research Findings:
* **The "Skill" Factor:** Cognitive skills are strong predictors of income, but they do not eliminate the gender gap.
* **Distributional Disparity:** Even among men and women with identical literacy and numeracy scores, men are significantly more likely to be in the top income quartile.
* **Human Capital:** The analysis challenges traditional human capital models by showing that the "return on skills" is not applied equally across genders.


---

## 📊 Data Source
The analysis is based on the **PIAAC Public Use File (PUF)** for the United States in all three PIAAC rounds combined. 
* **Variables:** Focuses on household income, educational attainment, work experience, and objective skill measures (literacy and numeracy).
* **Access:** Data can be downloaded via the [OECD PIAAC Gateway](https://www.oecd.org/en/about/programmes/piaac/piaac-data.html).

---

## 💻 Methodology
The analysis was conducted using **R**, focusing on complex survey data structures. The workflow includes:
1.  **Data Preprocessing:** Filtering for prime-age workers and handling missing values in household income using survey weights.
2.  **Descriptive Statistics:** Generating weighted means and distributions for literacy/numeracy scores across genders.
3.  **Regression Modeling:** Logistic regression models calculating the odds of being a "top earner" (top 25%) based on skill levels, education, and demographic variables.
4.  **Visualization:** Using `ggplot2` to visualize the shifts in wage distributions when controlling for cognitive proficiency.