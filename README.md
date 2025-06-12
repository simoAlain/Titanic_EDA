# Titanic_EDA
Exploratory Data Analysis of Titanic Dataset

# Exploratory Data Analysis (EDA) of the Titanic Dataset

![Titanic](https://storage.googleapis.com/kaggle-datasets-images/3376/5276/2578a9a3c1b93f5e8b1c4d4e8d7a1d98/dataset-card.jpg)

## 📌 Project Overview
This project conducts an in-depth Exploratory Data Analysis (EDA) of the [Kaggle Titanic dataset](https://www.kaggle.com/c/titanic), investigating factors influencing passenger survival. The analysis combines statistical summaries, visualizations, and feature engineering to uncover key patterns.

## 🔍 Key Questions Explored
1. **Demographics**: How did age, gender, and passenger class affect survival?
2. **Family Ties**: Did traveling with family (SibSp/Parch) improve survival odds?
3. **Economic Factors**: How did fare prices and cabin classes correlate with survival?
4. **Missing Data**: Which features required imputation or engineering?

## 🛠️ Tools Used
- **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn
- **Visualizations**: Histograms, Boxplots, Heatmaps, Survival Rate Bar Charts
- **Data Processing**: Feature engineering (e.g., Title extraction from names, Age binning)

## 📈 Key Findings
### 1. Survival Rates by Feature
| Feature          | Survival Rate (%) | Insight                          |
|------------------|------------------|----------------------------------|
| Female           | 74.2             | "Women and children first" policy confirmed |
| 1st Class        | 62.9             | Higher-class passengers had priority access to lifeboats |
| Age < 10         | 59.0             | Children were prioritized        |
| Embarked (Cherbourg)| 55.4         | Possible boarding order effect   |

### 2. Missing Data Handling
- **Age**: 20% missing → Imputed with median values per passenger class
- **Cabin**: 77% missing → Engineered into "Deck" (first letter) and "Has_Cabin" binary
- **Embarked**: 0.2% missing → Filled with mode (Southampton)

### 3. Feature Correlations
![Correlation Heatmap](https://i.imgur.com/XYZheatmap.png)  
*Strongest correlations: Fare ↔ Pclass (-0.55), Survived ↔ Fare (0.26)*

## 📂 Repository Structure
