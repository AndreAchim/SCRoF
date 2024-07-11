# SCRoF
Signal Cancellation Recovery of Factors: Matlab code

Two commands, each with two forms:
1) out=SCRoF(data)
 or out=SCRoF(R,N) where out is the name for a structure containing intermediate and final results
2) SCRoF(out) displays in descending ordre of fit probability the scenarios explored.
  First 3 columns are p, X^2 and d.f.; next 3 are scenario branches, respectiely about inclusion/exclusion
  of borderline orphan variables, possible factor structures, and nullable factor correlations
 or SCRoF(out,k), where k is a scenario rank. Thisprints the pattern matrix and factor correlation matrix
  and draws the dendrogram of variable clustering from pairwise signal cancellation. The umber of factors will be
  the number of cluaters of variable subsets that can mutually cancel their signal MINUS the clusters that are found
  coplanar with two other clusters (of the 3 clusters, the most orthogonal pair is retained as factors)   
  All scenarios with non-significant X^2 fit are worth reporting, although parcimony prefers a scenario with fewer factors.

For a 40 minute video presentation, see https://achim.uqam.ca/SCRoF.mp4
