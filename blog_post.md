# Wealth and Wellness: Unpacking the Relationship Between GDP and Life Expectancy (2000-2015)

### Introduction
Does a wealthier nation inherently guarantee a longer life for its citizens? 

It is a question that sits at the intersection of economics and public health. To explore this, I analyzed a combined dataset from the World Health Organization (WHO) and the World Bank, tracking six nations between the years 2000 and 2015. By visualizing the data, we can uncover exactly how economic output correlates with the longevity of a population.

### The Background: Understanding the Metrics
Before diving into the visualization, it helps to establish what we are actually measuring. 
* **Life Expectancy at Birth:** The average number of years a newborn is expected to live if mortality patterns at the time of its birth remain constant in the future.
* **Gross Domestic Product (GDP):** The total monetary value of all finished goods and services produced within a country's borders in a specific time period. It functions as a comprehensive scorecard of a given country’s economic health.

The dataset includes six countries (Chile, China, Germany, Mexico, the United States, and Zimbabwe), providing a diverse cross-section of global economies and healthcare infrastructures.

### Visualizing the Correlation (GDP vs. Life Expectancy)
To answer our core question, we plotted GDP against Life Expectancy on a facet grid of scatter plots using Seaborn. 

Because the GDP disparities between these six nations are so vast (ranging from billions to multi-trillions), I applied a logarithmic transformation (`np.log10`) to the GDP data. Without this transformation, the economic data of smaller nations would be completely squashed on a linear scale, making it impossible to read.

The results of the regression models are striking: there is a highly visible, strong positive correlation in almost every single nation. As a country's GDP grows over the 15-year period, its life expectancy trends upward in tandem. 

### Conclusion, Limitations, and Future Research
The data clearly demonstrates that economic growth is heavily correlated with increased life expectancy. However, as data scientists, we must remember that **correlation does not equal causation**. 

**Limitations of the Data:**
* GDP is a macro-economic indicator. It does not account for wealth inequality *within* a nation. A country could have a massive GDP, but if that wealth belongs to the top 1%, it may not positively impact the life expectancy of the average citizen.
* The data does not account for specific public health interventions, infrastructure changes, or historical events.

**Further Research:**
Future analysis should incorporate Gini coefficients (a measure of wealth inequality) and per-capita healthcare spending to determine if *how* money is distributed is a stronger predictor of life expectancy than raw GDP alone.
