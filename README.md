# Lab-9-Causal-Inference-I-A-B-Testing
A/B Testing — Designing the Data-Generating Process
Objective

I used a randomized job training experiment and a mobile game A/B test to see how random assignment, significance tests, confidence intervals, and power analysis work together to measure a causal effect.

Methodology
Loaded the LaLonde NSW job training experiment (445 people: 185 trainees and 260 controls) and computed the experimental average treatment effect (ATE) as the difference in mean 1978 earnings.
Simulated an observational comparison group to show selection bias, and split the gap into its parts: Observational ATE = True ATE + Selection Bias.
Ran a permutation test with 9,999 shuffles to check whether the ATE could be due to chance.
Computed a bootstrap BCa 95% confidence interval for the ATE.
Ran a power analysis to find the power of the LaLonde study and the sample size needed to detect three different dollar effects.
Applied the same difference in means, permutation test, and bootstrap to the Cookie Cats mobile game A/B test (90,189 players, first gate at level 30 or level 40, Day-1 retention).
Wrote a sample-size function, n_needed(), checked it against the power analysis results, and used it to find how many players a rerun of Cookie Cats would need.
Key Findings
Trainees earned $[YOUR VALUE] more than the control group in 1978 (permutation p = [YOUR VALUE], 95% CI $[YOUR VALUE] to $[YOUR VALUE]).
The simulated observational comparison group gave an ATE of $[YOUR VALUE], which shows how selection bias can flip the sign of an estimate when groups are not randomly assigned.
In Cookie Cats, the retention difference between the two gate positions was [YOUR VALUE] pp (p = [YOUR VALUE]).
A rerun of Cookie Cats would need [YOUR VALUE] players per group to detect that difference with 80% power.
