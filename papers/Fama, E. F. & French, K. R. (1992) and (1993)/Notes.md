
# Fama & French (1992): "The Cross‑Section of Expected Stock Returns"

The **Fama & French (1992)** paper shows that firm size and the **book‑to‑market equity ratio** (how much the company is worth on paper vs. how much the market thinks it is worth) explain most of the cross‑sectional variation in U.S. stocks.

The authors form portfolios based on beta, size, leverage, B/M, and earnings‑price ratios. They use the **Fama–MacBeth regression** (1973) to run these cross‑sectional tests.

## The Two-Step Process

### Step 1: The Time‑Series Step

We first determine how sensitive each asset  is to a specific factor by running a regression for every single asset in the sample over time .

**Variables:**

* : Return of asset  at time .
* : The **factor loading** (how much the asset moves with the factor).
* : The intercept (mispricing).

The result is an estimate of  for every asset, which we treat as a known variable for the next step.

---

### Step 2: The Cross‑Sectional Step

Next, we test if assets with higher betas actually earn higher average returns. Instead of regressing over time, we regress **across all assets** at each individual time period .

**Variables:**

* : The **risk premium** for that specific month or day.
* : The beta estimate we saved from Step 1.

This provides a **time series** of risk premiums ().

---

### Step 3: Average Risk Premium

Finally, we average those risk premiums to determine if the factors explain returns over the long term.

If  is statistically significant (based on a t-test), then the factor is considered a valid driver of cross‑sectional returns.


