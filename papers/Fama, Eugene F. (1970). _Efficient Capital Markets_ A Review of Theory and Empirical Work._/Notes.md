# Efficient Capital Markets: A Review of Theory and Empirical Work

The paper **Fama, Eugene F. (1970). Efficient Capital Markets: A Review of Theory and Empirical Work** defined **efficiency** as the idea that prices fully reflect all available information.

Fama took a messy, scattered set of ideas about markets and turned them into a **disciplined scientific framework**. He organized the market efficiency concept into **three forms**:

1. **Weak-form efficiency** – Does the price reflect past information?  
2. **Semi-strong form efficiency** – Does the price reflect all public information?  
3. **Strong-form efficiency** – Do prices reflect all information, including private or insider information?

Fama stated:

> "If markets process information correctly, then prices must behave like a particular process."

This was **extremely important** because it provided a rigorous stochastic foundation, allowing empirical testing using decades of mathematical frameworks and statistical tools.

## Key Insights from Fama's Work

- If all available information is reflected in today's prices, then **only new information can move prices**.
- New information is **unpredictable**, so price changes should also be unpredictable.
- The **best forecast for tomorrow's price is today's price** because prices are informationally efficient.
- Returns should follow a **fair game property**, meaning:
  - Investors cannot systematically earn abnormal profits using information everyone already knows.
  - Expected gain after adjusting for risk is zero.
  - Investors can earn normal risk-adjusted returns, but **abnormal returns are impossible** from publicly available information.

$$E[P_{t+1} \mid \text{information at time } t] = P_t$$

---

### Martingale

An **efficient market behaves like a martingale**, where future price changes are random and cannot be predicted from past or public information.

A **martingale** is a mathematical model used to describe the evolution of prices in an efficient market. It formalizes the idea that the **expected future price of an asset, given all information available today, is equal to its current price**:

$$E[P_{t+1} \mid P_t, P_{t-1}, \dots] = P_t$$

The fair game property applies to returns, while the martingale property applies to prices; they are closely related and often interchangeable. A fair game in returns implies a martingale in prices.

Prices in an efficient market can also be described as following a **random walk**, meaning that changes in price are independent and unpredictable, driven only by new information.

---

### Testing Weak-Form Efficiency

To test **weak-form efficiency**, we use historical price data. One common method is a regression of future returns on past returns:

$$R_{t+1} = \alpha + \beta R_t + \epsilon$$

- **β = 0** → returns are unpredictable → fair game holds → weak-form efficiency  
- **β ≠ 0** → returns are predictable → weak-form inefficiency  

---

### Testing Semi-Strong Form Efficiency

To test **semi-strong efficiency**, we need:  
- Stock price data around the time of public announcements (such as earnings reports, dividends, or mergers)  
- The exact dates of these announcements  
- Market index data to calculate expected returns  

We calculate **abnormal returns (AR)** for each day in the event window:

$$AR_t = R_t - E(R_t)$$

**Where:**

| Symbol | Meaning |
|--------|---------|
| $AR_t$ | Abnormal return on day $t$ |
| $R_t$ | Actual return on day $t$ |
| $E(R_t)$ | Expected return based on a market model or historical data |

If the market is efficient, the abnormal return should be zero immediately after the news is released.

Often, we sum abnormal returns over an **event window** (e.g., -1 to +1 days around the announcement) to see the total effect. This is called the **Cumulative Abnormal Return (CAR)**:

$$CAR = \sum_{t=-1}^{+1} AR_t$$

**Where:**

| Symbol | Meaning |
|--------|---------|
| $CAR$ | Total cumulative abnormal return over the event window |
| $t = -1$ | Day before the announcement |
| $t = 0$ | Day of the announcement |
| $t = +1$ | Day after the announcement |

The CAR measures the **total impact of the announcement on the stock price**. If the market is semi-strong efficient, CAR should be close to zero immediately after the news is incorporated.

---

### Testing Strong-Form Efficiency

Fama described **strong-form efficiency** as a market where prices fully reflect **all information, including private or insider information**. To test this, researchers examine whether **insiders or those with private knowledge can earn abnormal returns**. Typically, this involves comparing the returns earned by insiders, such as corporate executives or directors, to normal market returns.

- If insiders cannot consistently achieve excess profits, the market satisfies strong-form efficiency.
- If insiders earn systematic abnormal returns, strong-form efficiency is violated.
