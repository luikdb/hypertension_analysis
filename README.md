# **Biostatistical Analysis of Hypertension in Dahl Rat Models**
**By: Lui Kirtan Deori Bharali**

---

## **Overview**
This project explores **salt-sensitive hypertension (SS-HT)** using **Dahl-SS** and **SSBN13** rat models to understand how dietary salt impacts blood pressure and how genetic variations influence salt sensitivity. The goal is to gain insights into the multifactorial nature of SS-HT, focusing on both **renal** and **extrarenal** factors.

---

## **Data Processing & Visualization**
- **Box Plots**: Visualize blood pressure data across groups (SS & SSBN13, Low Salt & High Salt).
- **Outlier Removal**: Outliers were detected using the **Interquartile Range (IQR)** method and filtered out.

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

## **Dataset**
Access the dataset used in this study:
[Blood Pressure in Salt-Sensitive Dahl Rats](https://physionet.org/content/bpssrat/1.0.0/)

---

## **Requirements**
- R 
- Libraries: 'ggplot', 'dplyr', 'tidyr', 'multcomp', 'knitr'

---

## **Getting Started**
Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/Biostatistical-Analysis-of-Hypertension.git
cd Biostatistical-Analysis-of-Hypertension
pip install -r requirements.txt
