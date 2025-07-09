# NBA Shot Success Classification

This project uses NBA shot log data to predict whether a basketball shot will be successful based on contextual in-game features. It applies machine learning classification techniques to explore player efficiency and shot patterns.

---

## Project Objectives

- Predict shot success (make/miss) using features like shot distance, defender proximity, shot type, and game time.
- Compare multiple classification models for accuracy and interpretability.
- Visualize optimal shooting zones and generate actionable insights for strategy analysis.

---

## Dataset

- Source: [NBA Stats API / Kaggle NBA Shot Logs Dataset](https://www.kaggle.com/datasets)
- Includes features like:
  - Shot distance
  - Defender distance
  - Shot clock
  - Shot type
  - Game period

---

## Tools & Technologies

- **Python**: pandas, numpy, scikit-learn, matplotlib, seaborn
- **Modeling**: Logistic Regression, KNN, Random Forest
- **Evaluation**: Accuracy, Confusion Matrix, Precision, Recall

---

## Key Visualizations

![Heatmap of Shot Zones](visuals/heatmap_shot_zones.png)

---

## Modeling Results

| Model              | Accuracy |
|--------------------|----------|
| Logistic Regression| 74%      |
| KNN                | 72%      |
| Random Forest      | **78%**  |

- Most important features: Shot Distance, Defender Proximity, Shot Type
- Used cross-validation to ensure robust performance

---

## Insights

- Close-range shots and open space strongly correlate with shot success.
- Heatmaps reveal high-efficiency zones for different shot types.
- Random Forest offered best performance and interpretability using feature importance scores.

---

## Future Improvements

- Include player identities for personalized models
- Add more temporal context (e.g., game momentum, fatigue)
- Deploy with Streamlit for interactive exploration

---

## Setup Instructions

```bash
git clone https://github.com/TylerKT20/NBA-Shot-Classification.git
cd NBA-SHOT-CLASSIFICATION
pip install -r requirements.txt
```