## Overview
NB.MClust uses EM algorithm to group independent samples of multivariate or even high-dimensional data that follows Generalized Negative Binomial density. Variables are assumed to be independent and must be nonnegative. Integers and decimals are allowd as input. Clustering by NB.MClust performs well on the data with overdispersion.

## Example
 Example:
 
 data("Simulated_Count") # A 50x100 integer data frame.
 
 m1=NB.MClust(Simulated_Count,K=2:5)
 
 cluster=m1$cluster #Estimated cluster assignment
 
 k_hat=m1$K  #Estimated optimal K
