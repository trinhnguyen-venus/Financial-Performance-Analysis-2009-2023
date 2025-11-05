# 📊 Financial Performance Analysis of Global Companies (EDA & Storytelling)
---
## 1. Project Overview
This project explores the financial performance of global companies through data-driven storytelling.
Using key financial indicators such as Revenue, Market Capitalization, Profitability Ratios (ROE, ROA), and Capital Structure (Debt/Equity), the analysis aims to answer:

💡 “Do large companies truly generate better returns?”
💡 “How does industry type and inflation affect corporate profitability?”

The analysis combines data cleaning, financial ratio computation, and exploratory data visualization to uncover insights about firm efficiency and risk.

## 2. Tools Used

**Python (pandas):** Data manipulation and calculation
**Python (Matplotlib, Seaborn):** Visualization and storytelling
**Excel (initial data review):** Basic review and variable creation


## 3. Dataset Overview
**Existing Variables**
| Variable                                                      | Description                                           |
| ------------------------------------------------------------- | ----------------------------------------------------- |
| **Year**                                                      | Financial year                                        |
| **Market_Cap(in_B_USD)**                                      | Company market capitalization (Billion USD)           |
| **Revenue**                                                   | Annual revenue (Billion USD)                          |
| **Gross_Profit**                                              | Gross profit after production costs                   |
| **Net_Income**                                                | Net profit after taxes                                |
| **ROE, ROA**                                                  | Return on Equity & Assets – key profitability metrics |
| **Debt/Equity_Ratio**                                         | Capital structure measure of leverage                 |
| **Cash_Flow_from_Operating, Investing, Financial_Activities** | Cash flow components                                  |
| **Number_of_Employees**                                       | Workforce size                                        |
| **Category**                                                  | Industry classification                               |
| **Inflation_Rate(in_US)**                                     | Macro factor controlling environment                  |

**Newly Created Variables**
| New Metric               | Formula                                                 | Meaning                               |
| ------------------------ | ------------------------------------------------------- | ------------------------------------- |
| **Gross Margin**         | `gross_profit / revenue`                                | Efficiency of production & sales      |
| **Profit Margin**        | `net_income / revenue`                                  | Net profit per revenue unit           |
| **Return on Capital**    | `net_income / (shareholder_equity + total_liabilities)` | Capital efficiency                    |
| **Revenue per Employee** | `revenue / number_of_employees`                         | Workforce productivity                |
| **Debt to Equity**       | *Reassigned from `debt/equity_ratio`*                   | Leverage ratio for stability analysis |


## 4. Exploratory Storytelling
### 4.1 Relationship between Revenue and Market Cap

![Revenue vs Market Cap](Images/Revenue_vs_marketcap.png)
A clear positive correlation shows that higher revenue often translates into higher market capitalization.

However, industries like IT and Logistics exhibit disproportionately high market caps compared to revenue, reflecting investor confidence and growth potential rather than current income.

### 4.2 Market Cap & ROE Relationship
![Market Cap & ROE Relationship](Images/Market_Cap_&_ROE_Relationship.png)
- Companies with higher Debt-to-Equity tend to exhibit volatile ROE.
- Leverage helps increase returns to a certain extent, but too much debt increases financial risk.
- The trend line shows that moderate leverage improves capital efficiency.

### 4.3 Distribution of Key Financial Metrics
![Distribution of key metrics](Images/Distribution_of_Key_Financial_Metrics.png)
- Most companies operate in the lower range of revenue and profit, while a few large players dominate the market.
- ROE and ROA vary widely, showing different levels of operational efficiency across industries.

### 4.4 Profitability Trends Over Time
![ROA & ROE trend](Images/Profitability_Trend.png)
- ROE fluctuates more than ROA, showing greater sensitivity to equity and market shocks.
- Post-2016 recovery aligns with a global rebound in tech profitability.
- Stability in ROA suggests operational consistency even under inflationary pressure.

### 4.5 Industry Comparison of Financial Health

| Industry    | ROE    | ROA   | Debt/Equity | Interpretation                                      |
| ----------- | ------ | ----- | ----------- | --------------------------------------------------- |
| **IT**      | 36.8%  | 15.7% | 0.42        | Outstanding profitability with manageable leverage. |
| **FinTech** | 12.7%  | 4.3%  | 0.22        | Strong emerging sector with low debt reliance.      |
| **ELEC**    | 19.5%  | 12.2% | 0.26        | Balanced returns and stable capital structure.      |
| **FOOD**    | -42.2% | 14.3% | -2.83       | Negative ROE due to heavy liabilities.              |
| **Finance** | 16.7%  | -7.7% | -0.30       | High equity return but unstable asset efficiency.   |
| **BANK**    | 5.0%   | 0.24% | 6.29        | Highly leveraged — structurally risky.              |

- IT and FinTech sectors lead in profitability.
- Food and Manufacturing sectors face negative ROE due to high liabilities.
- Banking sectors show strong equity returns but carries high leverage risk.

## 5. Key Takeaways
1. Size doesn’t equal profitability: Large firms tend to have higher revenue and market cap, but profitability depends on capital structure efficiency, not size alone.
2. Leverage Balance is essential: Moderate debt can improve ROE, while excessive leverage leads to instability.
3. Tech-driven growth: IT and FinTech dominate due to scalable models, high margins, and investor optimism.
4. Productivity advantage: Tech firms generate higher revenue per employee, proving superior workforce efficiency.

## Author

Trinh Nguyen
📧 Contact: ng.trinh3023@gmail.com
📍 GitHub: [https://trinhnguyen-venus.github.io/](https://trinhnguyen-venus.github.io/)

📍 Project for skill development in financial analytics.