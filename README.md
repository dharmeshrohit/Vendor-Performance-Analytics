# Vendor Performance Analytics

Vendor Performance Analytics is a comprehensive data analysis project designed to help businesses understand and optimize the performance of their vendors. This repository provides the full workflow of ingesting raw transactional data, cleaning and organizing it into a structured database, and performing in-depth analytics to generate actionable insights on vendor selection, profitability, and product pricing optimization.

Data size: 2GB

Exploratory Data Analysis Notebook: [here](/Exploratory%20Data%20Analysis.ipynb)
<br>
Venodr Performance Analysis Notebook [here](/Vendor%20Performance%20Analysis.ipynb)
<br>
Comprehensive Analysis Report: [here](docs/Vendor%20Performance%20Report.pdf)
<br>
Power bi Dashboard: [here](docs/vendor_performance.pbix)
<br>
Cleaned & Aggregated data: [here](docs/vendor_sales_summary.xlsx)


## Business Problem 
Effective inventory and sales management are critical for optimizing 
profitability in the retail and wholesale industry. Companies need to ensure 
that they are not incurring losses due to inefficient pricing, poor inventory 
turnover, or vendor dependency. The goal of this analysis is to: 
- Identify underperforming brands that require promotional or pricing 
adjustments. 
- Determine top vendors contributing to sales and gross profit. 
- Analyze the impact of bulk purchasing on unit costs. 
- Assess inventory turnover to reduce holding costs and improve 
efficiency. 
- Investigate the profitability variance between high-performing and 
low-performing vendors. 

## Exploratory Data Analysis Insights
### Summary Statistics 
![Summary Statistics](docs/Summary%20Statistics.png)

**Negative & Zero Values:**
- **Gross Profit:** Minimum of -52,002.78, indicating potential losses due to high costs orheavy discounts. This could be due to selling products at lower prices than their purchase costs. 
- **Profit Margin:** Has a minimum of -∞, which suggests instances where revenue is zero or even lower than the total cost, leading to extreme negative profit margins.
- **Total Sales Quantity & Sales Dollars:** Some products show zero sales, indicating they were purchased but never sold. These may be slow-moving or obsolete stock, leading to inventory inefficiencies. 
- **Outliers Detected by High Standard Deviations:**
- **Purchase & Actual Prices:** Themaximum values (5,681.81 & 7,499.99) aresignificantly higher than the mean (24.39 &35.64), indicating premium product offerings. 

### Top Vendors by Sales & Purchase Contribution

![Top Vendors by Sales & Purchase Contribution](docs/Top%2010%20Vendor's%20Purchase%20Contribution.png)
The top 10 vendors contribute 65.69% of total purchases, while the remaining vendors contribute only 34.31%. This over-reliance on a few vendors may introduce risks such as supply chain disruptions, indicating a need for diversification.

### Profit Margin Comparison: High vs. Low-Performing Vendors
![](docs/Confidence%20Interval%20Comparison.png)
Top Vendors' Profit Margin (95% CI): (30.74%, 31.61%), Mean: 31.17%

Low Vendors' Profit Margin (95% CI): (40.48%, 42.62%), Mean: 41.55%

Low-performing vendors maintain higher margins but struggle with sales volumes, indicating potential pricing inefficiencies or market reach issues.

Actionable Insights: 
- Top-performing vendors: Optimize profitability by adjusting bundled pricing, reducing operational costs, or offering 
promotions. 
- Low-performing vendors: Improve marketing efforts, optimize pricing strategies, and enhance distribution networks

## Final Recommendations 
- Re-evaluate pricing for low-sales, high-margin brands to boost sales volume without sacrificing profitability. 
- Diversify vendor partnerships to reduce dependency on a few suppliers and mitigate supply chain risks. 
- Leverage bulk purchasing advantages to maintain competitive pricing while optimizing inventory management. 
- Optimize slow-moving inventory by adjusting purchase quantities, launching clearance sales, or revising storage strategies. 
- Enhance marketing and distribution strategies for low-performing vendors to drive higher sales volumes without compromising profit margins. 
- By implementing these recommendations, the company can achieve sustainable profitability, mitigate risks, and enhance overall operational efficiency.