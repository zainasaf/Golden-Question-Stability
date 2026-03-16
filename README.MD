This repository contains the R script used to assess the temporal stability of "golden questions".

The analysis examines whether the distribution of responses to these questions remains consistent over time, distinguishing genuine shifts in public opinion from statistical noise due to sampling variation.

Response Coding Because the focus is on directional stability (rather than intensity), response categories were grouped by directional leaning:

Four-point scales: Responses 1–2 (one direction) vs. 3–4 (opposite direction) Descriptive items: "Describes me very/quite well" vs. 
"Does not describe me particularly/at all" Other scale types (true/false, immigration, left-right grid, six-point, engagement) are handled separately

Statistical Tests Four formal tests are applied to each golden question:

Chi-Square Test of Homogeneity Tests whether the distribution of responses is identical across all polls. A significant result (p < 0.05) 
indicates variation beyond what would be expected from sampling error alone.
Cramér's V (Effect Size) Because large sample sizes (~2,000 respondents × 48 surveys) can make chi-square tests sensitive to trivial differences, 
Cramér's V is calculated alongside each chi-square result. This provides a scale-independent measure of association strength (0 = no association, 1 = perfect association).
Variance / Standard Deviation Test Tests whether the standard deviation of response percentages across surveys exceeds a threshold of 2.5 percentage points (the null hypothesis). 
Questions where SD is not significantly greater than 2.5pp are classified as Stable; those where it is are classified as Unstable.
Pairwise Comparison Test For each question, all possible pairs of polls are compared. The number of pairs exceeding absolute differences of 5, 10, and 20 percentage points is reported,
providing a concrete measure of variability.
All golden questions except one showed high stability across the 48 surveys. The exception was lr_grid_3 ("Ordinary working people don't get a fair share of the nation's wealth"),
which exhibited substantial variation: This is because prior to July, this question was somtimes asked "Ordinary peope DO get a fair share of the nation's wealth".
