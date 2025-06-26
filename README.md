# Contextualized Probabilistic Graphical Models for Cancer Genomics

This repository contains the full implementation for my STAT 479 course project, which explores learning subtype-specific gene regulatory networks from cancer genomics data. The full project write-up can be found in the `/report` directory.

## Project Overview

This project aims to uncover differences in gene regulatory pathways across distinct colorectal cancer subtypes. We leverage **probabilistic graphical models (PGMs)**, specifically Bayesian Networks, to model these complex dependencies. Using public data from The Cancer Genome Atlas (TCGA), we apply a Bayesian hierarchical framework to infer personalized, context-specific network structures.

## Key Methods & Technologies

* **Modeling Framework:** Employed Bayesian hierarchical models to capture patient- and subtype-specific variations.
* **Causal Structure Learning:** Implemented and compared score-based structure learning algorithms, including **Hill-Climbing** and the **K2 algorithm**.
* **Scoring Functions:** Utilized both Bayesian-Dirichlet equivalent (BDeu) and Minimum Description Length (MDL) scores to evaluate network structures.
* **Tech Stack:** Python, Jupyter Notebook, Pandas, NumPy, Scikit-learn, and `pgmpy` for probabilistic modeling.

## Key Results

* The learned models successfully identified interpretable differences in regulatory topology across different cancer subtypes.
* Achieved an **83% classification accuracy** in predicting cancer subtypes based on the inferred graphical structures, demonstrating the model's effectiveness.

## How to Use

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YueYao-stat/Causal-Cancer-Genomics.git](https://github.com/YueYao-stat/Causal-Cancer-Genomics.git)
    cd Causal-Cancer-Genomics
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the analysis:**
    Open and run the cells in the `notebooks/Causal_Discovery_Analysis.ipynb` Jupyter Notebook to see the full data processing, model implementation, and results evaluation.
