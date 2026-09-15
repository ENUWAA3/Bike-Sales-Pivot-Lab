# Bike Sales Pivot Lab

## Project Overview
This project analyzes a bike sales dataset using Excel, focusing on order quantity and revenue broken down by customer age group, gender, and country. A pivot table and bar chart were built to explore purchasing patterns across these customer segments.



![Bar Chart](Bar%20Chart.PNG)


## Dataset
The dataset includes order-level bike sales records with the following fields: sales order number, date, customer age and age group, customer gender, country, state, product category/sub-category, order quantity, unit cost, unit price, profit, cost, and revenue.

## Pivot Table: Order Quantity by Age Group, Gender, and Country



![Pivot Table](Pivot%20Table.PNG)


| Age Group             | Total Units Sold |
|------------------------|------------------|
| Youth (<25)            | 27               |
| Young Adults (25–34)   | 61               |
| Adults (35–64)         | 99               |
| **Grand Total**        | **187**          |

### Units sold by country (all age groups combined)
| Country         | Units Sold |
|-----------------|------------|
| Australia       | 63         |
| Canada          | 11         |
| France          | 20         |
| Germany         | 13         |
| United Kingdom  | 14         |
| United States   | 65*        |

*\*United States appears twice in the raw pivot (once as "United States" and once as "United  States" with an extra space), so its totals were combined here — see Data Quality below.*

## Key Findings

1. **Adults (35–64) are the largest customer segment**, accounting for 99 of 187 units sold (about 53%) — more than Youth and Young Adults combined.
2. **The United States and Australia are the top two markets**, together making up roughly 68% of total units sold.
3. **Gender split shifts across age groups.** Among Youth, female buyers outsold male buyers (16 vs. 11 units). Among Adults, female buyers again slightly outsold male buyers (55 vs. 44 units).
4. **Total revenue across the dataset was $361,232**, with the United States and Australia contributing the largest shares.

## Data Quality Notes
- The "United States" country label appears with inconsistent spacing in the source data (an extra space in some rows), which caused it to split into two separate categories in the raw pivot table. This should be cleaned (e.g., with TRIM or Find & Replace) before further analysis.
- A small number of rows have missing "Day" values, though this does not affect the order quantity or revenue totals.

## Tools
- Microsoft Excel (PivotTables, PivotCharts)

## Conclusion
This analysis shows that older customers (35–64) and buyers from the U.S. and Australia drive the majority of bike sales volume in this dataset. Cleaning up inconsistent country labels would improve the accuracy of any deeper regional analysis.
