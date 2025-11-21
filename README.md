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

AI entries encouraged.

