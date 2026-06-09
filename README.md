# CaseStudy_Team-Numbers-Don-t-Lie

<img width="623" height="624" alt="Screenshot 2026-02-01 155942" src="https://github.com/user-attachments/assets/3b5ea46d-322b-4a7f-8e9f-a9a711d3066d" />


---------------------------------Preview of the DashBoard------------------------------------
# Spotify Predictive Analytics: Decoding Regional vs. Global Hit Drivers 

### Can Machine Learning predict whether a Spotify song becomes a hit because of *how it sounds*… or *who sings it*?

This project explores the hidden mechanics behind music success by comparing **Spotify India** and **Spotify Global** ecosystems through predictive analytics and machine learning.

Instead of assuming that streaming success follows a universal formula, we investigate whether popularity is driven by:

* **Sonic Identity** → audio characteristics such as tempo, energy, loudness, acousticness
* **Artist Equity** → artist reputation, followers, popularity, and market influence

The result is an interactive analytics framework that reveals how different audiences consume music across regions.

---

## Project Objective

Modern recommendation systems often assume that songs succeed under similar conditions worldwide.

This project challenges that assumption.

Using machine learning and dashboard analytics, we identify:

* Which variables contribute most to creating a Spotify hit
* How listener behavior differs between India and global markets
* Whether artist reputation outweighs musical quality
* How future streaming trends may evolve regionally

---

## Dataset Overview

The analysis combines processed Spotify datasets enriched with:

### Audio Features

* Tempo (BPM)
* Energy
* Loudness
* Acousticness
* Danceability
* Duration

### Artist Features

* Followers
* Popularity Index
* Release Timeline
* Historical Performance

### Engineered Variables

* `hit_flag`
* Regional Market Tags
* Forecast Indicators

---

## Machine Learning Pipeline

### 1. Data Processing

* Data cleaning and null handling
* Feature encoding
* Dataset consolidation
* Feature engineering

### 2. Hit Prediction Model

A **Random Forest Classifier (100 Trees)** predicts whether a track becomes a platform hit.

#### Classification Rule

```python
hit_flag = 1 if popularity >= 70 else 0
```

Output:

* Hit probability
* Feature importance rankings
* Regional success comparison

---

### 3. Market Forecasting

A **Linear Regression model** was used to estimate:

* Regional language growth
* Artist popularity evolution
* Streaming trajectory (2025–2027)

---

## Technology Stack

| Layer           | Technologies          |
| --------------- | --------------------- |
| Data Processing | Python, Pandas, NumPy |
| Modeling        | Scikit-Learn          |
| Visualization   | Power BI              |
| Analysis        | Matplotlib, Seaborn   |
| Version Control | Git, GitHub           |

---

# Key Findings

## 🇮🇳 Spotify India → Content Wins

Success is driven more by **musical composition and listening experience** than celebrity status.

Top Drivers:

1. Artist Reputation
2. Loudness
3. Tempo
4. Energy

---

## Spotify Global → Brand Wins

Success becomes increasingly dependent on platform dominance.

Top Drivers:

1. Artist Followers
2. Duration Optimization
3. Artist Popularity
4. Release Recency

---

## Core Insight

> India behaves more like a **music-first market**, while global ecosystems demonstrate stronger **brand reinforcement effects**.

This suggests that recommendation systems and music marketing strategies should not be generalized across regions.

---

## Dashboard Design

The dashboard was designed as a **three-layer analytical experience**:

### Executive View

* Total Tracks
* Hit Threshold
* Regional Distribution
* Streaming KPIs

### Explainability Layer

* Feature Importance Charts
* Regional Comparison
* Driver Ranking

### Forecast Layer

* Future Growth Curves
* Artist Sustainability Index
* Regional Expansion Trends

---

## Repository Structure

```text
spotify-predictive-analytics/
│
├── data/
│   ├── songs_india_cleaned_fe.csv
│   ├── global_ml_features_with_hit_flag.csv
│   └── master_training_set.csv
│
├── models/
│   ├── spotify_ml_training_script.py
│   └── trend_forecasting_script.py
│
├── visualizations/
│   ├── ml_success_drivers.png
│   ├── language_prediction_chart.png
│   └── artist_prediction_chart.png
│
├── dashboard/
│   └── spotify_predictive_dashboard.pbix
│
└── README.md
```

---

## Future Improvements

* Deploy dashboard publicly
* Add XGBoost and SHAP explainability
* Integrate Spotify API for real-time predictions
* Expand to additional regional markets
* Build recommendation simulation engine

---

### Contributors

Built during a Gemini + Power BI analytics challenge.

Exploring how data can decode the business of music.
