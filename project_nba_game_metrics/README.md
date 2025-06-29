# 🏀 Predicting NBA Game Outcomes with Box Score Data

This repository presents a data science project focused on identifying the core performance metrics that best predict game outcomes in the NBA. The analysis uses over 70 years of historical box score data to uncover statistically significant trends and build an interpretable predictive model.

## 📊 Project Overview

- **Author**: Xhoi Shyti  
- **Course**: DSC 680 – Project 1, Milestone 3  
- **Objective**: Determine which box score statistics most accurately predict win/loss outcomes and offer strategic insights for player development and team planning.

## 📁 Data Source

- **NBA Box Scores** (1946–2023)  
- Data collected via the NBA Stats API using a custom Python script  
- Key features include: field goal percentage (FG%), free throw percentage (FT%), three-point percentage (3P%), total points, assists, rebounds, turnovers, and game outcomes (Win/Loss)

## 🧠 Methodology

1. **Exploratory Data Analysis (EDA)**  
   - Identified long-term trends and feature correlations
   - Observed increases in 3P% and FT% over time

2. **Feature Selection**  
   - Selected statistically significant features while addressing multicollinearity  
   - Efficiency metrics (e.g., FG%, FT%) favored over raw totals (e.g., FGM, FGA)

3. **Logistic Regression Modeling**  
   - Binary classification model: Win (1) or Loss (0)  
   - Targeted interpretability and transparency for stakeholders

4. **Model Evaluation**  
   - Accuracy: ~71.5%  
   - Balanced precision and recall  
   - Confusion matrix showed ~6,500 correct predictions per class

## 🔍 Key Findings

- **Free Throw Percentage (FT%)** was the most powerful predictor, followed by FG% and 3P%.
- Shooting efficiency had greater predictive value than scoring volume.
- Strategic shot selection and consistency at the free throw line are crucial to winning.

## ⚠️ Limitations

- Contextual game factors (e.g., opponent strength, clutch scenarios) not included
- Historical inconsistencies due to rule/style changes over decades
- Advanced metrics (e.g., PER, SportVU tracking) not used

## ✅ Strategic Implications

- Prioritize shooting efficiency in player development and scouting
- Emphasize FT and 3P training across all positions
- Use predictive modeling to support game-day planning and post-game evaluation

## 🔮 Future Directions

- Integrate advanced stats like PER, TS%, and player tracking data
- Explore ensemble methods (e.g., XGBoost, Random Forest) for improved accuracy
- Adjust models to account for context like game location, opponent quality, and rest days
- Develop player-specific and team-specific variants
- Consider interactive dashboard deployment for real-time coaching insights

## 📎 Supporting Files

- 📄 [Whitepaper PDF](project_nba_game_metrics/report)  
- 📊 [Slide Deck (PowerPoint)](project_nba_game_metrics/presentation/key_metrics_latest.pptx)

---

© 2025 Xhoi Shyti | For academic and educational use only