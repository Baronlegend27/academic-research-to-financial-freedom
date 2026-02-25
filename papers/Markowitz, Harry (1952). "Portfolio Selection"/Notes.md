## Markowitz, Harry (1952). "Portfolio Selection"

In his 1952 paper Portfolio Selection, Harry Markowitz introduced what became known as Modern Portfolio Theory (MPT), fundamentally changing how investors think about risk, return, and diversification.
He made a model formalizes how to choose an optimal investment portfolio by balancing expected return against risk, where risk is measured by variance of returns.



\[
E(R_p) = \sum_{i=1}^{n} w_i \cdot E(R_i)
\]


\[
\sigma_p^2 = \sum_{i=1}^{n} \sum_{j=1}^{n} w_i w_j \cdot \text{Cov}(R_i, R_j)
\]

Markowitz’s framework also formalized the role of covariance and correlation between asset returns. He showed that the risk of a portfolio depends not just on the risk of individual assets but on how those assets move together.

\[
\min_{\mathbf{w}} \quad \mathbf{w}^T \boldsymbol{\Sigma} \mathbf{w}
\]


A core concept introduced in Portfolio Selection is the efficient frontier — the set of portfolios that offer the best possible trade‑off between risk and return. Portfolios on this frontier are “efficient” because no other portfolio can provide a higher expected return without increasing risk. Markowitz demonstrated mathematically how diversification can reduce overall portfolio risk by combining assets with different return patterns and correlations. This shift in focus from individual securities to the interaction of assets within a portfolio was revolutionary

Subject to:
\[
\mathbf{1}^T \mathbf{w} = 1
\]
\[
\boldsymbol{\mu}^T \mathbf{w} = \mu_p
\]
