# Travel Habits ML Project

---
<div align="center">
  <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExdWk5aHFxdWFmN2xnZWZ3MmZxZThwZmRhMGI3dndkNmdqbDY4YmtndyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/rLEiCb16Ffyqk/giphy.gif" alt="giphy">
</div>

## Overview
This project analyzes household travel survey data from Israel to predict the main mode of transportation for individuals. Using a variety of machine learning models and clustering techniques, the project uncovers valuable insights about travel behaviors and patterns. These insights can guide urban transportation planning and improve mobility solutions.

## Dataset
The dataset consists of survey data collected from households, detailing demographics, transportation modes, and trip characteristics.

* Household Details (hhs_1.csv): Demographic and socio-economic data.

* Individual Details (pps_1.csv): Information about age, gender, and employment.

* Activity Details (aas_1.csv): Trip purposes, modes of transportation, and other specifics.

* Vechiles Detailes (vvs.csv): Vechiles types and amounts, *not in use for current work.*

* Metadata (NTHS-meta.xlsx): Descriptions of dataset columns for clarity.
  
Key preprocessing steps included merging datasets, handling missing values, and selecting the most relevant features to improve model performance.

## Methods
### Supervised Learning
Six models were implemented:

**Random Forest:** Achieved the highest performances (84% accuracy).

**Neural Network:** Used for capturing complex patterns with the best architecture tailored for the dataset.

**Logistic Regression:** Established as a baseline model.

**XGBoost:** Provided high performance but had longer runtime.

**LightGBM:** Balanced efficiency and accuracy, ideal for large-scale applications.

**CatBoost:** Specialized in handling categorical data, reducing preprocessing needs.
### Unsupervised Learning
**DBSCAN:** Identified dense clusters, uncovering unique patterns such as long-distance travel among specific groups.

**K-Means:** Clustered data into seven groups, revealing distinct travel patterns for younger individuals.

## Results

- High Accuracy Modes: Walking and driving were predicted with high precision due to distinct features.
- Challenges: Public transport modes, such as buses and taxis, often overlapped, leading to misclassifications.
- Cluster Insights: DBSCAN and K-Means highlighted unique groups, such as long-distance travelers and younger commuters.

## Key Findings
Improving data quality and adding route-specific features could enhance predictions for overlapping transport modes.
Balancing the dataset to address underrepresented modes like motorcycles can improve model accuracy.
