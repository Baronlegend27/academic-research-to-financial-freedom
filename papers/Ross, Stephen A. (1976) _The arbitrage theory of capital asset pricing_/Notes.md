## Arbitrage Theory of Capital Asset Pricing (1976)

The Arbitrage Pricing Theory (APT), developed by Stephen Ross in 1976, says that if there are no arbitrage opportunities in the market, asset returns must follow a linear factor structure. If two portfolios have the same risk, they must offer the same expected return; otherwise, investors could earn risk-free profits. Because APT relies only on the no-arbitrage assumption, it is more realistic than earlier asset pricing model

---

### Decomposition of Returns

Ross uses a basic probability identity for any random variable to explain where returns come from:

$$
X = \mathbb{E}[X] + (X - \mathbb{E}[X])
$$

This separates a variable into its expected part and its unexpected component.

$$
R = \mathbb{E}[R] + (R - \mathbb{E}[R])
$$

Thus, returns consist of:

- **Expected return**: $\mathbb{E}[R]$
- **Unexpected return**: $R - \mathbb{E}[R]$
The unexpected return is the surprise return that comes from new information. The unexpected return is the only part that moves prices day to day.
The expected return is what the investor thought they would earn on average. 

The unexpected return decomposes as:

$$
R - \mathbb{E}[R] = \beta_{i1}F_1 + \beta_{i2}F_2 + \cdots + \beta_{ik}F_k + \varepsilon_i
$$

Where:
- $F_j$ is a **factor**, which is a systematic source of market wide risk that influences returns. Some common factors include interest rates, commodity prices, and tax policy.
- $\beta_{ij}$ is the **factor loading** which measures how sensitive a stock is to a change in factor $j$.
- $\varepsilon_i$ is the **idiosyncratic risk** of a single stock (the error term)

---

The expected return is given by:

$$
\mathbb{E}[R] = R_f + \beta_{i1}\lambda_1 + \beta_{i2}\lambda_2 + \cdots + \beta_{ik}\lambda_k
$$

Where:
- $R_f$ is the **risk-free rate**
- $\beta_{ij}$ is the **factor loading** for asset $i$ on factor $j$ 
- $\lambda_j$ is the **risk premium** for factor $j$ which is the extra return the market offers for being exposed to one unit of risk from that factor

A larger $\beta_{ij}$ for a specific factor means the asset's return is more sensitive to economic shocks from that factor.

In an ideal market, $\lambda_j$ is the same for all assets, meaning the only way for an asset to earn higher returns is to have higher factor sensitivity.

---

### Factors and Linear Pricing

APT does not specify the exact factors but requires their existence. Using the no‑arbitrage condition, Ross shows that asset prices follow a linear structure. Even without knowing the factors, APT implies that expected returns are a linear combination of them, providing a testable prediction. It also introduced the concept that multiple systematic factors can drive asset returns, paving the way for multifactor models like Fama–French.
