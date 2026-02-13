# Dataset Download Instructions

This folder contains instructions for downloading the datasets used in this project. **Please do not commit actual data files to this repository.**

## Required Datasets

### 1. Financial Market Data
**Source:** Yahoo Finance or Alpha Vantage API

**Instructions:**
1. Visit [Yahoo Finance](https://finance.yahoo.com/) or sign up for a free API key at [Alpha Vantage](https://www.alphavantage.co/)
2. Download historical stock data for the following tickers:
   - Major indices (S&P 500, NASDAQ, Dow Jones)
   - Individual stocks of interest
3. Save the data in CSV format in this `data/` directory
4. Recommended filename format: `{ticker}_{start_date}_{end_date}.csv`

**Example using Python:**
```python
import yfinance as yf

# Download S&P 500 data
ticker = yf.Ticker("^GSPC")
data = ticker.history(period="5y")
data.to_csv("data/SP500_5y.csv")
```

### 2. Economic Indicators (Optional)
**Source:** FRED (Federal Reserve Economic Data)

**Instructions:**
1. Visit [FRED](https://fred.stlouisfed.org/)
2. Search for economic indicators such as:
   - GDP growth rate
   - Unemployment rate
   - Inflation rate
3. Download data in CSV format
4. Save to this `data/` directory

### 3. Alternative Dataset Sources
- [Kaggle Datasets](https://www.kaggle.com/datasets) - Various financial datasets
- [Quandl](https://www.quandl.com/) - Financial and economic data
- [Google Finance](https://www.google.com/finance) - Current market data

## Data Organization

After downloading, organize your data as follows:
```
data/
├── README.md          # This file
├── raw/               # Original downloaded data
├── processed/         # Cleaned and processed data
└── .gitkeep           # Keep empty folders in git
```

## Important Notes

⚠️ **Do not commit large data files to this repository!**
- Add data files to `.gitignore`
- The `.gitignore` file in the root directory already excludes common data formats
- If sharing data with team members, use external storage (Google Drive, Dropbox, etc.)

## Data Format Requirements

Ensure your downloaded data includes the following columns (for stock data):
- Date
- Open
- High
- Low
- Close
- Volume
- (Optional) Adjusted Close

## Need Help?

If you encounter issues downloading the data:
1. Check your internet connection
2. Verify API keys are valid (if using APIs)
3. Review API rate limits
4. Contact team members for assistance
