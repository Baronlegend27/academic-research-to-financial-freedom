# Fama & French (2015): *A Five‑Factor Asset Pricing Model*

The motivation for the **Fama & French (2015)** paper comes from well‑documented weaknesses in the **1993 three‑factor model**. Although the 1993 model captured size and value effects, a large empirical literature soon showed that it failed to explain return patterns linked to **profitability** and **investment**. Novy‑Marx (2013) demonstrated that firms with **high gross profitability** earned abnormally high returns unexplained by market, size, or value. Similarly, Titman, Wei, and Xie (2004), followed by Hou, Xue, and Zhang (2015), showed that firms with **conservative investment policies** systematically outperformed firms that aggressively expanded their assets, again contradicting the predictions of the three‑factor model. Additional evidence from Aharoni, Grundy, and Zeng (2013) reinforced that profitability and investment were powerful, persistent predictors of the cross‑section of returns. The **2015 five‑factor model** was Fama and French’s response: by adding **RMW** (profitability) and **CMA** (investment), they created a model that absorbs these anomalies and reveals that some original factors—especially HML—become less central once profitability and investment are explicitly included.


## What Stayed the Same (Methods Reused)

- **Factor construction through portfolio sorts** — size, book‑to‑market, profitability, and investment characteristics are used to build factor‑mimicking portfolios, following the same empirical design principles as the original three‑factor model.

- **Time‑series regressions** of excess returns on factor returns remain the core method for estimating each asset’s or portfolio’s factor loadings (betas).

- **Cross‑sectional evaluation** continues to test whether factor exposures are priced by comparing alphas, betas, and t‑statistics across large sets of test portfolios and examining the average factor premium.

$$R_{it} - R_{ft} = \alpha_{i} + \beta_i(R_{mt} - R_{ft}) + s_i \cdot SMB_t + h_i \cdot HML_t + r_i \cdot RMW_t + c_i \cdot CMA_t + \varepsilon_{it}$$


Robustness emphasis rather than new estimators: Rather than inventing new statistical estimators, Fama & French (2015) broaden the empirical scope (more sorts, more portfolios, alternative sample splits) to test the five‑factor specification’s robustness.



