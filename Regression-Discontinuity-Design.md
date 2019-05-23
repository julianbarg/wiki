Return to [[Methods]]

[[_TOC_]]

## Related to

### Seminal papers
* [[Imbens and Lemieux 2008]]
* [[Gelman and Imbens 2017]]

### Example
* [[Cunat Gine and Guadalupe 2012]]
* [[Flammer and Bansal 2017]]

### One-paragraph summary
To ensure that treatment is assigned as good as random (no selection on unobservables), a quasi-natural experiment is devised. To carry out this RDD study, one needs to identify an administrative decision with clear rules as to who will be affected, e.g., decided by a cutoff value ([[Imbens and Lemieux 2008]]). For instance, one might look at the outcome of a measure that is applied only to students in a certain age group at a specific point in time. Then, one limits the dataset to only those observations that are either slightly above or below the threshold. For example, if a measure requires a majority vote, one could choose the bracket from 49.5% to 50.5%, 49% to 51% or similar thresholds. Then, it is assumed that the assignment into treatment group or control group is approximately random because the two groups are not very dissimilar to each other with regards to the independent variable that assigns treatment. Whether an observation is in either of these groups is determined by various minuscule factors that are not systematic but quasi-random. After the two groups are determined, a regression is run with a fully specified model, including all covariates that might affect the dependent variable.