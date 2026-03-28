# Life Expectancy & GDP Analysis
 
## Overview
Analysis of the relationship between GDP per capita and life expectancy
across six countries using WHO and World Bank data (2000-2015).
 
## Countries Analysed
Chile, China, Germany, Mexico, United States, Zimbabwe
 
## Key Questions
- Is there a correlation between GDP and life expectancy?
- How has this relationship changed over time?
- Which countries show the strongest / weakest correlation?
 
## Setup
```bash
git clone https://github.com/<you>/life-expectancy-gdp-analysis.git
cd life-expectancy-gdp-analysis
python -m venv env && source env/bin/activate
pip install -r requirements.txt
jupyter notebook
```
 
## Data Sources
- World Health Organization (WHO)
- World Bank GDP data
 
## Results
See the blog post in blog_post.md or the full analysis in the notebook.

## Environment Setup

This project uses Anaconda. To recreate the environment:
```bash
conda env create -f environment.yml
conda activate life-expectancy
```

Or if you just want to install the dependencies manually:
```bash
conda install pandas matplotlib seaborn jupyter notebook
```

## Running the Notebook
```bash
jupyter notebook life_expectancy_gdp.ipynb
```

## Dependencies

See `environment.yml` for the full list of packages and versions.
