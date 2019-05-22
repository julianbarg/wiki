Return to [[Methods]]

## 

Matching is not a modeling method, instead, it is an approach to constructing a sample. Instead of using the full dataset, we limit the dataset to treated cases, and those cases from the control group that are most similar to the treated cases - in terms of the other variables that are available to us. The advantage of this approach is that (ideally) we do not have to extrapolate from the existing data too much, as is the case when we use lines of best fit (OLS) to compare observations with vastly different magnitudes in some variables. For instance, if the treatment group had systematically higher income than the control group, an OLS estimation would fit a line, and use the gradient to control for the effect of income. This can negatively affect the accuracy of the estimated model, for instance if some extreme outliers have high leverage on the model. Matching would allow us to limit the sample to similar observations, thereby alleviating the effect of systematic differences between treatment group and control group. On the other hand, matching does not use the full sample, therefore, we are losing some statistical power.

Exact Matching

Coarsened Exact Matching

Propensity Score Matching

Matching is still selection on observables (SOO).