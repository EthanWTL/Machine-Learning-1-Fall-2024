# 8/29 😀
# 1. Log Odds
## a. Probability, Odds, Log-Odds
Here is a quick comparision between three terms.
| Terminology  | Description | Equation |
| ------------- | ------------- | -------|
| Probability | The probability that an event happens |  $p$ |
| Odd (Odd of success)  | Probability of success / Probability of failure | $\frac{p}{1-p}$ |
| Log-Odds | logarithm of the odds | $log(\frac{p}{1-p})$ |

## b. Logistic Regression
Log Odds provides an alternate expression for logistic regression

 $log(\frac{p}{1-p}) = \beta_0 + \beta_1X_1 + \beta_2X_2 + ... + \beta_kX_k$

 Where $\beta_0, \beta_1, \beta_2, ..., \beta_k$ are coefficients, $X_1, X_2,..., X_k$ are the variables, $p$ is the success probability of the dependent variables.
 
 ```Logit Transformation``` 

 $log(\frac{have disease}{1-have disease}) = -5 + 0.04Age + 0.2Cholesterol$

 
---
# 2. Expectation






--- 
# Acknowledgments:

* [PennState Eberly College of Science](https://online.stat.psu.edu/stat462/node/207/)
