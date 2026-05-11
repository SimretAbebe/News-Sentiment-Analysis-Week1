# Financial News Sentiment & Stock Price Correlation Analysis

## Project Overview
This project, conducted for **Nova Financial Solutions**, enhances predictive analytics capabilities by connecting market narratives to price action. By analyzing the **Financial News and Stock Price Integration Dataset (FNSPID)**, we successfully built an end-to-end pipeline that quantifies news sentiment, computes technical indicators, and measures their statistical relationship.

## Project Structure
```text
news-sentiment-analysis/
├── .github/workflows/      # CI/CD pipeline (GitHub Actions)
├── data/                   # Raw and processed datasets
├── notebooks/              # Jupyter notebooks for EDA and analysis
├── src/                    # Source code for utility functions
├── tests/              # Unit tests for the analysis pipeline
├── scripts/                # Standalone Python scripts
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```

## Key Tasks & Progress
### Task 1: Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** Analyzed headline lengths and publication frequency across 1.4M articles.
- **Publisher Analysis:** Identified the top 10 most active news sources.
- **Text Analysis:** Extracted significant keywords and recurring themes using NLP Bigrams.
- **Time-Series Analysis:** Mapped news volume spikes, identifying a regime shift in 2020.

### Task 2: Quantitative Analysis
- **Technical Indicators:** Implemented SMA, EMA, RSI, and MACD using **TA-Lib**.
- **Financial Metrics:** Calculated annualized volatility and log returns.
- **Visualization:** Developed an integrated dashboard for correlating indicators with price action.

### Task 3: Correlation Analysis
- **Sentiment Scoring:** Applied **NLTK VADER** to assign numerical scores to headlines.
- **Date Alignment:** Synchronized news timestamps with the stock trading calendar.
- **Pearson Correlation:** Identified a **0.1196** correlation between sentiment and returns.
- **Interpretations:** Proved that positive sentiment days correlate with higher average daily returns.

## Key Insights
- **Sentiment Signal:** While daily headlines are noisy, the aggregate sentiment provides a statistically significant leading indicator for price momentum.
- **Volatility Context:** High news volume (e.g., in 2020) acts as a baseline for increased market uncertainty and trend reversals.

## Installation & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/SimretAbebe/News-Sentiment-Analysis-Week1.git
   ```
2. **Set up the Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   ```
3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

