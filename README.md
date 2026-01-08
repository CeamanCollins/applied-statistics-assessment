# Applied Statistics Assessment

## Overview

This repository contains the assessment for the *Applied Statistics* module at ATU as part of the HDip in Computer Science, Data Analytics. The project follows a series of problems designed to demonstrate applied statistical techniques.

The problems can be found in the [problems notebook](problems.ipynb).

---

## Problems

### Problem 1: Extending the Lady Tasting Tea
- Extend the Lady Tasting Tea experiment, where:
  - The standard experiment uses 8 cups (4 tea-first, 4 milk-first).
  - Extend to 12 cups (8 tea-first, 4 milk-first).
- Simulate the experiment using `numpy`:
  - Randomly shuffle cups and calculate the probability of a participant identifying all cups correctly by chance.
- Compare simulation results with theory.
- In the notebook:
  - Explain the simulation process.
  - Report and interpret the estimated probability.
  - Discuss adjustments to the experimental design based on the results.

---

### Problem 2: Normal Distribution
- Generate 100,000 samples of size 10 from the standard normal distribution.
  - Compute the sample standard deviation (`ddof=1`) and population standard deviation (`ddof=0`).
  - Plot histograms of the computed standard deviations and compare their distributions.

---

### Problem 3: t-Tests
- Investigate Type II errors:
  - For differences in means (`d` values of 0, 0.1, 0.2, ..., 1.0):
    1. Draw two samples (size 100 each) from:
       - Standard normal distribution.
       - Normal distribution with mean difference `d`.
    2. Perform independent samples t-tests.
    3. Record the proportion where the null hypothesis is not rejected (p-value ≥ 0.05).
  - Plot the Type II error rate against `d` and interpret how the error rate changes with larger mean differences.

---

### Problem 4: ANOVA
- Generate three independent samples (size 30 each) from normal distributions:
  - Means: 0, 0.5, and 1.
  - Standard deviation: 1.
- Compare conclusions from the following:
  1. Perform one-way ANOVA to test for equality of all three means.
  2. Conduct three independent two-sample t-tests:
      - Sample 1 vs Sample 2.
      - Sample 1 vs Sample 3.
      - Sample 2 vs Sample 3.
- Write a short note on why ANOVA is preferred over multiple t-tests.

---

## Setup and Installation

To execute the code in this project, follow the steps below.

### Dependencies
The repository includes a `requirements.txt` file specifying the necessary Python packages.

### Using `pip`:
Install the dependencies using pip:
```bash
pip install -r requirements.txt
```

### Using `conda`:
Alternatively, create a Conda environment using:
```bash
conda create --name <environment-name> --file requirements.txt
```

---

## Running the Notebook

This project runs on a Python environment with support for Jupyter Notebooks. Open the `problems.ipynb` file using one of the following tools once dependencies are installed:
- GitHub CodeSpaces
- VSCode
- Jupyter Notebook

---

## Technologies Used

The following technologies and tools were used in this project:
- **Python**: Programming language used for statistical calculations and simulations.
- **NumPy**: Library for numerical computations (used in simulations and calculations).
- **Matplotlib**: Visualization library for creating histograms, scatter plots, and other charts.
- **SciPy**: Library used for performing statistical tests like t-tests and ANOVA.
- **Jupyter Notebook**: Interactive environment for developing and sharing analyses.
- **GitHub CodeSpaces**: Cloud-based IDE for running and managing notebooks online.

---

This README now includes a detailed **Technologies Used** section in alignment with your other repositories. Let me know if you’d like further refinements.
