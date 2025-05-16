**Project: Developed and Emerging Countries Risk Analysis from an Investment Perspective**

**Objective:**
The primary objective of this project was to **assess and analyze investment risk** in both Developed Markets (DMs) and Emerging Markets (EMs). The goal was to provide insights for investors seeking to balance their portfolio in terms of risk and return, particularly through geographical diversification.

**Data:**
The project utilized **16 key metrics for 155 countries spanning from 1999 to 2022**. These metrics were categorized into four macrocategories: Macroeconomic Stability, Public Finance & Health, External Financing & Strength, and Governance Stability & Quality. Data was gathered, cleaned, dimensionally reduced, and normalized. 64 countries were eliminated if their GDP was less than 0.01% of the World's Total GDP.

**Methodology:**
1.  **Data Aggregation & CRI Build-Up:** An **aggregated Country Risk Index (CRI)** was created as an equally weighted sum of the cleaned and normalized key metrics. The CRI was normalized between 0 (minimum risk) and 1 (maximum risk).
2.  **Time Frame Analysis:** The CRI was calculated for **short-, medium-, and long-term time frames**. Time-dependent indicators (Macroeconomic and Public Finance categories) were calculated based on the difference between the last data point (2022) and the average of 3, 5, or 10 preceding years depending on the time frame.
3.  **Risk-Return Correlation & Regression:**
    *   A **univariate OLS regression** was performed between the CRI (predictor) and the Yield of 10-year maturity bonds (response) for each time frame.
    *   A **multidimensional regression** using the single key metrics was also conducted to evaluate their individual effects on the bond yield.

**Key Findings:**
*   **DM vs. EM Risk Profiles:** DMs are characterized by **stable financial systems, political contexts, lower volatility, and predictable returns**. EMs offer **rapid economic growth potential but have higher volatility, external vulnerabilities, lower liquidity, and higher transaction costs**. The CRI confirmed that DMs display lower risk values than EMs.
*   **Risk Factors:** Key risk factors analyzed included market liquidity, market volatility, sovereign debt, political stability, regulatory risk, global trade dependency, and commodity price dependency. EMs generally exhibited higher risk in these areas.
*   **Country Risk Index (CRI):** The CRI proved to be a valuable tool for assessing and forecasting risk, particularly distinguishing between short-, medium-, and long-term investment profiles.
    *   DMs dominate top rankings in the long-term CRI, while short-term CRI gives more weight to annual swings.
    *   Long-term risk can be higher for some DMs (like Japan, Italy, Ireland) due to increased debt-to-GDP in recent years.
    *   EMs exhibit higher risk in the short term, driven by unstable conditions and external shocks.
    *   Analysis of different EM sub-regions (Asia, LATAM, EME, MECA) revealed varying CRI values and specific challenges.
*   **CRI - Bond Yield Correlation:** Regression analyses showed that CRI indicators **strongly correlate with bond yields**, with R-squared values between 80% and 90% across time frames in the multidimensional models. The multidimensional models had high explanatory power (R^2 > 0.8) and statistical significance.

**Conclusion:**
The project successfully quantified and compared investment risks between Developed and Emerging Markets using the constructed Country Risk Index (CRI). The analysis demonstrated the significant influence of various macroeconomic, public finance, external financing, and governance factors on country risk and their strong correlation with bond yields. This provides investors with tools and insights for informed geographical diversification decisions. Enhancements to the CRI aggregation method could further improve its predictive accuracy.
