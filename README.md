# 🚀 SpaceX Launch Prediction & Cost Modeling

This project uses machine learning to predict the success of Falcon 9 first-stage landings based on SpaceX launch data. By accurately forecasting landing outcomes, the model enables cost estimation that can help aerospace competitors make data-driven bidding decisions.

## 📊 Project Overview

- **Goal**: Predict whether a SpaceX Falcon 9 first-stage will successfully land using historical launch data.
- **Business Value**: Accurate predictions can inform cost modeling, e.g., $62M for successful landings vs. $165M for failed ones.
- **Accuracy**: Achieved up to **94.4%** test accuracy using Logistic Regression, SVM, and Decision Tree classifiers.

## 🔧 Tech Stack

- **Languages**: Python, SQL
- **Libraries**: Pandas, Scikit-learn, Plotly, Folium, Seaborn
- **Dashboards**: Built using Plotly Dash for interactive filtering and visualization
- **Data Sources**: 
  - SpaceX REST API (v4)
  - Wikipedia scraping for historical data

## 📁 Project Structure

```

├── data/
│   ├── spacex\_launches.csv         # Final cleaned dataset
├── notebooks/
│   ├── 1\_data\_collection.ipynb     # API + scraping
│   ├── 2\_data\_wrangling.ipynb      # Cleaning, feature engineering
│   ├── 3\_eda\_sql.ipynb             # SQL analysis
│   ├── 4\_eda\_visual.ipynb          # Plotly, Folium, Seaborn
│   ├── 5\_modeling.ipynb            # ML models + tuning
│   └── 6\_dashboard.py              # Plotly Dash app
├── requirements.txt
└── README.md

```

## 📈 Key Insights

- Heavy payloads (>6000kg) were **30% less likely** to result in successful landings.
- RTLS (Return To Launch Site) landings had an **80% success rate** vs. 50% for droneships.
- Certain boosters and orbit types significantly impacted outcomes.

## 🧠 Models & Results

| Model              | Test Accuracy |
|-------------------|---------------|
| Logistic Regression | **94.4%**      |
| SVM                | **94.4%**      |
| Decision Tree      | **94.4%**      |
| K-Nearest Neighbors| 83.3%         |

Hyperparameter tuning was performed via `GridSearchCV` using 10-fold cross-validation.

## 📌 Next Steps

- Deploy the model as a real-time advisory tool for aerospace bidding strategies.
- Integrate live data feeds to keep predictions up-to-date.
- Monitor model performance post-launch to ensure continued accuracy.

## 🤝 Acknowledgements

- SpaceX for making launch data publicly available via their API.
- Wikipedia contributors for historical data.
- Coursera's Data Science Capstone for providing the project framework.

---

**Author**: [Francis Blessed Kim](https://www.linkedin.com/in/francis-kim-1931681b6/)

