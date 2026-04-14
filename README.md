# Life Expectancy & GDP Analysis

An analysis of the relationship between GDP and life expectancy across six 
countries using data from the World Health Organization (WHO) and the World 
Bank, covering the period 2000–2015.

## Research Questions

- Has life expectancy increased over time in the six nations?
- Has GDP increased over time in the six nations?
- Is there a correlation between GDP and life expectancy of a country?
- What is the average life expectancy in these nations?
- What is the distribution of that life expectancy?

## Countries Analyzed

| Country | Avg Life Expectancy | Avg GDP |
|---|---|---|
| Germany | 79.66 years | $3.09 trillion |
| Chile | 78.94 years | $169.8 billion |
| United States | 78.06 years | $14.07 trillion |
| Mexico | 75.72 years | $976.7 billion |
| China | 74.26 years | $4.96 trillion |
| Zimbabwe | 50.09 years | $9.1 billion |

## Key Findings

- Every country showed a correlation above 0.90 between GDP and life 
  expectancy when measured individually
- Zimbabwe gained 14.7 years of life expectancy (46.0 → 60.7) — the 
  largest improvement despite having the lowest GDP
- China recorded the largest economic growth, expanding nearly 10x 
  from $1.2 trillion to $11.1 trillion
- Chile outperforms the USA in average life expectancy (78.94 vs 78.06 
  years) despite having a GDP roughly 80x smaller
- The overall cross-country correlation between GDP and life expectancy 
  is moderate at 0.343, showing that GDP alone does not explain 
  differences between nations

## Project Structure
```
life-expectancy-gdp-analysis/
├── all_data.csv                  # Raw data (WHO & World Bank)
├── life_expectancy_gdp.ipynb     # Full analysis notebook
├── images/                       # Exported chart images
│   ├── life_expectancy_over_time.png
│   ├── gdp_over_time.png
│   ├── gdp_vs_life_expectancy.png
│   ├── average_life_expectancy.png
│   ├── life_expectancy_distribution.png
│   ├── correlation_matrix.png
│   ├── correlation_by_country.png
│   ├── facet_life_expectancy.png
│   ├── facet_gdp.png
│   └── facet_gdp_vs_life_expectancy.png
├── blog_post.md                  # Written findings
├── environment.yml               # Conda environment
└── README.md
```

## Setup & Installation

### Using Conda
```bash
# Clone the repository
git clone git@github.com:dxsastrous/life-expectancy-gdp-analysis.git
cd life-expectancy-gdp-analysis

# Create and activate the environment
conda env create -f environment.yml
conda activate life-expectancy

# Launch the notebook
jupyter notebook life_expectancy_gdp.ipynb
```

## Dependencies

- Python 3.11
- pandas
- matplotlib
- seaborn
- jupyter
- notebook

See `environment.yml` for the full list of packages and versions.

## Data Sources

- World Health Organization (WHO) — Life expectancy at birth (years)
  https://www.who.int
- World Bank — GDP (current USD)
  https://data.worldbank.org

## Visualizations

The notebook produces the following charts:

- Line plots of life expectancy and GDP over time per country
- Facet grids showing individual country trends side by side
- Scatter plot of GDP vs life expectancy on a log scale
- Horizontal bar chart of average life expectancy by country
- Violin plot and histogram showing life expectancy distribution
- Correlation heatmap and per-country correlation bar chart

## Conclusions

GDP and life expectancy are strongly correlated within each country,
but GDP alone does not explain the differences between countries.
Chile outperforms the USA in life expectancy despite a fraction of the
economic output, and Zimbabwe's remarkable health recovery demonstrates
that targeted public health investment can drive results independent of
GDP growth.

## Blog Post

Read the full write-up here:
https://medium.com/@ashanshethran2/does-wealth-buy-a-longer-life-a-15-year-analysis-of-gdp-and-life-expectancy-across-six-nations-4aec4e1af191

## License

MIT License — see `LICENSE` for details.