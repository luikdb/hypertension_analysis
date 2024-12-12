# **Biostatistical Analysis of Hypertension in Dahl Rat Models**
**by Lui Kirtan**

---

## **Overview**
This study explores the impact of dietary salt on blood pressure across different genetic strains, with a focus on uncovering underlying patterns. Data preprocessing involved visualizing and refining the dataset to remove potential outliers, setting the stage for a deeper analysis. Statistical methods were employed to examine the influence of salt intake and genetic factors on blood pressure, revealing intriguing insights into the complexity of salt-sensitive hypertension. **There is also a PDF attached for more detailed explanation.**

---

## **Dataset**

It is a time-series dataset of blood pressure measurements collected from different groups of rats subjected to various diets, including salt-sensitive low and high-salt diets, as well as salt-resistant low and high-salt diets.
[Blood Pressure in Salt-Sensitive Dahl Rats](https://physionet.org/content/bpssrat/1.0.0/) 
---

## **Data Processing & Visualization**
- **Box Plots**: Visualize blood pressure data across groups (SS & SSBN13, Low Salt & High Salt).
- **Outlier Removal**: Outliers were detected using the **Interquartile Range (IQR)** method and filtered out.

---

<!-- Aligning two images side by side with 50% width each -->
<div style="display: flex; justify-content: space-between;">
  <img src="https://github.com/user-attachments/assets/d9f470b9-e316-49b7-a909-cb7d685e25f6" alt="SSBN13-No-Outlier" style="width: 49%;"/>
  <img src="https://github.com/user-attachments/assets/af6c588b-9300-4942-a8fe-7f24f131f1a7" alt="SS-No-Outlier" style="width: 49%;"/>
</div>

*Figure 1: Side-by-side comparison of cleaned blood pressure data of salt resistive and salt sensitive rats*

---

## **Statistical Analysis**
### **Normality Test (Shapiro-Wilk)**
A normality test was conducted on the blood pressure data to ensure the assumptions for parametric tests were met. Results indicated that the data was normally distributed.

### **Welch's t-Test**
Used to compare mean blood pressure between different groups under low and high salt conditions.

#### Key Results:
- **High Salt**: SS rats showed a significant increase in blood pressure.
- **SSBN13 rats**: Showed a less pronounced increase in blood pressure in response to high salt.

### **ANOVA**
A **two-way ANOVA** was used to evaluate the effects of **Diet (Salt vs. No Salt)** and **Strain (SS vs. SSBN13)** on blood pressure.

### **Tukey HSD Post-hoc Analysis**
Identified significant differences in blood pressure between diet and strain combinations, confirming that dietary salt significantly influences blood pressure.

---

## **Conclusion**
The study reinforces the critical role of dietary salt in regulating blood pressure, with significant genetic variability in salt sensitivity. The findings highlight the complex interplay between genetic factors and environmental influences (like diet) in hypertension development.

---



---

## **Requirements**
- R 
- Libraries: 'ggplot', 'dplyr', 'tidyr', 'multcomp', 'knitr'

---
