# First- # 🏥 Healthcare Code Swapping Detection

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

## 📌 Project Overview

A biopharmaceutical company identified **$13 million in improper payments** across 404 pharmacies due to a fraudulent practice known as **"code swapping"** — changing medical billing codes to maximize reimbursement from patient assistance programs.

This project develops a data-driven anomaly detection framework to identify suspicious billing patterns, quantify financial impact, and outperform existing detection systems.

🔗 **[View the Complete Analysis Notebook](https://github.com/alejandrocanulchan-IATB/First-/blob/main/code_swapping_healthcare_providers.ipynb)**

---

## 🎯 Business Problem & Objectives

**Problem:** Healthcare providers may exploit patient assistance programs by systematically altering CPT (Current Procedural Terminology) codes to obtain higher reimbursements.

**Objectives:**
- Detect providers with abnormally high single-code concentration (>80%)
- Analyze correlation between billing patterns and high payments
- Identify atypical CPT-ICD code combinations
- Estimate financial impact and prioritize audit targets

---

## 🔍 Key Findings

| Finding | Result |
|:--------|-------:|
| **Suspicious providers** (>80% single CPT code) | 5,350 providers (74.4%) |
| **Atypical CPT-ICD combinations** | 10 identified (z-score < -1) |
| **Potentially overpaid amount** | **$1.84 million** |
| **Improvement over dataset's anomaly flag** | 14.3x more claims flagged |

### 📊 Detection Performance Comparison

| Model | Claims Flagged | Billed Amount |
|:---|:---:|:---:|
| Dataset's anomaly flag | 394 | $399,072 |
| **Code-swapping detection** | **5,653** | **$1,835,482** |
| **Improvement** | **+5,259 claims** | **+$1.44M** |

---

## 🛠️ Technologies Used

- **Python 3.8+** – Core programming language
- **Pandas & NumPy** – Data manipulation and analysis
- **Matplotlib & Seaborn** – Data visualization
- **SciPy** – Statistical analysis (z-scores)
- **Jupyter Notebook** – Interactive development environment
- **Git & GitHub** – Version control and collaboration

---

## 📁 Repository Structure

## 🚀 How to Run This Project

### 1. Clone the repository
```bash
git clone https://github.com/alejandrocanulchan-IATB/First-.git
cd First-

---

## 📈 Methodology

### 1. Provider-level CPT Code Concentration
- Group claims by provider and CPT code
- Calculate percentage of claims under most frequent code
- Flag providers with >80% single-code usage

### 2. Correlation Analysis
- Compare concentration percentages with average billed amounts
- Compute Pearson correlation coefficient

### 3. Atypical CPT-ICD Combinations
- Calculate frequency of each code pair
- Compute z-scores to identify statistically rare combinations

### 4. Financial Impact Estimation
- Flag suspicious claims (high concentration + atypical combos)
- Sum billed amounts as potential overpayment

---

## 💡 Business Recommendations

| Priority | Action | Estimated Recovery |
|:---|:---|:---:|
| **Tier 1 (Immediate)** | Audit providers with single claims >$10,000 | ~$85,000 |
| **Tier 2 (Secondary)** | Review providers with >80% concentration | ~$1.7M |
| **System Enhancement** | Integrate code-swapping metrics into production monitoring | Ongoing |

---

## 🚀 How to Run This Project

### 1. Clone the repository
```bash
git clone https://github.com/alejandrocanulchan-IATB/First-.git
cd First-

jupyter notebook code_swapping_healthcare_providers.ipynb


The notebook includes the following visualizations:

Top 10 providers by single CPT code concentration (bar chart)

Distribution of concentration across all providers (histogram with KDE)

Provider concentration vs. average billed amount (scatter plot)

Comparison of anomaly detection models (bar charts)

Top suspicious providers by billed amount (bar chart)

Author
Alejandro Canul Chan
Data Analyst and M.Sc. Biotechnology
https://img.shields.io/badge/LinkedIn-Connect-blue


License
This project is licensed under the MIT License – see the LICENSE file for details.

Acknowledgments
Inspired by real-world healthcare fraud cases

Synthetic dataset generated for demonstration purposes

Thanks to the data science community for open-source tools

 Disclaimer
This project uses synthetic data for illustrative purposes only. The findings and financial estimates are hypothetical and should not be used for real-world decision-making without validation against actual claims data.



## 📝 Next Steps

Since your repository currently only contains the notebook, you might want to add:

1. **`requirements.txt`** – List of Python dependencies:



2. **`LICENSE`** – MIT License file (optional but recommended)

3. **`data/` folder** – You can add a `.gitkeep` file with a note that the actual data is synthetic and available upon request

Would you like me to generate any of these additional files for you?

