# Fama & French (1992) — Markdown + LaTeX Version (Full Text Included)

The Fama & French (1992) paper shows that firm size and the book‑to‑market equity ratio (how much the company is worth on paper vs. how much the market thinks the company is worth) explain most of the cross‑sectional variation in U.S. stocks.

The authors form portfolios based on beta, size, leverage, B/M, and earnings‑price ratios, then run cross‑sectional tests to get this result. They use the Fama–MacBeth regression, which was formulated in 1973, to run these cross‑sectional tests.

These tests consist of first determining how sensitive each asset \( i \) is to a specific factor for every single asset in the sample over time \( t \).

### Time‑Series Step (in LaTeX)



\[
R_{i,t} = \alpha_i + \beta_{i,F} F_t + \varepsilon_{i,t}
\]



Where:

- \( R_{i,t} \): return of asset \( i \) at time \( t \)  
- \( \beta_{i,F} \): the factor loading (how much the asset moves with the factor)

The result is that you end up with an estimate of \( \beta \) for every asset.

---

Now we want to see if assets with higher betas actually earn higher average returns. Instead of regressing over time, we regress **across all assets** at each time period \( t \).

### Cross‑Sectional Step (in LaTeX)



\[
R_{i,t} = \gamma_{0,t} + \gamma_{1,t} \hat{\beta}_{i,F} + \eta_{i,t}
\]



Here:

- \( \gamma_{1,t} \) is the risk premium for that specific month/day.

This gives us a **time series** of risk premiums.

---

Finally, we average those risk premiums to see if the factors actually “explain” returns over a long period.

### Average Risk Premium (in LaTeX)



\[
\bar{\gamma}_1 = \frac{1}{T} \sum_{t=1}^{T} \gamma_{1,t}
\]



If \( \bar{\gamma}_1 \) is statistically significant, then the factor helps explain cross‑sectional returns.

