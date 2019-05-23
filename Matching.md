Return to [[Methods]]

[[_TOC_]

## Related to

### Coarsened exact matching (cem)
* [[Blackwell et al 2009]]

#### Example
* [[Younge Tong and Fleming 2015]]

### Propensity score matching (PSM)
* [[Imbens 2000]]
* [[Rosenbaum and Rubin 1983]]

#### Example
* [[Love Lim and Bednar 2017]]

### Courses etc.
* [[Special Topics in Statistics 2018]]: Sessions 3 & 4

## One-paragraph summary
Matching is not just a modeling method, instead, it can also be an approach to constructing a sample. In older articles, the author might also forgo controlling for covariates completely (e.g., Imbens 2000), only including the propensity score. When matching, instead of using the full dataset, we limit the dataset to treated cases, and those cases from the control group that are most similar to the treated cases - in terms of the other variables that are available to us. The advantage of this approach is that (ideally) we do not have to extrapolate from the existing data too much, as is the case when we use lines of best fit (OLS) to compare observations with vastly different magnitudes in some variables. For instance, if the treatment group had systematically higher income than the control group, an OLS estimation would fit a line, and use the gradient to control for the effect of income. This can negatively affect the accuracy of the estimated model, for instance if some extreme outliers have high leverage on the model. Matching would allow us to limit the sample to similar observations, thereby alleviating the effect of systematic differences between treatment group and control group. On the other hand, matching does not use the full sample, therefore, we are losing some statistical power.

### Matching methods
* **Exact Matchig**: Exact matching matches each observation from the treatment group to one observation of the control group. Usually not possible if the sample includes continuous variables.

* **Coarsened Exact Matching**: Similar to exact matching, but continuous variables are separated into "buckets" to enable an approximate form (coarsened) of exact matching.

* **Propensity Score Matching**: Instead of using exact matches, the covariates are used to calculate the likelihood that an observation will be "selected into" treatment or not. Then, each observation in the treatment group is matched to the observation in the control group that has the closest propensity score (score that determines the likelihood to receive treatment.

### Caveat
All three matching methods still constitute selection on observables (SOO). If there is still an exogenous variable that affects the likelihood to be selected into treatment, the endogeneity problem persists.