Here is a clean, plain-text version of your Task 1 README. I have removed all the stars and emojis so you can copy and paste it directly into your file.
## 10 Academy: Week 1 - Financial News Sentiment Analysis## Project Overview
As a Data Analyst at Nova Financial Solutions, I am building an analytical pipeline to understand how financial news headlines impact stock price movements. This project focuses on identifying the relationship between news sentiment and market trends.
## Task 1: Environment Setup and EDA
This task focused on setting up a professional development environment and conducting a rigorous Exploratory Data Analysis (EDA).
## Environment and Tools

* Operating System: Ubuntu 24.04
* Workflow: Git and GitHub with a dedicated task-1 branch.
* Environment: Python Virtual Environment (venv).
* Key Libraries: pandas, vaderSentiment, scikit-learn, matplotlib, yfinance.
* CI/CD: Configured GitHub Actions for automated testing.

## Exploratory Data Analysis (EDA) Findings

* Dataset Size: Successfully loaded and processed 1,407,328 news headlines.
* Publisher Insights:
* Identified that the top 5 publishers account for a massive portion of the news.
   * Top authors: Paul Quintaro (30.7 percent) and Lisa Levin (25.1 percent).
* Headline Lengths:
* Average headline is 73 characters.
   * This distribution helps identify noisy short headlines vs. detailed news.
* Time-Series Trends:
* Analyzed news spikes over time, normalizing dates to UTC for consistency.
   * Identified specific busy hours for financial reporting (Market hours UTC-4).

## Sentiment and Text Analysis

* Sentiment Analysis: Used the VADER model to score headlines.
* Neutral: ~52 percent (Majority of financial news is factual).
   * Positive: ~31 percent (Earnings beats, upgrades).
   * Negative: ~17 percent (Price drops, bearish bets).
* Keyword Extraction: Used CountVectorizer to find recurring themes like Earnings, Price Target, and Stocks.





## 📂 Project Structure
```text
news-sentiment-analysis/
├── data/
│   └── raw/              # CSV and Zip data files
├── notebooks/
│   ├── 01_eda_news.ipynb # Main Task 1 Analysis
│   └── README.md         # Notebook documentation
├── src/                  # Source code for reusable functions
├── .github/workflows/    # CI/CD pipelines
├── .gitignore            # Files to ignore (venv, data/)
└── requirements.txt      # List of dependencies
```
