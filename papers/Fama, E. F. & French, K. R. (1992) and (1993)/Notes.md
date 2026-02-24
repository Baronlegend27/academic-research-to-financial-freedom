# Fama & French (1992): *The Cross-Section of Expected Stock Returns*

The **Fama & French (1992)** paper *“The Cross-Section of Expected Stock Returns”* is one of the most influential empirical studies in asset pricing. In this work, Eugene F. Fama and Kenneth R. French examine how characteristics of stocks relate to their average returns, extending beyond what the traditional Capital Asset Pricing Model (CAPM) predicts. They find that two simple, measurable firm characteristics, size (market capitalization) and book-to-market equity, explain a large portion of the cross-sectional variation in average stock returns. Specifically:

- Stocks of **smaller firms** tend to earn higher average returns than those of larger firms.  
- Firms with a **high book-to-market ratio** (often interpreted as *value* stocks) also tend to earn higher returns than low book-to-market (or *growth*) stocks.

These results show that the relationship between return and *beta* (as predicted by CAPM) is weak once size and book-to-market effects are allowed to vary, suggesting that these additional factors provide important explanatory power for stock returns.

---

# Fama & French (1993): *Common Risk Factors in the Returns on Stocks and Bonds*

The **Fama & French (1993)** paper identifies common risk factors that help explain the average returns on both stocks and bonds. While the earlier three-factor model focused primarily on stocks, this study extends the multifactor approach to **both financial markets**, emphasizing that variations in returns can be captured by a few systematic risk factors. 

he authors construct portfolios based on multiple characteristics including beta, size, leverage, book-to-market equity, and earnings-price ratios and then apply the **Fama–MacBeth two-stage regression** method to examine how these characteristics relate to expected returns across assets.

## The Two-Step Process

### Step 1: The Time-Series Step

We first determine how sensitive each asset is to a specific factor by running a regression for every single asset in the sample over time.

**Variables:**
- $R_{i,t}$: Return of asset $i$ at time $t$  
- $\beta_{i,F}$: The **factor loading** (how much the asset moves with the factor)

The result is an estimate of $\beta$ for every asset, which we treat as a known variable for the next step.

$$R_{i,t} - R_{f,t} = \alpha_i + \beta_{i,F1} \cdot F1_t + \beta_{i,F2} \cdot F2_t + \beta_{i,F3} \cdot F3_t + \varepsilon_{i,t}$$

---

### Step 2: The Cross-Sectional Step

Next, we test if assets with higher betas actually earn higher average returns. Instead of regressing over time, we regress **across all assets** at each individual time period $t$.

**Variables:**
- The **risk premium** $\lambda_{1,t}$ for that specific month or day  
- The beta estimate we saved from Step 1

This provides a **time series** of risk premiums $\lambda_{1,t}$.

$$R_{i,t} = \lambda_{0,t} + \lambda_{1,t}\,\beta_{i,F} + \varepsilon_{i,t}$$

---

### Step 3: Average Risk Premium

Finally, we average those risk premiums to determine if the factors explain returns over the long term.

$$
\bar{\lambda}_{1}
= \frac{1}{T} \sum_{t=1}^{T} \lambda_{1,t}
$$

If $\bar{\lambda}_{1}$ is statistically significant (based on a t-test), then the factor is considered a valid driver of cross-sectional returns.
