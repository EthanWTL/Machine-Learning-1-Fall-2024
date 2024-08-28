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
 
 ## c. Example of ```Logit Transformation``` 
 We write logistic regression of whether patient have a certain disease in the following form
 
 $log(\frac{p}{1-p}) = -5 + 0.04Age + 0.2Cholesterol$

 Now, if $Age$ is increased by 1, the log odds of having the disease in increased by 0.04

 $Odds Ratio = e^{0.04} = 1.04$

 This tells us if the age grow up 1 year, then the odds will increase by 4%.

 If the odds of having a disease is 50%, which is $\frac{p}{1-p} = 0.5$ or $1:2$ which means the probability is 33.3% right now. 

 If the age increase by 1, then the new Odds is going to be $50\\% * 1.04 = 52\\%$, now we get,

 $\frac{p}{1-p} = 0.52$

 so the new probability of having this disease after one year older is $35.13\\%$.

 
---
# 2. Expectation






--- 
# Acknowledgments:

* [PennState Eberly College of Science](https://online.stat.psu.edu/stat462/node/207/)
