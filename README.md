# UNSUPERVISED FRAUD DETECTION ON BANK TRANSACTIONS

**this repository focuses on analyzing a financial transaction dataset to identify anomalies and potential fraud using unsupervised learning techniques.**

## OVERVIEW

this project leverages both **R** and **python** to perform a complete analysis that includes:

- **feature engineering:**  
  creation of new features (e.g., transaction ratio, days since last transaction, device/ip change flags) to enrich the dataset.

- **exploratory data analysis (eda):**  
  in-depth exploration and visualization of the data to understand patterns and detect outliers.

- **clustering & anomaly detection:**  
  application of hierarchical clustering, pca, dbscan, and lof to isolate and characterize suspicious transactions.

## DATA SOURCE

the dataset is sourced from kaggle:  
[**bank transaction dataset for fraud detection**](https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection)

it contains **2,512 transactions** with detailed attributes on bank accounts, transaction characteristics, and user behavior.

## REPOSITORY CONTENTS

- **dataset:**  
  the original csv file is included in the repository.

- **r markdown script:**  
  contains the full analysis performed in **r**, along with a knitted pdf report.

- **knitted pdf report:**  
  a detailed report with commentary on the analysis results.

- **python script for google colab:**  
  a **python** version of the analysis designed to run on google colab, reproducing the **r** analysis.

## TOOLS & LIBRARIES

- **r & r markdown:**  
  used for data processing, visualization, clustering, and anomaly detection.

- **python:**  
  utilizes libraries such as:
  - **pandas** & **numpy** for data manipulation.
  - **matplotlib** & **seaborn** for visualization.
  - **scikit-learn** for clustering (pca, dbscan) and anomaly detection (lof).
  - **prince** for multiple correspondence analysis (mca).

- **clustering techniques:**
  - hierarchical clustering using **ward's method**.
  - principal component analysis (**pca**) for dimensionality reduction.

- **anomaly detection techniques:**
  - **dbscan** (density-based spatial clustering of applications with noise).
  - **local outlier factor (lof)**.

## HOW TO RUN THE PROJECT

### R analysis

1. open the provided **r markdown** file.
2. knit the document to run the analysis and generate the pdf report.
3. review the pdf for detailed results and commentary.

### python analysis (google colab)

1. open the provided **python script** in google colab.
2. upload the dataset (or load it directly from github/kaggle).
3. run each cell to reproduce the analysis steps, including feature engineering, eda, clustering, and anomaly detection.
4. visualizations and results will be generated inline.

## RESULTS & CONCLUSIONS

✅ **key findings:**  
- **cluster 1** exhibits the highest fraud indicators, including high transaction ratios, frequent device/ip changes, and login anomalies.  
- **dbscan** effectively detected noise points, which were further analyzed with hierarchical clustering.  
- **lof** flagged localized outliers, complementing the density-based anomaly detection.

✅ **real-world relevance:**  
- the approach mirrors how a bank investigates fraud, focusing on transaction patterns rather than binary fraud labels.  
- the insights can guide risk management teams in refining their fraud prevention strategies.

✅ **next steps & improvements:**  
- **enhance model interpretability:** develop a scoring system for fraud risk assessment.  
- **real-time fraud detection:** deploy models in production with continuous monitoring.  
- **integrate external data:** cross-check flagged transactions with external fraud databases.

## CONTRIBUTION

**teamwork with tommaso biganzoli (github: [Biguz-commits])**

---

## LICENSE

this project is licensed under the **mit license**.







