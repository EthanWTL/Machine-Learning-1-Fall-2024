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

 $$log(\frac{p}{1-p}) = \beta_0 + \beta_1X_1 + \beta_2X_2 + ... + \beta_kX_k$$

 Where $\beta_0, \beta_1, \beta_2, ..., \beta_k$ are coefficients, $X_1, X_2,..., X_k$ are the variables, $p$ is the success probability of the dependent variables.
 
 ## c. Example of ```Logit Transformation``` 
 We write logistic regression of whether patient have a certain disease in the following form
 
 $$log(\frac{p}{1-p}) = -5 + 0.04Age + 0.2Cholesterol$$

 Now, if $Age$ is increased by 1, the log odds of having the disease in increased by 0.04

 $$Odds Ratio = e^{0.04} = 1.04$$

 This tells us if the age grow up 1 year, then the odds will increase by 4%.

 If the odds of having a disease is 50%, which is $\frac{p}{1-p} = 0.5$ or $1:2$ which means the probability is 33.3% right now. 

 If the age increase by 1, then the new Odds is going to be $50\\% * 1.04 = 52\\%$, now we get,

 $$\frac{p}{1-p} = 0.52$$

 so the new probability of having this disease after one year older is $35.13\\%$.

 ## d. Paper Selection
 * [Decentralized Machine Learning Approach on ICU Admission Prediction for Enhanced Patient Care Using COVID-19 Data](https://dergipark.org.tr/en/pub/pims/issue/81233/1390925), Tianlong Wang, Takeshi Matsuda, Mehmet DIK

 Left Hand Side: Shall a patient got admitted into ICU?
 
 Right Hand Side: clinical data (sex, gender,...) + disease history information (Pneumonia, diabetes,...).
 
---
# 2. Expectation
## a. For discrete variable $Y$
For variable $y_1,y_2,y_3,...,y_k$ and corresponding probability $p_1,p_2,p_3,...,p_k$, the expected value is defined:

$$
E(Y) = \sum_{k=1}^{n}y_k \cdot p_k
$$

## b. For continues random variable $Y$
For continues variable $Y$ with probability density function $f(y), the expectation is:

$$
E(Y) = \int_{-\infty}^{\infty} y \cdot f(y) \, dy
$$

## c. Examples
```Normal Distribution``` Consider $Y$ follows normal distribution $N(\mu,\sigma^2)$, the Expected value of normal distribution is:

$$
E(Y) = \mu
$$

```Gamma Distribution``` Consider $Y$ follows Gamma distribution with Shape Parameter $k$ and Rate Parameter \theta, then the expected value is:

$$
E(Y) = k\theta
$$



--- 
# Acknowledgments:

* [PennState Eberly College of Science](https://online.stat.psu.edu/stat462/node/207/)
* [Journal of Uncertain Systems, Vol1 No3, 2007, August, World Academic Union (World Academic Press)](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=e348ebb8e669c385ef2819343e98af2399701135)
