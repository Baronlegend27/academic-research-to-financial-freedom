## Markowitz, Harry (1952). "Portfolio Selection"

In his 1952 paper *Portfolio Selection*, Harry Markowitz introduced what became known as **Modern Portfolio Theory (MPT)**, fundamentally changing how investors think about risk, return, and diversification. His model formalizes how to choose an **optimal investment portfolio** by balancing expected return against risk, where risk is measured by the **variance of returns**.

---

### Portfolio Expected Return

The expected return of a portfolio is the **weighted average of individual asset returns**:

$$E(R_p) = \sum_{i=1}^{n} w_i \cdot E(R_i)$$

| Symbol | Meaning |
|--------|---------|
| $E(R_p)$ | Expected return of the portfolio |
| $w_i$ | Weight of asset $i$ in the portfolio |
| $E(R_i)$ | Expected return of asset $i$ |
| $n$ | Number of assets in the portfolio |

---

### Portfolio Variance (Risk)

Markowitz showed that portfolio risk depends not just on individual asset risk, but on **how assets move together** (covariance). The portfolio variance is:

$$\sigma_p^2 = \sum_{i=1}^{n} \sum_{j=1}^{n} w_i w_j \cdot \text{Cov}(R_i, R_j)$$

| Symbol | Meaning |
|--------|---------|
| $\sigma_p^2$ | Variance (risk) of the portfolio |
| $w_i, w_j$ | Weights of assets $i$ and $j$ |
| $\text{Cov}(R_i, R_j)$ | Covariance between returns of asset $i$ and asset $j$ |

This formalizes **diversification** — combining assets with low or negative covariance reduces overall portfolio risk, even if individual assets are risky.

---

### The Efficient Frontier

A core concept introduced in *Portfolio Selection* is the **efficient frontier** — the set of portfolios that offer the best possible trade-off between risk and return. Portfolios on this frontier are *efficient* because no other portfolio can provide a higher expected return without increasing risk.

Markowitz demonstrated mathematically how diversification can reduce overall portfolio risk by combining assets with **different return patterns and correlations**. This shift in focus from individual securities to the **interaction of assets within a portfolio** was revolutionary.

---

### The Optimization Problem

To find the efficient frontier, Markowitz formulated a **constrained optimization problem** — minimize portfolio variance for a given target return:

**Minimize:**

$$\min_{\mathbf{w}} \quad \mathbf{w}^T \boldsymbol{\Sigma} \mathbf{w}$$

**Subject to:**

$$\mathbf{1}^T \mathbf{w} = 1$$

$$\boldsymbol{\mu}^T \mathbf{w} = \mu_p$$

| Symbol | Meaning |
|--------|---------|
| $\mathbf{w}$ | Vector of portfolio weights |
| $\boldsymbol{\Sigma}$ | Covariance matrix of asset returns |
| $\mathbf{1}^T \mathbf{w} = 1$ | Weights must sum to 1 (fully invested) |
| $\boldsymbol{\mu}^T \mathbf{w} = \mu_p$ | Portfolio must achieve target return $\mu_p$ |
