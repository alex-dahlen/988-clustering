# 988-clustering
Code and data to accompany ""Preferred Sources For Suicide Prevention And Crisis Services Among Segments Of The US Adult Population".

Results were weighted by the survey weights were provided by Ipsos to generate nationally representative estimates of the U.S. adult population.  Missing data were rare (1.9% of responses for psychological distress score; 0.4% of responses about political party; and less than 0.8% for each question about sources of support), and were imputed using Multiple Imputation by Chained Equations (MICE).   The 95% confidence intervals combine the Bernoulli standard error across imputations using Rubin’s rules.

For the audience segmentation, we used a Latent Class Analysis (LCA) to cluster the survey respondents in terms of which sources of support they were “very likely” and “very unlikely” to reach out to in a crisis, for a total of 10 binary features.  We used a Full Information Maximum Likelihood (FIML) to average over the (rare) missing survey responses.  The optimal number of clusters was chosen to optimize the cross-validated log-likelihood.
