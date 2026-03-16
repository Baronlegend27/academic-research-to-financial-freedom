# The Relationship Between Return and Market Value of Common Stocks

The author of this paper wanted to test if the market beta was truly the only thing that explained the differences in returns between stocks.

He used market data from 1936 to 1976, using the market capitalization of each stock at the start of every month to determine its size, and then tracked the stock’s subsequent monthly returns.

During this time the CAPM model said that the difference in returns was due to the different betas of stocks.

The beta is basically how sensitive a stock is relative to the market. Mathematically it is the covariance of the market returns and the individual stock.

Positive beta means that the stock moves with the market and negative beta means it moves in the opposite direction.

Beta = 1 means if the market goes up 1% then the stock goes up 1%.

If beta is higher than 1 like beta = 2 then if the market moves 1% the stock moves 2%.

Then if beta = 0.5 and the market goes down 10% then the stock only goes down 5%.

Market value, also called market capitalization, is the total value of a company’s outstanding shares of stock, calculated as the stock price multiplied by the number of shares.

Banz sorts NYSE stocks into market‑value deciles and finds that the smallest decile (Decile 1) earns significantly higher average returns than predicted by the CAPM, with excess returns relative to the largest firms ranging roughly from 4% to 8% per year, depending on the period and specification. In contrast, the largest decile (Decile 10) has the lowest average returns and shows essentially no size premium. 

 **The effect is highly non-linear:** almost all of the premium comes from the very smallest firms, while medium and large firms exhibit little difference in returns.


### Economic Magnitude

Across the 1936–1975 sample, the return spread between small and large firms (SMB‑like) was roughly **0.3% to 0.7% per month**, which translates to about **3.6% to 8.4% per year**.  

This means that, on average, **investors earned noticeably higher returns from holding small-cap stocks compared to large-cap stocks**. The spread reflects the “size premium”: the additional compensation that the market historically provided for taking on the risk of investing in smaller, potentially more volatile firms. A 0.3–0.7% monthly difference may seem small, but compounded over a year, it represents a meaningful extra return for small-firm investors, consistent with the size effect that Banz documented.


Banz showed that the size effect was persistent by demonstrating that small firms earned higher returns in **every major subperiod** of the 1936–1975 sample. He also showed that the size coefficient in his regressions remained **consistently negative and statistically significant** year after year. In other words, the return advantage for small firms appeared repeatedly regardless of how the data was partitioned.

To test this relationship, Banz estimated cross-sectional regressions of the form:

$$
R_i = a + b \cdot \ln(\text{MV}_i) + c \cdot \beta_i + \varepsilon_i
$$

where $R_i$ is the return on stock $i$, $MV_i$ is the market value (firm size), and $\beta_i$ is the stock’s CAPM beta.

The empirical results show that the coefficient on **log market value** is negative and statistically significant. This implies that **smaller firms earn higher risk-adjusted returns**, even after controlling for beta, indicating that firm size contains explanatory power for returns beyond what **CAPM beta** alone captures.


In conclusion his key findings were that:

1. Small firms earn significantly higher average returns

2. He adjusted for beta (risk) so that the smallest stocks earned higher returns than larger stocks even when they have the same beta.

3. He found that this is stable and something that happened over a long period of time.
