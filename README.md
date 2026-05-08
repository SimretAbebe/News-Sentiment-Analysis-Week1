# Financial News Sentiment & Stock Price Correlation Analysis

## Project Overview
This project, conducted for **Nova Financial Solutions**, aims to enhance predictive analytics capabilities by connecting market narratives to price action. By analyzing the **Financial News and Stock Price Integration Dataset (FNSPID)**, we separate "signal from noise" to determine the statistical relationship between news sentiment and stock market movements.

## Project Structure
```text
news-sentiment-analysis/
├── .github/workflows/      # CI/CD pipeline (GitHub Actions)
├── data/                   # Raw and processed datasets
├── notebooks/              # Jupyter notebooks for EDA and analysis
├── src/                    # Source code for utility functions
├── tests/                  # Unit tests for the analysis pipeline
├── scripts/                # Standalone Python scripts
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```

## Key Tasks & Progress
### Task 1: Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** Analyzed headline lengths and publication frequency.
- **Publisher Analysis:** Identified the top 10 most active news sources.
- **Text Analysis:** Extracted significant keywords and recurring themes using NLP.
- **Time-Series Analysis:** Mapped news volume spikes, identifying a regime shift in 2020.

### Task 2: Quantitative Analysis
- **Technical Indicators:** Implemented SMA, EMA, RSI, and MACD using **TA-Lib**.
- **Financial Metrics:** Calculated annualized volatility and log returns.
- **Visualization:** Developed an integrated dashboard for correlating indicators with price action.

### Task 3: Correlation Analysis (Upcoming)
- Sentiment scoring using NLTK VADER.
- Date alignment between news and trading days.
- Pearson correlation analysis and investment strategy recommendations.

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

