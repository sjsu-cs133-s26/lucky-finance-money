# Lucky Finance Money

## Project Overview
This repository now uses the Kaggle **Airline Delay** dataset for data analysis and modeling work.

- Dataset link: https://www.kaggle.com/datasets/sriharshaeedala/airline-delay
- Main goal: analyze delay patterns and build insights around flight punctuality.

## Team Members
- Bryan Le
- Justin Nguyen
- Carolyna Sias
- Emily Williams
- Ngoc Huy Tran

## Dataset
Source: Kaggle - Airline Delay (by sriharshaeedala)

Typical fields in this dataset include flight date information, carrier, origin/destination airports, and delay values. Exact column names can vary based on the downloaded version.

## Getting Started
1. Clone this repository.
2. Download the dataset from Kaggle:
	- https://www.kaggle.com/datasets/sriharshaeedala/airline-delay
3. Place the raw downloaded file(s) in `data/raw/`.
4. Keep any cleaned or transformed outputs in `data/processed/`.
5. Run your analysis notebooks/scripts against files in `data/raw/` or `data/processed/`.

## Quick Download with Kaggle CLI (Optional)
If you have Kaggle API credentials configured:

```bash
kaggle datasets download -d sriharshaeedala/airline-delay -p data/raw --unzip
```

## Project Structure
```text
lucky-finance-money/
├── data/
│   ├── README.md      # Dataset download/setup instructions
│   ├── raw/           # Original files from Kaggle
│   └── processed/     # Cleaned/transformed datasets
└── README.md          # Project documentation
```

## Notes
- Do not commit large dataset files to this repository.
- Use `.gitignore` to keep raw/processed data files out of version control.
