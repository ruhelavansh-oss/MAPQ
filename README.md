# MAPQ Experimental Project

This repository contains the source code, data processing pipelines, and analytical reports for the Modified Attitudes on Psychedelics Questionnaire (MAPQ) project. The study focuses on the psychometric validation of the instrument and the application of causal inference methods to observational behavioral data.

## Project Overview

The MAPQ project is a scientific initiative designed to evaluate a psychometric instrument within the Canadian demographic context. It utilizes advanced statistical frameworks to ensure the reliability of the measurement and explores the causal impact of demographic variables on knowledge-sharing behaviors.

### Primary Objectives
1.  **Psychometric Validation**: Verification of the 4-factor structure through Exploratory Factor Analysis (EFA), Confirmatory Factor Analysis (CFA), and Monte Carlo simulations.
2.  **Causal Inference**: Estimation of Average Treatment Effects (ATE) and Local Average Treatment Effects (LATE) using Double Machine Learning (DML) architectures.
3.  **Scientific Reproducibility**: Implementation of a version-controlled, containerized workflow to ensure all results are verifiable and transparent.

## Analysis Modules

The project is structured into two distinct computational modules:

### 1. Psychological Metrics (analysis_psych.qmd)
*   **Reliability Assessment**: Calculation of Cronbach's Alpha and McDonald's Omega coefficients.
*   **Structural Modeling**: Execution of EFA and CFA on observed and synthetic datasets.
*   **Robustness Testing**: Implementation of Monte Carlo simulations to validate factor stability across generated distributions.

### 2. Causal Machine Learning (analysis_dml.qmd)
*   **Estimation Framework**: Utilization of the Interactive Regression Model (IRM) within the DoubleML framework.
*   **Class Balancing**: Application of the Synthetic Minority Over-sampling Technique (SMOTE) to mitigate demographic group imbalance.
*   **Instrumental Variables**: Simulation-based LATE estimation to address potential unobserved confounding.

## Technical Stack

*   **Platform**: Quarto Publishing System
*   **Language**: R System for Statistical Computing
*   **Deployment**: Posit Connect / Posit Cloud
*   **Core Libraries**:
    *   `psych`, `psychTools`: Psychometric analytics
    *   `DoubleML`, `mlr3`: Causal inference and machine learning
    *   `lavaan`: Structural equation modeling
    *   `knitr`, `kableExtra`: Scientific reporting and table generation

## Repository Structure

```
mapq-analysis/
├── _quarto.yml          # Global configuration and navigation
├── index.qmd            # Project Introduction and Scope
├── about.qmd            # Author metadata and study context
├── analysis_psych.qmd   # Psychometric analysis implementation
├── analysis_dml.qmd     # Causal machine learning implementation
├── data/                # Observational datasets
├── styles.css           # Scientific formatting and visual styles
├── README.md            # Project documentation
└── LICENSE              # MIT License documentation
```

## Security and Data Integrity

*   **Confidentiality**: Access to raw observational data is restricted to authorized environments.
*   **Secret Management**: Sensitive configuration parameters and API credentials are managed via environment variables and are excluded from version control.

## Author

**Vansh Singh Ruhela**  
Centre for Criminology and Sociolegal Studies, University of Toronto  
Centre for Criminology and Sociolegal Studies, University of Toronto  
[GitHub](https://github.com/ruhelavansh-oss) | [ORCID](https://orcid.org/0009-0004-1750-3592)

## License

This project is licensed under the terms of the MIT License. See the [LICENSE](LICENSE) file for the full text.

---
*Copyright © 2026 Vansh Singh Ruhela. All rights reserved.*