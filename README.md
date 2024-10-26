#### Product Data Analysis


![Product Data](https://github.com/user-attachments/assets/68c44213-f00d-4423-8638-879f2ac3613e)

## Objective:

Analyze product-related data to address specific business questions, such as filtering costs within a range, counting items by specific criteria, and creating conditional logic based on cost, year, and status.

## Problems Solved and Approach:
- Highlighting Cost Values Between 10,000 and 20,000

Objective: Identify products with costs between 10,000 and 20,000.

Method:
Applied Conditional Formatting with the formula:
=AND(C2>10000, C2<20000)

Changed the background color to red and the text color to white for the matching cells.

- Finding the Total Number of Items Based on Criteria

Objective: Find the total number of specific items (Product 3) with a status of "Excess extra."

Method:
Used SUMIF formula:
=SUMIF(A2:A50, A2, C2:C50)
=SUMIF(D2:D50, D2, C2:C50)

- Calculating the Average Cost for Specific Years

Objective: Calculate the average cost for the years 2015, 2017, and 2019.

Method:
Applied AVERAGEIF formula:
=AVERAGEIF(B2:B50, F2, C2:C50)

- Creating a Validation Logic

Objective: Generate “Yes” or “-” based on these conditions:
Year < 2020
Cost >= 15,000

- Status: Promo or Excess extra
  
Method:
Used a Nested IF formula:
=IF(B2<2020, "YES", IF(C2>=15000, "YES", IF(OR(D2="PROMO", D2="EXTRA"), "YES", "-")))

## Summary of Key Insights:

Products within the cost range of 10,000 to 20,000 were effectively highlighted, ensuring clear identification.

Total quantities of specific products based on custom criteria were calculated, supporting inventory and procurement decisions.

Average cost analysis for multiple years provided insights into historical pricing trends.

Conditional validation logic enabled easy classification based on year, cost, and product status.
