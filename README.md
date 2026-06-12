# 📊 YouTube Recommendation Prediction
> Does positive audience experience increase recommendation likelihood?

A data science group project analyzing YouTube viewer analytics to predict content recommendation likelihood using statistical hypothesis testing and machine learning classification models.

---

## 🔍 Research Question

*Can a viewer's experience — measured through watch time, sentiment, and engagement — predict whether they will recommend content?*

**H₀** — Positive audience experience does NOT increase recommendation likelihood.  
**H₁** — Positive audience experience DOES increase recommendation likelihood. *(One-tailed, α = 0.05)*

---

## 📁 Project Structure

```
youtube-recommendation-prediction/
├── youtube_analytics.ipynb     # Full analysis notebook
├── presentation.pptx           # Final viva presentation
└── README.md
```

---

## 🔧 Pipeline

| Step | Description |
|------|-------------|
| A | Data Loading & Overview |
| B | Feature Engineering (Audience Experience Score) |
| C | Exploratory Data Analysis (7 visualizations) |
| D | Statistical Validation (t-test, chi-square, correlation) |
| D2 | Formal Hypothesis Testing |
| E | Predictive Modeling (Logistic Regression + Random Forest) |
| F | Evaluation & Interpretation |

---

## ⚙️ Feature Engineering

A composite **Audience Experience Score** was built from:
- `watch_time_ratio` × 0.35
- `sentiment_score` × 0.30
- `engagement_score` × 0.25
- `replay_count` × 0.10

Additional engineered features: `engagement_score`, `watch_sentiment_ix`, `high_retention`, `positive_sentiment`, `exp_tier`.

---

## 🤖 Models

| Model | Technique |
|-------|-----------|
| Logistic Regression | Baseline linear classifier |
| Random Forest | Ensemble tree-based classifier |

Both models evaluated with **5-fold stratified cross-validation** using AUC-ROC, F1-score, Precision-Recall curves, and confusion matrices.

---

## 🛠️ Tech Stack

`Python` · `pandas` · `NumPy` · `scikit-learn` · `matplotlib` · `seaborn` · `SciPy`

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yuwaniyash/youtube-recommendation-prediction.git
cd youtube-recommendation-prediction

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn scipy

# Launch notebook
jupyter notebook youtube_analytics.ipynb
```

---

## 👥 Group

IT3011 – Theory & Practices in Statistical Modeling · DATA SCIENCE (sp) 3YS1 · SLIIT

| Name |
|------|
| Devagiri D.M.U.A |
| Yasmada K.Y |
| Wijethilaka P.L.A.W.K |
| Pathirana P.U.O.R |
