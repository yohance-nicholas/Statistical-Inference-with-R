# Statistical Inference Course Project
Prepared by Yohance Nicholas
Date: 03/15/2020

# Overview
This project was completed in partial fulfilment of the Statistical Inference Course which comprises one of the five courses necessary for the Data Science: Statistics and Machine Learning Specialization offered by Johns Hopikins University through Coursera.

This project consists of two parts:

1. A simulation exercise; and 
2. Basic inferential data analysis.

To be considered successful in the completion of the assignment, it is required that candidates generate a PDF report to answer questions identified. For ease of peer-review, each part must not exceed three pages in length.  

# Parts of the Coursework Project
## Part 1. Simulation Exercise

In this project, candidates will investigate the exponential distribution in R and compare it with the Central Limit Theorem. The exponential distribution can be simulated in R with rexp(n, lambda) where lambda is the rate parameter. The mean of exponential distribution is 1/lambda and the standard deviation is also 1/lambda. Set lambda = 0.2 for all of the simulations. Candidates will investigate the distribution of averages of 40 exponentials (with the assistance of a thousand simulations)

Illustrate via simulation and associated explanatory text the properties of the distribution of the mean of 40 exponentials. You should

1. Show the sample mean and compare it to the theoretical mean of the distribution.
2. Show how variable the sample is (via variance) and compare it to the theoretical variance of the distribution.
3. Show that the distribution is approximately normal.

In point 3, focus on the difference between the distribution of a large collection of random exponentials and the distribution of a large collection of averages of 40 exponentials.

As a motivating example, compare the distribution of 1000 random uniforms

```R
hist(runif(1000))
```


and the distribution of 1000 averages of 40 random uniforms  

```R
mns = NULL
for (i in 1 : 1000) mns = c(mns, mean(runif(40)))
hist(mns)
```

### Proposed Structure for Part 1

As was mentioned previously, For ease of peer-review, each part must not exceed three pages in length. The instructions have provided a sample set of headings which might be used to guide the creation of each report:

* **Title** (give an appropriate title) and Author Name
* **Overview:**  In a few (2-3) sentences explain what is going to be reported on.
* **Simulations:** Include English explanations of the simulations you ran, with the accompanying R code. Your explanations should make clear what the R code accomplishes.
* **Sample Mean versus Theoretical Mean:** Include figures with titles. In the figures, highlight the means you are comparing. Include text that explains the figures and what is shown on them, and provides appropriate numbers.
* **Sample Variance versus Theoretical Variance:** Include figures (output from R) with titles. Highlight the variances you are comparing. Include text that explains your understanding of the differences of the variances.
* **Distribution:** Via figures and text, explain how one can tell the distribution is approximately normal.

## Part 2. Basic Inferential Data Analysis

The second portion of the project requires an analysis of the ToothGrowth data in the R datasets package. Recommended steps include the following:

1. Load the ToothGrowth data and perform some basic exploratory data analyses
2. Provide a basic summary of the data.
3. Use confidence intervals and/or hypothesis tests to compare tooth growth by supp and dose. (Only use the techniques from class, even if there's other approaches worth considering)
4. State your conclusions and the assumptions needed for your conclusions.

# Files in the Repository

In addition to this readme file, the repository contains the following files:

* [1_simulation_exercise.pdf](https://docs.google.com/spreadsheets/d/1avGWWl1J19O_Zm0NGTGy2E-fOG05i4ljRfjl87P7FiA/htmlview?ts=5e5e9222&sle=true#gid=0)
* 1_simulation_exercise.Rmd
* 2_inferential_data_analysis.pdf
* 2_inferential_data_analysis.Rmd
