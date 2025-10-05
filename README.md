# Government R&D Expenditure Analysis: Economic Activity-wise Distribution (2018-2021)

## Data Disclaimer
 **Important Notice**: This analysis is based on publicly available government data and is intended for educational and research purposes only. The findings and interpretations presented in this report are those of the analyst and do not necessarily reflect official government positions or policies. Users should verify data accuracy and consult original sources before making any decisions based on this analysis.

## Project Overview
This project presents a comprehensive analysis of Government expenditure on Research & Development (R&D) across different economic activities in India during the financial years 2018-19 to 2020-21. The analysis employs various data visualization techniques to identify trends, patterns, and insights in R&D spending allocation across sectors.

## Dataset Details

### Source
- **Dataset Name**: Government Expenditure on R & D by Economic Activity during FY 2018-19 to 2020-21
- **Source**: [data.gov.in](https://data.gov.in) - India's Open Government Data Platform
- **Data Type**: Open Source Government Data
- **Time Period**: Financial Years 2018-19, 2019-20, and 2020-21

### Dataset Structure
```
Dataset Shape: 21 entries × 6 columns
Total Economic Activities Analyzed: 20 (excluding total row)

Columns:
- S.No.: Serial Number
- Economic Activity: Sector/Industry Classification
- NIC Code: National Industrial Classification Code
- Research & Development Expenditure (2018-19): R&D spending in FY 2018-19
- Research & Development Expenditure (2019-20): R&D spending in FY 2019-20
- Research & Development Expenditure (2020-21): R&D spending in FY 2020-21

Data Types: 5 float64 columns, 1 object column
Memory Usage: 1.1+ KB
Missing Values: Minimal (only in total count row)
```

## Key Statistics and Initial Findings

### Overall Expenditure Trends
- **Total R&D Expenditure (2018-2021)**: ₹204,703.44 crores
- **2018-19**: ₹67,859.39 crores
- **2019-20**: ₹72,681.71 crores (7.11% increase from previous year)
- **2020-21**: ₹64,162.34 crores (-11.72% decrease from previous year)
- **Net Change (2018-19 to 2020-21)**: -5.45% decline

### Top Performing Sectors (by Total Expenditure)
1. **Professional, Scientific and Technical Activities**: ₹111,936.06 crores (54.7% of total)
2. **Agriculture, Forestry and Fishing**: ₹37,926.54 crores (18.5% of total)
3. **Human Health and Social Work Activities**: ₹13,039.18 crores (6.4% of total)
4. **Education**: ₹11,462.97 crores (5.6% of total)
5. **Electricity, Gas, Steam and Air Conditioning Supply**: ₹10,143.76 crores (5.0% of total)

### Least Funded Sectors
1. **Other Manufacturing**: ₹0.03 crores
2. **Manufacture of Basic Metals**: ₹2.85 crores
3. **Manufacture of Computer, Electronic and Optical Products**: ₹10.37 crores
4. **Construction**: ₹30.41 crores
5. **Manufacture of Wood and Wood Products**: ₹33.37 crores

## Methodology

we have done basic Data exploratory approches to visualize the trends in the given data.

**Libraries Used:**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations and correlation analysis
- **Matplotlib**: Data visualization and plotting

### Visualization Techniques

#### 1. Bar Plots
- **Purpose**: Identify top-performing economic activities
- **Implementation**: Side-by-side comparison of top 10 sectors across three fiscal years
- **Insights**: Shows sector-wise R&D spending hierarchy and year-over-year changes

#### 2. Scatter Plots
- **Purpose**: Correlation analysis between different fiscal years
- **Implementation**: Three scatter plots comparing expenditure patterns
- **Statistical Measure**: Pearson correlation coefficients calculated for each year pair

#### 3. Box Plots
- **Purpose**: Distribution analysis and outlier identification
- **Implementation**: 
  - Overall distribution across all 20 economic activities
  - Focused analysis on top 10 activities
- **Statistical Analysis**: Interquartile Range (IQR) method for outlier detection

## Observations and Results

### From Bar Plot Analysis
- **Consistent Leaders**: Professional, Scientific and Technical Activities dominates across all years
- **Stable Sectors**: Agriculture, Forestry and Fishing maintains second position consistently
- **Growth Patterns**: Most sectors show gradual increase from 2018-19 to 2019-20, followed by decline in 2020-21
- **Sectoral Concentration**: Top 5 sectors account for approximately 90% of total R&D expenditure

### From Scatter Plot Analysis
- **High Correlations**: Extremely strong positive correlations between all year pairs
  - 2018-19 vs 2019-20: r = 0.999
  - 2019-20 vs 2020-21: r = 0.998
  - 2018-19 vs 2020-21: r = 0.998
- **Spending Consistency**: Sectors maintain relative spending positions across years
- **Linear Relationship**: Strong linear relationship indicates predictable spending patterns

### From Box Plot Analysis
- **Identified Outliers**: 
  - Agriculture, Forestry and Fishing (consistently above upper quartile)
  - Professional, Scientific and Technical Activities (extreme outlier across all years)
- **Distribution Characteristics**: 
  - Highly right-skewed distribution
  - Large interquartile range indicating significant spending disparities
  - Median expenditure remains relatively stable across years

### Temporal Trends
- **2019-20 Peak**: Maximum R&D expenditure recorded in FY 2019-20
- **2020-21 Decline**: Notable decrease possibly attributed to economic impacts
- **Sectoral Resilience**: Top sectors maintained their positions despite overall decline

## Key Conclusions

### 1. Sectoral Concentration
R&D expenditure is highly concentrated, with the top 2 sectors (Professional/Scientific/Technical Activities and Agriculture/Forestry/Fishing) accounting for over 73% of total spending.

### 2. Spending Stability
Despite year-to-year variations in absolute amounts, the relative distribution of R&D expenditure across sectors remains remarkably stable, as evidenced by correlation coefficients exceeding 0.998.

### 3. Economic Impact Indicators
The decline in 2020-21 expenditure (-11.72%) suggests potential economic pressures affecting R&D investments, while the recovery trajectory needs monitoring in subsequent years.

### 4. Strategic Focus Areas
Government R&D investment priorities clearly favor:
- Advanced scientific and technical research
- Agricultural innovation and food security
- Healthcare and social welfare technologies
- Educational advancement

### 5. Underinvested Sectors
Manufacturing subsectors, particularly traditional industries like basic metals and wood products, receive minimal R&D investment, potentially indicating areas for policy intervention.




