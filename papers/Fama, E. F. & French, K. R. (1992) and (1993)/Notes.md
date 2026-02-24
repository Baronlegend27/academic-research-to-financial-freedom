# Fama & French (1993): *Common Risk Factors in the Returns on Stocks and Bonds*

The **Fama & French (1993)** paper shows that firm size and the **book-to-market equity ratio** (how much the company is worth on paper vs. how much the market thinks it is worth) explain most of the cross-sectional variation in U.S. stocks.

The authors form portfolios based on beta, size, leverage, B/M, and earnings-price ratios. They use the **Fama–MacBeth regression** (1973) to run these cross-sectional tests.

## The Two-Step Process

### Step 1: The Time-Series Step

We first determine how sensitive each asset is to a specific factor by running a regression for every single asset in the sample over time.

**Variables:**

- $R_{i,t}$: Return of asset $i$ at time $t$  
- $\beta_{i,F}$: The **factor loading** (how much the asset moves with the factor)

The result is an estimate of $\beta$ for every asset, which we treat as a known variable for the next step.

$$
R_{i,t} - R_{f,t}
= \alpha_i
+ \beta_{i,F1} \cdot F1_t
+ \beta_{i,F2} \cdot F2_t
+ \beta_{i,F3} \cdot F3_t
+ \varepsilon_{i,t}
$$

---

### Step 2: The Cross-Sectional Step

Next, we test if assets with higher betas actually earn higher average returns. Instead of regressing over time, we regress **across all assets** at each individual time period $t$.

**Variables:**

- The **risk premium** $\lambda_{1,t}$ for that specific month or day  
- The beta estimate we saved from Step 1

This provides a **time series** of risk premiums $\lambda_{1,t}$.


$$
R_{i,t}
= \lambda_{0,t}
+ \lambda_{1,t}\,\beta_{i,F}
+ \varepsilon_{i,t}
$$

---

### Step 3: Average Risk Premium

Finally, we average those risk premiums to determine if the factors explain returns over the long term.

$$
\bar{\lambda}_{1}
= \frac{1}{T} \sum_{t=1}^{T} \lambda_{1,t}
$$

If $\bar{\lambda}_{1}$ is statistically significant (based on a t-test), then the factor is considered a valid driver of cross-sectional returns.
