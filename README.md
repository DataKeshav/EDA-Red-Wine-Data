# 🍷 Red Wine Quality EDA

## 📌 Project Overview  
This project analyzes the **Red Wine Quality dataset** from the UCI Machine Learning Repository, containing **1,599 wine samples** with **11 physicochemical features** and a quality score. Using **Python (Pandas, Seaborn, Matplotlib)**, I performed a full **Exploratory Data Analysis (EDA)** pipeline to uncover chemical drivers of wine quality and deliver actionable insights for producers and analysts.

---

## 🛠️ Tools & Libraries  
- **Python**: Pandas, NumPy  
- **Visualization**: Matplotlib, Seaborn  
- **Analysis**: Correlation, PCA, Boxplots, Violin plots  
- **Environment**: Jupyter Notebook (VS Code)

---

## 🔍 Steps Performed  
1. **Data Cleaning**  
   - Verified integrity of **1,599 rows × 12 columns**  
   - Removed duplicates and standardized column names  

2. **Univariate Analysis**  
   - Analyzed distributions of alcohol, pH, residual sugar, citric acid  
   - Detected **>50 outliers** in residual sugar and sulphates  

3. **Bivariate Analysis**  
   - Compared alcohol vs. quality, density vs. alcohol, citric acid vs. pH  
   - Found **alcohol content increases by ~1.2%** from quality score 5 to 8  

4. **Multivariate Analysis**  
   - Correlation heatmap revealed **alcohol (r = +0.48)** and **volatile acidity (r = –0.39)** as top predictors  
   - PCA reduced dimensionality from 11 to 2 components, explaining **~63% variance**  
   - Pair plots visualized feature interactions across **6 quality levels**

---

## 📊 Key Insights  
- Wines rated **7–8** had **~11.5% alcohol**, compared to **~9.5%** for lower-quality wines  
- **Sulphates** showed a positive correlation (r = +0.25) with quality  
- **Volatile acidity** negatively impacted quality (r = –0.39)  
- Majority of wines (87%) rated between **5 and 6**, confirming class imbalance  
- **Residual sugar and citric acid** had weak predictive power (r < ±0.1)

---

## 📈 Sample Visuals  
  
- ![Alcohol vs Quality]()  
- ![Correlation Heatmap](images/correlation_heatmap.png)  
- ![PCA Scatter Plot](images/pca_scatter.png)

---

## 🎯 Business Impact Framing  
This analysis provides **data-driven recommendations** for wine producers:
- Target **alcohol levels above 10.5%** and **sulphates above 0.6 g/dm³** to improve quality ratings  
- Monitor and reduce **volatile acidity below 0.4 g/dm³** to avoid poor ratings  
- Use PCA and correlation insights to guide feature selection for predictive modeling

---

## 📎 Dataset  
- Source: [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- Samples: 1,599 red wines  
- Features: 11 physicochemical + 1 quality score (0–10 scale)

---

## 🚀 Next Steps  
- Build a **classification model** to predict wine quality (e.g., Random Forest, XGBoost)  
- Create an interactive **dashboard** for non-technical stakeholders  
- Compare with **White Wine dataset** to generalize findings

---

