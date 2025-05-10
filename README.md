# Optimizing Team Tactics in Valorant

A data-driven analysis of agent selection strategies and economic decisions using Valorant Champions Tour (VCT) data (2021–2025).

## Team  
Vedant Hirekar, Dhruvil Joshi, Naishal Shah

## Project Overview

Valorant is a tactical 5v5 FPS where outcomes often hinge on more than just aim, economic decisions and agent compositions significantly affect team success. This project explores:

- How team economy (buy category) influences round win rates.
- How agent compositions perform across different maps.

## Dataset

Data sourced from **Kaggle**, covering VCT matches from 2021 to 2025. It includes:

- Match IDs, player IDs
- Agent picks
- Buy categories (Eco, Semi-Eco, Semi-Buy, Full-Buy)
- Map names and round outcomes

Dataset Link - https://www.kaggle.com/datasets/ryanluong1/valorant-champion-tour-2021-2023-data/data

## Methodology

**Data Preprocessing**
- Cleaned missing values, standardized columns
- Filtered relevant matches and structured team-level round data

**Analysis & Modeling**
- Visualizations to examine economy and agent pick trends
- Hypothesis testing on buy category win rates
- ML model (XGBoost) trained to predict win probability based on agent compositions


## How to Run

You can first download all the reqirements/libraries using the command `pip install -r requirements.txt` to execute the script.

We have directly referenced the data from the Kaggle API so the notebooks can be directly run to replicate the data cleaning, visualizations, and model training.

## Tools Used

- Python (Pandas, Seaborn, Scikit-learn, XGBoost)
- Google Colab

## Limitations & Future Work

- Limited support for rare comps (small sample size)
- No modeling of multi-round momentum or utility usage
- Data limited to pro matches—may not generalize to ranked play

**Planned Improvements:**
- Incorporate time-series elements for round sequences
- Add ability usage data of each agents (flashes, smokes)
- Explore reinforcement learning for dynamic composition/buy suggestions

---

For any questions or suggestions, feel free to open an issue or contact the team.
