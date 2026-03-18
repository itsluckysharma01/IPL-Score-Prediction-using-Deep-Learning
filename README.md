# IPL Score Prediction using Deep Learning

Interactive deep learning project to predict IPL innings scores from match context such as teams, venue, batsman, bowler, runs, wickets, and overs.

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](IPL.ipynb)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## Quick Navigation

- [Project Overview](#project-overview)
- [Live Notebook Actions](#live-notebook-actions)
- [Project Highlights](#project-highlights)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)
- [Run Locally](#run-locally)
- [Interactive Prediction Widget](#interactive-prediction-widget)
- [Model Workflow](#model-workflow)
- [Future Improvements](#future-improvements)

## Project Overview

This project builds a deep learning regression model that predicts final IPL scores during an innings.
It includes:

- Data loading and preprocessing
- Label encoding of categorical cricket features
- Feature scaling with MinMaxScaler
- Neural network training with Keras
- Interactive score prediction using ipywidgets

## Live Notebook Actions

- Open notebook locally: [IPL.ipynb](IPL.ipynb)
- Open in GitHub: [View on GitHub](https://github.com/itsluckysharma01/IPL-Score-Prediction-using-Deep-Learning/blob/main/IPL.ipynb)
- Open in Colab: [Run in Colab](https://colab.research.google.com/github/itsluckysharma01/IPL-Score-Prediction-using-Deep-Learning/blob/main/IPL.ipynb)

## Project Highlights

<details>
<summary><strong>Click to expand key features</strong></summary>

- End-to-end notebook workflow from EDA to prediction
- Categorical encoding for venue, teams, batsman, and bowler
- Deep neural network with Huber loss for robust regression
- Interactive widget interface for real-time score predictions

</details>

## Tech Stack

| Area          | Tools               |
| ------------- | ------------------- |
| Language      | Python              |
| Data          | pandas, numpy       |
| Visualization | matplotlib, seaborn |
| ML / DL       | scikit-learn, keras |
| Notebook UI   | ipywidgets          |

## How It Works

1. Load IPL historical ball-by-ball style data.
2. Explore trends (venues, batsmen, bowlers, wickets).
3. Encode categorical inputs using LabelEncoder.
4. Select features and split into train/test sets.
5. Scale features using MinMaxScaler.
6. Train a Keras regression model.
7. Predict innings total through interactive widgets.

## Run Locally

### 1. Clone Repository

```bash
git clone https://github.com/itsluckysharma01/IPL-Score-Prediction-using-Deep-Learning.git
cd IPL-Score-Prediction-using-Deep-Learning
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn keras ipywidgets notebook
```

### 3. Launch Notebook

```bash
jupyter notebook IPL.ipynb
```

## Interactive Prediction Widget

The notebook includes dropdowns and numeric inputs for:

- Venue
- Batting team
- Bowling team
- Striker
- Bowler
- Runs, wickets, overs, and striker indicator

Then click **Predict Score** to get a predicted total runs value.

## Model Workflow

<details>
<summary><strong>Expand training setup</strong></summary>

- Input features: teams, venue, batsman, bowler, wickets, overs, striker, runs
- Target: innings total score
- Architecture: Dense(512, relu) -> Dense(216, relu) -> Dense(1, linear)
- Loss function: Huber loss
- Optimizer: Adam

</details>

## Future Improvements

- Add model comparison (XGBoost, Random Forest, LSTM)
- Add evaluation metrics dashboard (MAE, RMSE, R2)
- Deploy as a web app with Streamlit or FastAPI
- Add CI checks and reproducible environment files

## Author

Lucky Sharma
