# IoT IDS Analysis and Export

## Project Overview

This repository contains a Jupyter Notebook for exploratory data analysis, clustering, and classification of an IoT intrusion detection dataset.

The notebook performs:
- dataset loading, sampling, and feature selection
- descriptive statistics, missing-value and duplicate checks
- correlation analysis, outlier detection, and normalization
- visualizations for class balance, feature distributions, and clustering results
- unsupervised learning with hierarchical clustering and K-means
- supervised learning with ANN, logistic regression, and random forest models
- export of numbered figures, tables, text summaries, and an asset register

## Repository Contents

- `AI_PR2.ipynb` - main analysis notebook.
- `10_PR2.pdf` - exported project report deliverable.
- `README.md` - project documentation.

## Dataset

The dataset is not included in this repository. It should be downloaded from Kaggle:

- https://www.kaggle.com/datasets/azalhowaide/iot-dataset-for-intrusion-detection-systems-ids

The notebook currently expects the downloaded file at:

- `/content/drive/MyDrive/P2/BotNeTIoT-L01_label_NoDuplicates.csv`

This path is configured for Google Colab and Google Drive mounting. If running locally, update the `DATA_PATH` variable inside `AI_PR2.ipynb` to point to the downloaded CSV file.

## Exported Assets

The notebook generates a structured export under `PR2_Export/`:

- `PR2_Export/Figures/` - numbered PNG visualizations
- `PR2_Export/Tables/` - numbered CSV tables
- `PR2_Export/Text/` - numbered text summaries
- `PR2_Export/PR2_Export_All.zip` - archive containing all generated assets
- `PR2_Export/PR2_Asset_Register.csv` - registry with asset metadata

## Key Notebook Sections

1. Part I: Data pre-processing and exploration
2. Part II: Unsupervised learning and clustering experiments
3. Part III: Supervised learning and test evaluation
4. Final asset export and asset register creation

## Requirements

The notebook uses the following Python packages:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`
- `scikit-learn`

If running on a local machine, install dependencies with:

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn
```

## Running the Notebook

1. Open `AI_PR2.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
2. If using Google Colab, keep the Drive mount cell and follow the authentication prompts.
3. Update `DATA_PATH` if the dataset is stored in a different location.
4. Execute all cells in order.

## Notes

- The notebook samples up to 10,000 rows from the dataset for analysis.
- It chooses a subset of candidate features by name, falling back to the first numeric columns if needed.
- Model evaluation uses a stratified train/test split and macro-averaged metrics.

## Contact

For questions or improvements, edit the notebook and update this repository with comments or enhancements.