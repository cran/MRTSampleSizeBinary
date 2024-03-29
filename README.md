# MRTSampleSizeBinary

This package provides a sample size calculator for Micro-randomized Trials with
binary outcomes, based on the following article. Cohn, E. R., Qian, T., & Murphy, S. A. (2023). Sample size considerations for micro‐randomized trials with binary proximal outcomes. Statistics in Medicine.

Before using the calculator the user should have knowledge of the following:

1. **Study Setup**
The number of decision time points and the randomization
probability, i.e. the probability of assigning the treatment at each decision
time point.

1. **Availability** 
Treatment can only be provided when an individual is
available. The expected availability is the probability a person is available to
receive the intervention at the decision times. You need to select a
time-varying pattern for the expected availability.

1. **Success Probability Null Curve** 
The Success Probability Null Curve at
each decision time point is defined as the probability of the proximal outcome
equal to 1 for available individuals who are not assigned treatment. You need to
provide the trend of success probability null curve.

1. **Proximal Treatment Effect**
The Proximal Treatment Effect at each decision
time point is defined as the mean difference in the proximal outcome between
available people who are assigned a treatment versus available people who are
not assigned treatment. In this work, we only consider the binary treatment. You
need to provide the trend of proximal treatment effects.

The outputs one can get using this package are mainly two values, power and
sample size. In both cases, you will need to input the desired significance
level.