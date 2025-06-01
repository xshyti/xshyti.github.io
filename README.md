# 🎓 Xhoi Shyti | Data Science Portfolio

Welcome to my data science portfolio. This repository showcases a collection of projects developed throughout my graduate studies and professional work. Each project combines statistical rigor, programming skills, and domain expertise to solve real-world problems using data.

---

## 📌 Featured Projects

### ⚾ 1. Predicting Home Run Probability Using Statcast Data
**Status:** ✅ Completed  
**Overview:**  
This project uses MLB Statcast data from the 2023 and 2024 seasons to develop a logistic regression model predicting whether a batted ball will result in a home run. The model incorporates features such as launch speed, launch angle, and a custom park-adjustment factor (`extra_distance_2025`) to account for environmental influences.

**Highlights:**  
- Used pybaseball to collect a 10,000-row sample of batted ball data  
- Created a binary classification target (`is_home_run`)  
- Key predictors: launch speed, launch angle, and hit distance  
- Achieved 96.8% accuracy and ROC-AUC of 0.95  
- Accounted for park-specific variance using `extra_distance_2025`  
- EDA included histograms and scatter plots revealing the home run "sweet spot"

**Key Components:**  
- Business Problem, Background, Data Explanation  
- Exploratory Data Analysis and Visualizations  
- Logistic Regression Modeling  
- ROC/AUC Analysis and Interpretability  
- Limitations (rare-event imbalance) and Recommendations for ensemble methods  
- Ethical Assessment (e.g., avoiding misuse in scouting)  

**Links:**  
📂 [GitHub Repo](project_statcast_predictors) | 📄 [Whitepaper](project_nba_game_metrics/report) | 📊 [Slide Deck](project_nba_game_metrics/presentation/key_metrics_pres.pptx)

---

### 💼 2. Predicting Income Levels from Demographic and Employment Data
**Status:** ✅ Completed  
**Overview:**  
Using the UCI Adult Income dataset (Census 1994), this project applies machine learning to classify whether an individual earns above or below $50K per year. Both logistic regression and random forest classifiers were used, with the latter achieving superior performance.

**Highlights:**  
- Dataset included 32,561 records and 15 demographic/employment variables  
- Key predictors: education level, capital gains, hours worked, age, and marital status  
- Logistic Regression: 78.6% accuracy | Random Forest: 85.8% accuracy  
- Feature engineering, label encoding, and data normalization conducted  
- Visualized relationships between features and income class (e.g., boxplots, barplots)  

**Key Components:**  
- Business Problem and Historical Context  
- Data Preparation and Feature Encoding  
- Model Training and Evaluation (Precision, Recall, ROC-AUC)  
- Discussion on Class Imbalance and Feature Importance  
- Future Applications in policy, education, and labor economics  
- Ethical Considerations regarding bias in demographic-based predictions  

**Links:**  
📂 [GitHub Repo](project_income_level_data) | 📄 [Whitepaper](project_income_level_data/report) | 📊 [Slide Deck](project_income_level_data/presentation)

---

### 📊 3. Predicting NBA Game Outcomes
**Status:** ✅ Completed  
**Overview:**  
This project analyzes over 70 years of NBA box score data to determine which performance metrics most strongly predict game outcomes. A logistic regression model was developed using core shooting statistics, achieving ~72% accuracy and highlighting the importance of shooting efficiency—especially free throw percentage.

**Highlights:**  
- Logistic regression model for binary classification (Win/Loss)  
- FT%, FG%, and 3P% identified as top predictors  
- Strategic implications for player development and game strategy  
- Visual analysis included margin of victory distribution, heatmaps, and coefficient interpretation

**Links:**  
📂 [GitHub Repo](project_nba_game_metrics/) | 📄 [Whitepaper](project_nba_game_metrics/report) | 📊 [Slide Deck](project_nba_game_metrics/presentation/key_metrics_pres.pptx)

---

## 📁 Repository Structure

- `nba-game-metrics/`: Code and data for NBA analysis  
- `presentation/`: Project whitepapers and presentation materials  
- `statcast-home-run/`: Code for MLB home run prediction  
- `adult-income-prediction/`: Code for income classification models  
