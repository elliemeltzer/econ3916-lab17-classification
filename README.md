# Classification: When 90% Accurate Is Worthless

## Objective

I examined why accuracy can be misleading when loan defaults are uncommon and chose a decision threshold based on financial costs.

## Methodology

- Simulated 6,000 loan applications with a 9.6% default rate.
- Fitted and interpreted a logistic regression.
- Compared precision and recall across thresholds.
- Selected a threshold using false-positive and false-negative costs.
- Checked probability calibration.

## Key Findings

Approving everyone was 90.4% accurate, and the model also achieved 90.4% accuracy at the usual 0.5 threshold while predicting zero defaults. One additional prior default multiplied the odds by 1.63. The cost-minimizing threshold was 0.121, close to the closed-form value of 0.118. It reduced expected cost from $1,147 to $944 per applicant. At the closed-form threshold, precision was 0.181 and recall was 0.477. The original probabilities were reasonably calibrated.
