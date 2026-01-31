# MAPQ Experimental Project

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Language](https://img.shields.io/badge/Language-R-blue)
![Framework](https://img.shields.io/badge/Framework-Quarto-blueviolet)

The **Modified Attitudes on Psychedelics Questionnaire (MAPQ)** is a scientific project designed to validate a psychometric instrument for the Canadian context and explore causal relationships between demographic factors and knowledge sharing behaviors.

## 🚀 Project Overview

This repository hosts the source code and analysis pipeline for the **MAPQ Experiment**. It is built using [Quarto](https://quarto.org/) and deployed via Posit Connect.

### Key Objectives
1.  **Psychometric Validation**: Validate the 4-factor structure of the MAPQ using Exploratory and Confirmatory Factor Analysis (EFA/CFA) and Monte Carlo simulations.
2.  **Causal Inference**: Apply Double Machine Learning (DML) to estimate the causal effect of gender on knowledge sharing, controlling for high-dimensional confounders.
3.  **Reproducibility**: Ensure all analyses are transparent, version-controlled, and reproducible.

## 📊 Analysis Modules

The project is divided into two primary computational modules:

### 1. Psychological Metrics (`analysis_psych.qmd`)
*   **Reliability**: Cronbach's Alpha and McDonald's Omega.
*   **Factor Analysis**: EFA and CFA on both observed and simulated data.
*   **Simulation**: Monte Carlo simulation (`mvrnorm`) to test structural robustness.

### 2. Causal Machine Learning (`analysis_dml.qmd`)
*   **Double Machine Learning**: Estimation of Average Treatment Effects (ATE) using the `DoubleML` package.
*   **SMOTE**: Synthetic Minority Over-sampling Technique to handle class imbalance.
*   **LATE**: Local Average Treatment Effect estimation using Instrumental Variables (Simulated).

## 🛠️ Tech Stack

*   **Language**: R (Primary)
*   **Publishing**: Quarto
*   **Deployment**: Posit Cloud / Connect
*   **Key Libraries**:
    *   `psych`, `psychTools`: Psychometrics
    *   `DoubleML`, `mlr3`: Causal Machine Learning
    *   `lavaan`: Structural Equation Modeling
    *   `knitr`, `kableExtra`: Reporting

## 📂 Repository Structure

```
mapq-analysis/
├── _quarto.yml          # Project configuration (Navigation, Theme)
├── index.qmd            # Home page (Project Scope)
├── about.qmd            # Author & adaptation context
├── analysis_psych.qmd   # Psychometric analysis source
├── analysis_dml.qmd     # Causal ML analysis source
├── data/                # Observational datasets (Secured)
├── styles.css           # Custom CSS for scientific formatting
├── deploy.R             # Deployment script for Posit Connect
└── manifest.json        # Environment manifest for reproduction
```

## 🔐 Security & Privacy

*   **Data Protection**: Raw data is stored in restricted directories.
*   **Configuration**: Sensitive API keys and credentials are managed via `.env` files (git-ignored) and environment variables.

## ✍️ Author

**Vansh Singh Ruhela**  
*Independent Researcher*  
Centre for Criminology and Sociolegal Studies, University of Toronto  
[GitHub](https://github.com/ruhelavansh-oss) | [ORCID](https://orcid.org/0009-0004-1750-3592)

## 📄 License

This project is open-source. Please view the [LICENSE](LICENSE) file for more details.

---
*Copyright © 2026 Vansh Singh Ruhela.*
