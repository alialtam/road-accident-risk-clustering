# Road Accident Risk Clustering 

## Overview
This project analyzes real-world road accident data to identify **high-risk conditions** using clustering techniques.

Instead of predicting accidents directly, the goal is to **discover hidden patterns** in accident scenarios based on environmental and road-related factors.

---

## Objective
- Group accidents based on similar conditions
- Identify high-risk scenarios
- Provide insights for safer road planning

---

## Dataset
- UK Road Safety Dataset
- File: `Accident_Information.csv`

### Features Used:
- Weather Conditions  
- Road Surface  
- Road Type  
- Speed Limit  
- Light Conditions  
- Urban / Rural Area  
- Time (Hour extracted)

---

## Data Preprocessing
- Removed missing & invalid values
- Feature engineering (Hour extraction)
- One-Hot Encoding for categorical variables
- Feature scaling using StandardScaler

---

## Algorithm Used
### K-Means Clustering
- Groups similar accident conditions
- Simple and effective for structured data

### Choosing K
- Used **Elbow Method**
- Optimal clusters: **K = 3**

---

## Methodology
1. Data loading & exploration  
2. Data cleaning & preprocessing  
3. Feature engineering  
4. Encoding & scaling  
5. K-Means clustering  
6. PCA for visualization  
7. Cluster interpretation  

---

## Results & Insights

### Cluster 0 — High Risk (Adverse Conditions)
- Rainy weather & wet roads  
- Higher fatality rate (~2.05%)  
- Mostly environmental risk  

---

### Cluster 1 — Low Risk (Normal Conditions)
- Daylight, dry roads  
- Mostly urban  
- Lowest fatality rate (~1.08%)  

---

### Cluster 2 — Medium Risk (Low Visibility)
- Night-time / darkness  
- Reduced visibility  
- Higher serious injuries (~15.38%)  

---

## Key Insight
> Accident frequency ≠ Accident risk

- Most accidents occur in normal conditions (due to traffic volume)
- BUT highest **risk per accident** occurs in:
  - Bad weather
  - Low visibility conditions

---

## Visualization
- Raw feature clustering plots  
- PCA-based 2D visualization  

---

## What Makes This Project Strong
- Real-world dataset
- Proper preprocessing pipeline
- Clear clustering interpretation
- Focus on **insights, not just model**

