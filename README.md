# Quantitative Analysis of Trader Behavior & Market Sentiment

## Project Overview

This project investigates the relationship between Bitcoin market sentiment and trader behavior on the Hyperliquid decentralized exchange.

Using historical trade execution data and the Bitcoin Fear & Greed Index, the analysis explores how different sentiment regimes influence trading activity, profitability, participation levels, and behavioral patterns among traders.

The objective is to determine whether market sentiment affects trader decision-making and to identify behavioral archetypes that can support risk monitoring and trading analytics.

---

## Business Problem

Trading platforms and quantitative trading firms need to understand how changing market sentiment influences trader behavior and platform-wide activity.

Key questions addressed in this analysis include:

* Does market sentiment impact trader profitability?
* Do traders behave differently during Fear and Greed regimes?
* How do sentiment transitions affect trading activity?
* Can traders be segmented into meaningful behavioral groups?
* Can sentiment-aware analytics improve risk monitoring and decision-making?

---

## Datasets

### 1. Hyperliquid Historical Trade Data

Contains execution-level trading records including:

* Account information
* Trade direction
* Trade size
* Realized PnL
* Transaction fees
* Trade timestamps

### 2. Bitcoin Fear & Greed Index

Daily sentiment dataset containing:

* Sentiment score
* Sentiment classification
* Date

Sentiment regimes include:

* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

---

## Analytical Approach

The project follows a structured quantitative workflow:

### Data Preparation

* Data cleaning
* Missing value assessment
* Duplicate detection
* Timestamp standardization
* Dataset merging

### Feature Engineering

Creation of analytical features including:

* Daily PnL
* Trade frequency
* Trading volume
* Average trade size
* Win rate
* Profitability metrics
* Behavioral indicators

### Exploratory Data Analysis

Analysis of:

* Trading activity by sentiment regime
* Profitability trends
* Participation levels
* Sentiment distribution
* Behavioral shifts

### Regime Transition Analysis

Study of sentiment state changes such as:

* Fear → Greed
* Neutral → Greed
* Greed → Fear

to evaluate how traders react when market psychology changes.

### Trader Segmentation

Traders are segmented based on behavioral characteristics to identify:

* Low Activity Traders
* High Activity Traders
* Consistent Winners
* High-Risk Participants

### Behavioral Clustering

K-Means clustering is applied to discover trader archetypes based on:

* Trading activity
* Profitability
* Trade size
* Volume characteristics

### Statistical Testing

Mann-Whitney U Tests are performed to determine whether observed differences between sentiment regimes are statistically significant.

### Predictive Modeling

A tree-based machine learning model is developed to classify trader performance segments using sentiment and behavioral features.

---

## Key Findings

* Trading activity increases during Greed and Extreme Greed regimes.
* Sentiment transitions often reveal stronger behavioral changes than static sentiment levels.
* Trader groups exhibit significantly different performance characteristics.
* Higher participation periods are frequently accompanied by greater variability in outcomes.
* Behavioral clustering identifies distinct trader archetypes with varying sensitivity to market sentiment.

---

## Repository Structure

```text
Trader-Performance-vs-Market-Sentiment/
│
├── Dev_Garg_Trader_Performance_vs_Market_Sentiment.ipynb
├── historical_data.csv
├── fear_greed_index.csv
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/gargdev07/Trader-Performance-vs-Market-Sentiment.git
```

Navigate to the project directory:

```bash
cd Trader-Performance-vs-Market-Sentiment
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Requirements

Python 3.10+

Main libraries used:

* pandas
* numpy
* matplotlib
* seaborn
* scipy
* scikit-learn
* jupyter

---

## How to Run

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Dev_Garg_Trader_Performance_vs_Market_Sentiment.ipynb
```

Run all cells from top to bottom.

The notebook automatically:

1. Loads datasets
2. Cleans and prepares data
3. Performs feature engineering
4. Conducts exploratory analysis
5. Executes statistical tests
6. Performs trader segmentation
7. Builds clustering models
8. Generates visualizations and insights

---

## Results

The notebook produces:

* Sentiment regime analysis
* Trading activity visualizations
* Profitability comparisons
* Regime transition insights
* Behavioral clusters
* Statistical significance tests
* Predictive modeling outputs
* Business recommendations

---

## Author

**Dev Garg**

Data Science Undergraduate | Quantitative Analytics Enthusiast

Project completed as part of the Primetrade.ai Data Science / Analytics Internship Assignment.
