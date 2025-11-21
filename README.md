# Q-Variance Challenge

Can any continuous-time stochastic-volatility model reproduce the parabolic relationship  
σ(z) = √(σ₀² + z²/2)  
across 8 assets and all horizons 1-26 weeks with R² ≥ 0.92 and ≤ 2 free parameters?

Here z = x/sqrt(T) where x is the log price change over a period T, adjusted for drift.
Read the paper Q-Variance_Wilmott_July2025.pdf for more details.

Quantum baseline (Orrell 2025): R² ≈ 0.95

Repository contains:
- Full dataset generator (data_loader.py)
- Scoring engine
- Live leaderboard
- Baseline quantum fit

Frequently Asked Questions

Q: Is q-variance a well-known "stylized fact"?
A: No, a stylized fact is just a general observation about market data, as opposed to a firm prediction. Q-variance is a falsifiable prediction because the multiplicative constant on the quadratic term is not a fit, it is set by theory at 0.5. The same formula applies for all period lengths T.

Q: Is q-variance a large effect?
A: Yes, the minimum variance is about half the total variance so this is a large effect.

Q: Has q-variance been previously reported in the literature?
A: Not to our knowledge, and we have asked many people, but please bring any references to our attention. This is strange because as mentioned it is a large effect.

Q: Does q-variance have implications for finance?
A: Yes, it means that standard formulas such as the Black-Scholes model or the model used to calculate VIX will not work as expected?

Q: Is q-variance replated to the implied volatility smile?
A: Yes, but it is not the same thing because it applies to realized volatility.

Q: Can I use AI for the challenge?
A: Yes, AI entries are encouraged.
