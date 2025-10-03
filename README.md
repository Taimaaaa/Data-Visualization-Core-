# **Data Visualization Core – Insurance Dataset**

This project explores data visualization techniques in Python using the Insurance dataset.
The dataset contains information about age, sex, BMI, children, smoking status, region, and insurance charges.
The goal is to understand relationships between features and medical charges through visualizations.

## **Objectives**

1. Explore correlations between features and insurance charges.
2. Compare insurance charges across categories (e.g., smokers vs. non-smokers, males vs. females, regions).
3. Visualize relationships using barplots, boxplots, scatterplots, regression plots, and countplots.
4. Interpret findings and highlight key insights about factors affecting medical charges.

## **Workflow**
1. Dataset Overview

    * Rows: 1,338
    * Columns: 7 (age, sex, bmi, children, smoker, region, charges)
    * Target of interest: **charges**

2. Visualizations:
    * **Correlation Analysis**
      * Heatmap of correlations.
      * Key Insight: Smoking status shows the strongest correlation with charges.

    * **Charges vs. Smoking Status**
  
      * Barplot: Smokers pay ~4x higher charges than non-smokers.
      * Boxplot: Shows medians, spread, and outliers. Smokers have charges exceeding $60k+.

    * **Charges vs. Sex**
      * Barplot: Males have slightly higher mean charges (~$13.8k vs. $12.9k).
      * Grouped Barplot (Sex × Smoker): Smoker effect dominates — male smokers highest (~$33k).

    
    
    * **Age vs. Charges**
    
      * Scatterplot: Charges increase with age.
      
      * Colored by Smoker: Smokers always pay more at every age.
      
      * Colored by Sex: Overlap is heavy; sex has little explanatory power.
    
    
    * **BMI vs. Charges**
    
      * Regplot: Weak positive trend overall.
      
      * Colored by Smoker: Clear split into two bands.
      
      * LMPlot: Smokers show steep positive slope; non-smokers almost flat.
    
    * **Regional Analysis**
    
      * Countplot: Southeast has the highest count.
      
      * Barplot: Southeast has the highest average charges.
      
      * Smoker Ratio: Southeast has the highest smoker percentage (~25%).




## **Key Insights**

1. Smoking status is the strongest predictor of high charges.

    * Smokers consistently incur charges ~3–4x higher.
    * Effect is amplified with higher BMI and age.

2. Sex differences are minor compared to smoking.
    * Male smokers slightly higher than female smokers, but gap is small.

3. BMI has more impact among smokers than non-smokers.

    * Clear interaction between BMI and smoking.

4. Regional differences exist.

    * Southeast has both the highest charges and the highest smoker ratio.


## **Conclusion**

This project demonstrates how EDA (Exploratory Data Analysis) and visualizations reveal key drivers of insurance costs.
The findings strongly suggest that smoking status, followed by age and BMI, are the dominant factors influencing charges, while sex plays only a minor role.
