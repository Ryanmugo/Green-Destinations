# Green Destinations Attrition Analysis

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
