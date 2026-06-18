# Stock ML Backtesting Pipeline

A machine learning-based stock analysis and backtesting pipeline using Korean stock market data from Naver Finance.

## Overview

This project collects Korean stock market data, preprocesses time-series price data, creates technical indicators, trains machine learning models, and compares trading strategies through a simple backtesting process.

The project was originally developed as part of a Data Analysis Programming class and later cleaned and documented for portfolio use.

## 🇰🇷 한국어 소개

이 프로젝트는 네이버 금융 데이터를 활용하여 국내 주식 데이터를 수집하고, 시계열 가격 데이터를 전처리한 뒤 머신러닝 모델과 백테스팅 전략을 비교하는 데이터 분석 프로젝트입니다.

데이터 수집, 전처리, 피처 엔지니어링, 모델 학습, 전략 성과 비교 과정을 하나의 파이프라인으로 구성했습니다.

## Features

* Crawls top-volume Korean stock data from Naver Finance
* Retrieves KOSPI market information
* Collects daily stock price data by stock code
* Performs preprocessing and feature engineering
* Creates moving averages, daily returns, volatility, drawdown, and volume-change features
* Trains machine learning models to predict next-day price movement
* Compares model-based strategy, moving-average rule strategy, and buy-and-hold strategy
* Saves feature importance, strategy signals, and summary results

## Tech Stack

* Python
* Pandas
* NumPy
* Requests
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* XGBoost
* Jupyter Notebook

## Machine Learning Models

The project uses the following models:

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

The models are evaluated using:

* Accuracy
* F1 Score
* ROC-AUC

## Backtesting Strategies

This project compares three strategies:

1. Moving Average Rule Strategy
2. Machine Learning Model Strategy
3. Buy and Hold Strategy

The strategy performance is measured using:

* Total Return
* CAGR
* Maximum Drawdown

## How to Run

Install the required libraries:

```bash
pip install pandas numpy requests matplotlib seaborn plotly scikit-learn xgboost openpyxl
```

Open the notebook:

```bash
jupyter notebook
```

Then run the modeling and backtesting notebook.

You can enter a Korean stock name, a six-digit stock code, or use `AUTO` to automatically select a top-volume stock.

## Output Files

The pipeline generates the following output files:

* `output/feature_importance_top3.csv`
* `output/strategy_signals.csv`
* `output/c3_summary.json`

## My Role

This project is a cleaned and documented version of a class/team project.

My contribution focused on organizing the data analysis pipeline, improving the modeling and backtesting workflow, and preparing the project for portfolio use.

## What I Learned

Through this project, I practiced:

* Working with real financial data
* Collecting data from web APIs
* Cleaning and preprocessing time-series data
* Creating technical indicators for machine learning
* Training classification models
* Comparing trading strategies with backtesting
* Documenting a project for GitHub and portfolio use

## Future Improvements

* Refactor notebook code into reusable Python modules
* Add more technical indicators
* Improve validation with walk-forward testing
* Add more stocks and longer time ranges
* Build a Streamlit dashboard for interactive visualization
* Add Docker support for easier execution
# stock-ml-backtest
Machine learning-based stock analysis and backtesting pipeline using Naver Finance data.
