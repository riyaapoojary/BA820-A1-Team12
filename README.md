# BA820 Project M1 — Question-Driven EDA (Primary + Backup)

This repository contains a **fully populated EDA notebook (with outputs shown)** for BA820 (Unsupervised & Unstructured Machine Learning).

## Datasets
### Primary: Hollywood Age Gaps
- File: `age_gaps.csv`
- What it is: Movie couples dataset with actor ages, character genders, and age differences.
- Goal: Explore patterns in age gaps over time and across gender pairings, and motivate segmentation at the movie level.

### Backup: SAFI African Farm Survey
- File: `safi_data.csv`
- What it is: Household/village survey data (assets, livestock, food security proxies, etc.).
- Goal: Explore household heterogeneity and motivate clustering into interpretable household “profiles”.

## Notebook
- `BA820_EDA.ipynb`  
  Includes:
  - data overview + quality checks (missing values, duplicates, ranges)
  - visual EDA (distributions, trends, group comparisons)
  - feature engineering (e.g., pairing/decade for Hollywood; item/month counts for SAFI)
  - **PCA** (dimensionality reduction)
  - **KMeans clustering** (segmentation) + cluster profiles

> The notebook is saved with outputs/plots visible for grading.

## How to Run (Google Colab)
1. Open the notebook in Colab:
   - Upload `BA820_EDA.ipynb` to Colab (or open directly from GitHub).
2. Upload the datasets into the Colab session:
   - `age_gaps.csv`
   - `safi_data.csv`
3. Run: **Runtime → Run all**

## How to Run (Local Jupyter)
1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
