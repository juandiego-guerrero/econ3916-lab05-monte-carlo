# econ3916-lab05-monte-carlo
Lab 05 Submission

# Monte Carlo Engine -- Probability & Simulation

## Objective
I used Monte Carlo simulation to see how probability rules play out in practice, from coin flips to portfolio risk.

## Methodology
- Simulated 10,000 fair coin flips and plotted the running share of heads to watch the Law of Large Numbers at work.
- Played 10,000 Monty Hall games under two strategies, always stay and always switch, and compared win rates.
- Applied Bayes' Theorem to a disease screening test (prevalence 1%, sensitivity 95%, specificity 90%), then checked the result by simulating 100,000 people.
- Simulated daily returns for a $1M portfolio and computed Value at Risk and Expected Shortfall at the 95% and 99% levels.
- Estimated pi at increasing sample sizes and checked that the Monte Carlo error shrinks like 1/sqrt(n).
- Asked an AI to write a VaR/ES function, revised my prompt once, and checked its output against my own numbers.

## Key Findings
- The running share of heads was noisy early on and only settled near 0.5 after thousands of flips.
- Switching won [YOUR VALUE] of Monty Hall games, close to the theoretical 2/3.
- Only [YOUR VALUE]% of positive tests came from sick people. When a disease is rare, false positives outnumber true ones.
- On a $1M portfolio, the 95% VaR was $19,889 and the 95% ES was $24,894. On the worst 5% of days, the average loss is well beyond the VaR cutoff.
- Monte Carlo error fell like 1/sqrt(n), so halving the error takes four times as many draws.
