# La Liga Transfer Spending & Sporting Performance Analytics

## Project Overview

This project analyses the relationship between football transfer activity, transfer spending, and sporting performance in La Liga.

The objective is to understand whether clubs that spend more in the transfer market consistently achieve better sporting outcomes, and whether clubs can achieve strong performance through more efficient transfer strategies.

The analysis is designed from a Sporting Director / football business perspective, focusing not only on how much clubs spend, but on how effectively that investment is converted into sporting results.

## Business Objectives

The project aims to answer the following questions:

1. How active are La Liga clubs in the transfer market?
2. Which types of transfers are most commonly used?
3. Is higher transfer spending associated with better league performance?
4. How strong is the relationship between transfer spending and league points?
5. Can clubs achieve strong sporting performance with relatively low transfer investment?
6. Which club-seasons demonstrate characteristics of a "Smart Spender"?
7. Which clubs spend heavily without achieving proportionate sporting success?
8. Which transfer strategies appear to be associated with stronger sporting outcomes?
9. From a Sporting Director's perspective, what strategy provides the best balance between financial investment and sporting performance?

## Dataset

The analysis covers La Liga club season data from **2019 to 2022**.

Key variables include:

- Transfer spending
- Number of transfers
- Number of paid transfers
- Average player age
- League points
- Wins, draws and losses
- Goals scored
- Goals conceded
- Goal difference
- Transfer strategy/type

The final analytical dataset contains **54 club-season observations**.

## Analytical Approach

The project uses Python and applies several analytical techniques:

- Data cleaning and preparation
- Exploratory Data Analysis
- Descriptive statistics
- Correlation analysis
- Correlation heatmap
- Linear regression 
- Transfer spending efficiency analysis
- High vs low spending comparison
- Sporting Director segmentation
- Transfer strategy effectiveness analysis
- Data visualization

## Key Findings

### 1. Transfer Spending and League Performance

The correlation between transfer spending and league points is:

**0.506**

This indicates a **moderate positive relationship** between transfer spending and league performance.

However, the relationship is not strong enough to suggest that spending alone determines sporting success.

### 2. Regression Analysis

The linear regression model produced:

- **R² = 0.256**
- **Transfer spending coefficient = 0.1146**
- **p-value < 0.001**

The model indicates that transfer spending has a statistically significant positive relationship with league points.

However, spending explains approximately **25.6% of the variation in league points**, showing that other factors also play a major role in sporting performance.

This supports an important football-business insight:

> **Spending more can help, but spending efficiently matters more than simply spending more.**


### 3. High vs Low Spending Clubs

The analysis divided club-seasons into high- and low-spending groups using the median transfer spending.

| Metric | High Spending | Low Spending |
|---|---:|---:|
| Average Transfer Spending | €64.09M | €5.32M |
| Average League Points | 60.26 | 49.19 |
| Average Wins | 16.63 | 12.56 |
| Average Goal Difference | +12.89 | -2.89 |

High-spending clubs achieved better average sporting outcomes, but the results also show that financial investment does not guarantee proportional success.

## Sporting Director Matrix

Club-seasons were classified into four strategic categories:

### Big Spender - Successful
High investment combined with strong sporting performance.

### Smart Spender
Relatively low investment combined with strong sporting performance.

### Low Investment - Low Performance
Low spending accompanied by weaker sporting results.

### Expensive Underperformer
Relatively high spending without proportionate sporting success.

This framework allows transfer strategies to be evaluated from both a **financial and sporting perspective**.

## Transfer Efficiency

The project also evaluates transfer efficiency using measures such as:

- Points per €1 million spent
- Sporting performance score
- League points
- Wins
- Goal difference

Examples of high-efficiency club-seasons included:

- Real Sociedad - 2021
- Villarreal CF - 2022
- Getafe CF - 2019

These examples demonstrate that strong sporting outcomes can sometimes be achieved without extremely high transfer expenditure.

## Transfer Strategy Effectiveness

The analysis compares different transfer strategies, including:

- Loan Return
- Internal Promotion
- Permanent Transfer
- Free Transfer
- Loan

The results show that different transfer mechanisms have different relationships with sporting performance.

This suggests that Sporting Directors should evaluate not only the financial value of a player acquisition, but also the wider strategic role of the transfer.

## Business Recommendations

### 1. Focus on transfer efficiency, not transfer volume.

Clubs should evaluate how much sporting value is generated from each euro invested rather than simply increasing transfer expenditure.

### 2. Identify undervalued recruitment opportunities.

Clubs with limited budgets can potentially compete by identifying players whose expected sporting contribution exceeds their acquisition cost.

### 3. Monitor expensive underperformers.

High transfer spending should be continuously evaluated against league points, wins and goal difference to identify inefficient investment.

### 4. Strengthen internal player development.

Internal promotion can provide clubs with a lower-cost alternative to external recruitment and may improve long-term squad sustainability.

### 5. Combine financial and sporting KPIs.

Transfer decisions should be evaluated using both financial metrics and sporting indicators rather than relying on transfer fees alone.

## Key Business Insight

The central finding of this project is:

> **Financial investment is associated with better sporting performance, but transfer spending alone does not guarantee success. The strongest strategic opportunity lies in improving the efficiency with which transfer investment is converted into sporting performance.**

From a Sporting Director's perspective, the goal should therefore not simply be to **spend more**, but to **create more sporting value from every euro spent**.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Jupyter / Google Colab
- GitHub

## Project Structure

```text
LaLiga-transfer-performance-analytics/
│
├── LaLiga_TMA.ipynb
├── final_football_transfer_performance.csv
├── primera-division (1).csv
├── spanish_football_games.csv
│
├── top_10_transfer_efficiency.csv
├── top_10_biggest_spenders.csv
├── smart_spenders.csv
├── expensive_underperformers.csv
├── sporting_director_matrix_summary.csv
├── transfer_strategy_effectiveness.csv
│
├── spending_vs_points.png
├── correlation_heatmap.png
├── high_vs_low_spending.png
├── sporting_director.png
│
└── README.md
