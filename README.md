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
