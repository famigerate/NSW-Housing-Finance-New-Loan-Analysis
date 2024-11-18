# Housing Finance New Loan Analysis
Please open the [NSW_Housing_Finance_New_Loan_Analysis.ipynb](https://github.com/famigerate/NSW-Housing-Finance-New-Loan-Analysis/blob/9a290928216b98cb5aab1d5a05b34c6c5f11c94d/NSW_Housing_Finance_New_Loan_Analysis.ipynb) for the project.

What was explored: 

With the current housing crisis, I was curious on the gap and the trend of how much is the average loan given to first home buyers vs the average loan given to a subsequent home buyer.

Outcome:

| Loan Type | Start Value ($,000) | End Value ($,000) | Percentage Increase (%) |
| :---: | :---: | :---: | :---: |
| NSW-FHB-OO | 558.27 | 711.81 | 27.50 |
| NSW-Subsequent-OO | 555.98 | 751.67 | 35.20 |
| NSW-FHB-Investment | 567.99 | 711.73 | 25.31|
| NSW-Subsequent-Investment | 553.98 | 799.57 | 44.33 |
| Sydney-Median-House-Price | 903.82 | 1479.52 | 63.70 |

Witn data consideration of One person may be approved for multiple subsequent investment loan. Which means the graph above is a conservative estimate as the true loan subsequent loan value is higher in potential.

In conclusion, from the data of the past 5 years it shows notable shift in the average loan ammount given to subsequent loan approval which highlight the steadily growing gap of NSW First Home Buyer in trying to break into the housing market.

What I did:
- There is no data of loan given subsequent home buyer ,however, I found that the Australia Bureau of Statistics has 2 diffrent data sets which can be use to get the data.
- Under [Lending Indicators](https://www.abs.gov.au/statistics/economy/finance/lending-indicators) we can find "Value of new borrower-accepted loan commitments" and "First Home Buyer" datasets.
- To make it less complicated, I extracted only the NSW data and saved it to my [NSW-FHB-vs-Subsequent-Loan.xlxs](https://github.com/famigerate/NSW-Housing-Finance-New-Loan-Analysis/blob/main/NSW-FHB-vs-Subsequent-Loan.xlsx) using xlookup to make sure no human error in compiling the data across.
- Calculation of Subsequent Household Loan Commitment value and loans given was made in Excel
- Graph of NSW FHB OO, NSW FHB investment, NSW Subsequent OO, NSW Subsequent investment now can be created as the result.
- The Median Dwelling Price was added to contrast on how the buying power effect each group, to make it simple, I only added the Sydney median dwelling price.
- Google Collab then used for its ease of developing, sharing and display.
- The cleaned dataset was used and reffered to make sure no human error was carried across
- Naive regression was applied to show the trend change between each group
  
What I learn:
- Excel sheet is bad for github. It enforces absolute path everytime it is saved. so it keeps putting my local path and refuse to just safe the absolute path. Relinking is needed and security is bad because of it
