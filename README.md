# applied-statistics-assessment
 
This repository contains the assessment for the Applied Statistics module at ATU as part of the HDip in Computer Science, Data Analytics. The project follows a series of problems set, serving to explore statistical analysis of various types of synthetic datasets.

The problems can be found in the [problems notebook](problems.ipynb).

There is a [requirements](requirements.txt) file containing the required packages for the project.

To execute the code contained in this project, please open the problems notebook in CodeSpaces, VSCode or JupyterNotebook in a python environment with the required packages installed.

Installing packages:

> pip install -r requirements.txt

or

> conda create --name <environment-name> --file requirements.txt

The full problems are as follows:

## Problems

### Problem 1: Extending the Lady Tasting Tea
> Let's extend the Lady Tasting Tea experiment as follows. The original experiment has 8 cups: 4 tea-first and 4 milk-first. Suppose we prepare 12 cups: 8 tea-first and 4 milk-first. A participant claims they can tell which was poured first.

> Simulate this experiment using numpy by randomly shuffling the cups many times and calculating the probability of the participant correctly identifying all cups by chance. Compare your result with the original 8-cup experiment.

> In your notebook, explain your simulation process clearly, report and interpret the estimated probability, and discuss whether, based on this probability, you would consider extending or relaxing the p-value threshold compared to the original design.

### Problem 2: Normal Distribution
> Generate 100,000 samples of size 10 from the standard normal distribution. For each sample, compute the standard deviation with ddof=1 (sample SD) and with ddof=0 (population SD). Plot histograms of both sets of values on the same axes with transparency. Describe the differences you see. Explain how you expect these differences to change if the sample size is increased.

### Problem 3: t-Tests
> A type II error occurs when a test fails to reject the null hypothesis even though it is false. For each mean difference d = 0, 0.1, 0.2, … , 1.0, repeat the following simulation 1,000 times:

> 1. Draw two samples of size 100, one from the standard normal distribution and one from the normal distribution with mean d and standard deviation 1.
> 2. Run an independent samples t-test on the two samples, rejecting the null hypothesis if the p-value is less than 0.05.
> 3. Record the proportion of times the null hypothesis is not rejected.

>Plot this proportion against d, and explain how the type II error rate changes as the difference in means increases.

### Problem 4: ANOVA
> Generate three independent samples, each of size 30, from normal distributions with means 0, 0.5, and 1, each with standard deviation 1.

> 1. Perform a one-way ANOVA to test whether all three means are equal.
> 2. Perform three independent two-sample t-tests: samples 1 vs 2, 1 vs 3, and 2 vs 3.
> 3. Compare the conclusions.

> Write a short note on why ANOVA is preferred over running several t-tests.
