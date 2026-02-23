# BA820 – Hollywood Age Gaps Project (M1–M4)

## 📌 Project Overview

This project analyzes the **Hollywood Age Gaps dataset** to examine whether on-screen romantic pairings follow a consistent age-gap pattern.

Across milestones, the analysis evolved from exploratory analysis (M1) to clustering and validation (M2–M4).

**Main question:**
> Does the data show a stable and interpretable age-gap structure (small-gap vs large-gap group), and does this pattern remain consistent across methods and decades?

---

## 📂 Repository Structure

### Milestone 1 (M1)
- Initial EDA
- Data quality checks
- Feature engineering (pairing_type, decade, age_difference)
- Early clustering exploration

### Milestone 2 (M2)
- Individual EDA notebooks (team members)
- PCA exploration
- KMeans clustering experiments

### Milestone 3 (M3)
- Integrated team analysis
- Comparison of feature sets
- Cluster stability checks

### Milestone 4 (M4) – Refinement & Validation
- Narrowed focus to dominant pairings (98% of data)
- Simplified clustering to `age_difference` only
- k=2 vs k=3 sensitivity testing
- Hierarchical clustering validation
- Adjusted Rand Index (ARI) comparison
- Decade-level descriptive analysis

**Primary notebook for grading:**
- `M4_Riya_Refinement.ipynb`

---

## 🔎 Key Methods Used

- Data cleaning & preprocessing
- Feature engineering (`age_difference`, `pairing_type`, `decade`)
- KMeans clustering
- Hierarchical (agglomerative) clustering
- Silhouette score (cluster separation quality)
- Adjusted Rand Index (method agreement check)
- Decade-level descriptive comparisons

---

## 📊 Main Findings (M4)

- The data consistently forms **two clusters**:
  - Small age-gap group (~6 years)
  - Large age-gap group (~22 years)
- The two-cluster structure is stable across methods.
- High ARI (~0.893) shows strong agreement between KMeans and hierarchical clustering.
- Cluster proportions shift across decades, but the overall two-group structure remains meaningful.

---

## ▶️ How to Run (Google Colab)

1. Open `M4_Riya_Refinement.ipynb` in Colab (or directly from GitHub).
2. Ensure `age_gaps.csv` is available in the session.
3. Run: **Runtime → Run all**

---

## 💻 How to Run (Local Jupyter)

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
