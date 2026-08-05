# Wealth and Wellness: Unpacking the Relationship Between GDP and Life Expectancy (2000-2015)

### Introduction
Does a wealthier nation inherently guarantee a longer life for its citizens? 

It is a question that sits at the intersection of economics and public health. To explore this, I analyzed a combined dataset from the World Health Organization (WHO) and the World Bank, tracking six nations between the years 2000 and 2015. By visualizing the data, we can uncover exactly how economic output correlates with the longevity of a population.

### The Background: Understanding the Metrics
Before diving into the visualizations, it helps to establish what we are actually measuring. 
* **Life Expectancy at Birth:** The average number of years a newborn is expected to live if mortality patterns at the time of its birth remain constant in the future.
* **Gross Domestic Product (GDP):** The total monetary value of all finished goods and services produced within a country's borders in a specific time period. It functions as a comprehensive scorecard of a given country’s economic health.

The dataset includes six countries (Chile, China, Germany, Mexico, the United States, and Zimbabwe), providing a diverse cross-section of global economies and healthcare infrastructures.

### Visualizing the Data

**1. The Distribution of Life Expectancy (Violin Plots)**
To understand the baseline, we first look at the distribution of life expectancy across the six nations using a violin plot. While developed nations like Germany and the United States show a tight clustering of life expectancies in the high 70s to low 80s, Zimbabwe's distribution sits significantly lower, though it shows a wide spread indicating rapid changes within the 15-year window.

**2. Tracking Life Expectancy Over Time (Line Graphs)**
When mapping life expectancy sequentially from 2000 to 2015, the overarching trend is incredibly positive. Every single nation in the dataset saw an increase in life expectancy over the 15-year period. Most notably, Zimbabwe experienced a dramatic upward curve starting around 2004, recovering from a severe dip in the early 2000s.

**3. Tracking Economic Growth (Line Graphs)**
Plotting GDP over the same time period reveals stark economic disparities. The United States and China show massive, exponential upward trajectories in economic growth. Conversely, nations like Chile and Zimbabwe have GDPs that appear nearly flat on a standard axis when compared to the multi-trillion-dollar economies of the US and China, highlighting the sheer scale of global wealth inequality.

**4. The Correlation: GDP vs. Life Expectancy (Scatter Plots)**
To answer our core question, we plot GDP against Life Expectancy on a facet grid of scatter plots. Because the GDP disparities between nations are so vast, I applied a logarithmic transformation to the GDP data. 

The results are striking: there is a highly visible, strong positive correlation in almost every nation. As a country's GDP grows, its life expectancy trends upward in tandem. 

### Conclusion, Limitations, and Future Research
The data clearly demonstrates that economic growth is heavily correlated with increased life expectancy. However, as data scientists, we must remember that **correlation does not equal causation**. 

**Limitations of the Data:**
* GDP is a macro-economic indicator. It does not account for wealth inequality *within* a nation. A country could have a massive GDP, but if that wealth belongs to the top 1%, it may not positively impact the life expectancy of the average citizen.
* The data does not account for specific public health interventions, infrastructure changes, or historical events (like wars or pandemics).

**Further Research:**
Future analysis should incorporate Gini coefficients (a measure of wealth inequality) and per-capita healthcare spending to determine if *how* money is distributed is a stronger predictor of life expectancy than raw GDP alone.
