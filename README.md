# Green Destinations Attrition Analysis

![green-destinations-image](GREEN_IMAGE.png)

## Project Overview 

- Green Destinations, a prominent travel agency, is experiencing an increase in employee attrition. This project aims to analyze the attrition data to identify trends and patterns. The HR Director is keen on understanding the attrition rate and exploring whether factors such as age, years at the company and income influence employees' likelihood to leave.

## Data:

- The dataset for analysis includes survey results from Green Destinations' staff. Key fields in the dataset are:

    - Employee Number
    - Age
    - Years at Company
    - Monthly Income
    - Attrition (Yes/No)
 
## Analysis and Visualizations:

### Attrition Rate Calculation:

- A calculated field determines the attrition rate (% of employees who have left):

```sql

(SUM(IF [Attrition] = 'Yes' THEN 1 ELSE 0 END) / COUNT([Employee Number]))


```

### Visualizations:

 #### Age Distribution:
 
   - Bar Chart showing the distribution of employees' ages, grouped into different age ranges.

 #### Years at Company Distribution:
 
   - Bar chart displaying the distribution of employees based on their tenure at the company, binned by length of service.

 #### Income Distribution:
 
   - Bar chart illustrating the distribution of employees' monthly incomes, grouped into various income ranges.

### Correlation Analysis:

- Several scatter plots examine potential correlations between factors:

  #### Age vs. Monthly Income:
  
    - Scatter plot (circle view) to explore correlation between age and monthly income.

  #### Age vs. Years at Company:
  
    - Scatter plot (circle view) to analyze correlation between and years spent at the company.
 
  #### Years at Company vs. Monthly Income:
  
    - Scatter plot (circle view) to investigate correlation between years at the company and monthly income.


## Findings: 

 - Calculated attrition rate highlights the percentage of employees who have left.
 - Bar charts provide insights into the distribution of age, tenure and income among employees.
 - Scatter plots visualize potential correlations between age, income and years at the company.


## Conclusion:

- This analysis aims to assist Green Destinations' HR Director in understanding attrition patterns. By examining age, tenure and income, the company can identify trends contributing to attrition and develop strategies to mitigate it.
