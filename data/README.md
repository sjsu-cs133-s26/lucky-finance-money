# Dataset Download Instructions

This folder contains instructions for downloading the datasets used in this project. **Please do not commit actual data files to this repository.**

## Required Datasets
- Kaggle: Airline Delay
- Link: https://www.kaggle.com/datasets/sriharshaeedala/airline-delay

You can download manually from the Kaggle page or use the Kaggle CLI.

### Option 1: Manual Download
1. Open the dataset page.
2. Click **Download**.
3. Move the downloaded file(s) into `data/raw/`.

### Option 2: Kaggle CLI
1. Install Kaggle CLI (if not already installed).
2. Set up your Kaggle API token (`kaggle.json`).
3. Run:

```bash
kaggle datasets download -d sriharshaeedala/airline-delay -p data/raw --unzip
```

## Data Organization

After downloading, organize your data as follows:
```text
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


## Need Help?

If you encounter issues downloading the data:
1. Check your internet connection
2. Verify your Kaggle API token is configured correctly (if using CLI)
3. Review Kaggle access permissions and rate limits
4. Contact team members for assistance
