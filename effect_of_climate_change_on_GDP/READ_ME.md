
**Project Summary: Temperature Shocks and Economic Growth**

This project is based on the academic paper "Temperature Shocks and Economic Growth: Evidence from the Last Half Century" by Melissa Dell, Benjamin F. Jones, and Benjamin A. Olken, published in the American Economic Journal: Macroeconomics in July 2012. The extension work builds upon the analysis presented in this paper.

**Summary of the Original Paper:**

*   **Objective:** The paper investigates the effects of historical fluctuations in temperature and precipitation on aggregate economic outcomes across countries over the last half century (1950-2003). It aims to inform long-standing debates about temperature's role in economic development and newer discussions about the potential impacts of future warming.
*   **Methodology:** The authors constructed a dataset combining country-year level temperature and precipitation data (derived from gridded monthly time series, primarily from the Global Historical Climatology Network) with aggregate output data, mainly from the World Development Indicators. Their main approach uses year-to-year fluctuations ("weather shocks") to identify the causal effects of temperature and precipitation, isolating these effects from time-invariant country characteristics. They analyze aggregate outcomes directly, without relying on a priori assumptions about specific mechanisms.
*   **Key Findings:** The paper reports three primary results:
    1.  **Significant negative effects of higher temperatures on economic growth, specifically in poor countries**. A 1°C rise in temperature in a given year is estimated to have reduced economic growth in poor countries by about 1.3 percentage points in that year.
    2.  Evidence suggesting that **higher temperatures may reduce growth rates**, not just the level of output. Analysis of multiple lags of temperature indicates that shocks appear to have persistent impacts on economic output.
    3.  Demonstration that **higher temperatures have wide-ranging effects beyond agriculture**, also reducing industrial output and political stability. This highlights channels often not considered in traditional aggregate climate-economy models.
*   **Rich vs. Poor Countries:** Temperature changes did not show a robust, discernible negative effect on growth in rich countries. The impact of temperature on economic growth is strikingly different between rich and poor countries.
*   **Precipitation:** Changes in precipitation had relatively mild effects on national growth in both rich and poor countries, although precipitation did show positive effects on agricultural output in poor countries.

**Summary of the Extension Work:**

*   **Objective:** This extension paper investigates the relationship between environmental factors—specifically temperature and precipitation—and economic growth in both rich and poor countries, building on the framework of the original paper. The motivation is rooted in growing concerns over climate change and its potential effects on economic growth and inequality.
*   **Empirical Approach:** The analysis utilizes a "Base Model" structured with the formula: `gdp_growth ~ temp + prec + poor:temp + poor:prec + C(country) + C(region_year) + C(poor_year)`. This panel regression includes country fixed effects (`C(country)`), region-year fixed effects (`C(region_year)`), and poor-year fixed effects (`C(poor_year)`), as well as interactions between temperature/precipitation and a dummy variable for poor countries (`poor:temp`, `poor:prec`).
*   **Finding from Base Model:** In the Base Model, the coefficient for `temp` models the average effect of a 1°C increase in temperature on GDP growth (%) for rich (non-poor) countries. This coefficient is estimated at 0.085, suggesting a positive relationship, but the source notes that this result is not statistically significant, meaning a consistent or reliable impact on rich countries' economic performance cannot be confidently stated based on this coefficient in the base model.
*   **Effect on Poor Countries:** The effect of temperature on poor countries in this model is calculated as the sum of the non-interacted `temp` term and the interacted `poor:temp` term.

LINK TO ORIGINAL PAPER: https://www.aeaweb.org/articles?id=10.1257/mac.4.3.66
