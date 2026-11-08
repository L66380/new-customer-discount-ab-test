# A/B Testing: 10% Discount for New Customers

## Project Overview
This project investigates whether offering a 10% discount to new customers increases purchase conversion rates. The analysis uses simulated customer data, not a real-world experiment.

## Hypothesis
New customers receiving a 10% discount will have a higher purchase conversion rate than customers receiving no discount.

## Experiment Design
- Group A (Control): No discount
- Group B (Treatment): 10% discount
- Primary metric: Purchase conversion rate
- Guardrail metric: Profit per customer (not available in the simulation)

## Sample Size and Duration
- Required sample: 875 customers per group (1,750 total)
- Statistical power: 80%
- Significance level: 5%
- Estimated duration: 18 days, assuming 100 new customers per day

## Results
| Metric | Group A | Group B |
|---|---:|---:|
| Customers | 885 | 865 |
| Purchases | 79 | 107 |
| Conversion rate | 8.93% | 12.37% |

- Absolute conversion uplift: 3.44 percentage points
- Chi-square p-value: 0.0195
- 95% confidence interval for uplift: 0.55 to 6.33 percentage points
- SRM p-value: 0.6326 (no evidence of sample ratio mismatch)

## Conclusion and Recommendation
Group B achieved a statistically significantly higher conversion rate in the simulated data. However, these findings do not establish real-world business impact. A real customer experiment and profitability analysis are recommended before implementing the discount.

## Tools and Libraries
Python, Google Colab, pandas, NumPy, SciPy, statsmodels, and Matplotlib.

## How to Run
Open the project notebook in Google Colab and select Runtime > Run all. The simulation uses a fixed random seed for reproducibility.