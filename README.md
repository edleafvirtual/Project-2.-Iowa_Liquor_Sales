![](https://www.leafwebstudio.com/wp-content/uploads/2022/07/png-20.png)

## Iowa Alcoholic Beverages Division 2022 Prediction
#### Iowa Liquor Sales Project is an exercise that is part of Coding Dojo: Data Science Bootcamp, where I'm trying to show how Industrial Engineering and Data Science would live together when we want to improve business process/KPI performances.
<img src="https://raw.githubusercontent.com/matiassingers/awesome-readme/master/icon.png" align="right" />

## Author
#### Name: Eduardo Galindez.
#### Date: August 2022.

<img alt="GitHub followers" src="https://img.shields.io/github/followers/edleafvirtual?style=social"> <img alt="GitHub User's stars" src="https://img.shields.io/github/stars/edleafvirtual?style=social"> <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/edleafvirtual/sales_predictions2023?style=social">

## Case Study Information
#### General Objective:
- Prepare the data for Machine Learning to predict [Iowa Alcoholic Beverages Division](https://abd.iowa.gov/ "Iowa Alcoholic Beverages Division") 2022 income from Class E alcohol liquor sales across licensed vendors using historical data (2019, 2020, and 2021) from Iowa [Liquor Sales](https://console.cloud.google.com/marketplace/product/iowa-department-of-commerce/iowa-liquor-sales?project=lively-clover-358509 "Liquor Sales").
#### Specific Objectives:
- 

#### Scope:
- Our study consists of two parts. The [first](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20I:%20sales_prediction2023.ipynb "first") one is where we developed a visual analysis in order to understand the current situation of the sales, focused on how the visibility index could affect the sales performance.
- In [Part II](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20II:%20sales_prediction2023_(ML).ipynb "Part II"), we prepared our data for Machine Learning, evaluating two regression methods to predict the sales for 2023.

#### Dataset:
- The data set can be found [here](https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view "here").
- In context (as is reported in [Part I](https://github.com/edleafvirtual/sales_predictions2023/blob/main/sales_prediction2023.ipynb "Part I")):
+ We have three variables that we consider that would affect the sales volume (Variables Type A):
  + Item_Visibility.
  + Item_Type.
  + Item_MRP.
- We identified three variables that could affect the sales behavior (Variables Type B):
  - Outlet_Size.
  - Outlet_Location_Type.
  - Outlet_Type.
 
- We are going to work with the variables described above to compare their relationship with Item_Outlet_Sales, our target.
- For our Machine Learning model:
  - Target (y):
    - Item_Outlet_Sales.
  - Features (X):
    - Numerical:
      - Item_Visibility.
      - Item_MRP.
    - Categorical:
      - Item_Type.
      - Outlet_Size.
      - Outlet_Location_Type.
      - Outlet_Type.

## Outcome
### Insights from [Part I](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20I:%20sales_prediction2023.ipynb "Part I"):
- We decided to plot a Pareto analysis in order to determine the product types that Big Mart sells more, to have a better idea about the possible impact in the results.
![pareto](https://www.leafwebstudio.com/wp-content/uploads/2022/07/P1-pareto.png "pareto")

- Keeping the focus on the visibility index, we plot the relationship between this index and sales.
![sales vs visibility index](https://www.leafwebstudio.com/wp-content/uploads/2022/07/P1-sales.png "sales vs visibility index")

- The visibility index is a feature that we identified as a variable that could be improved in order to increase sales, so we decided to compare the improvement with two stores that possibly will open in 2023.
![strategy](https://www.leafwebstudio.com/wp-content/uploads/2022/07/P1-strategy.png "strategy")

### Insights from [Part II](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20II:%20sales_prediction2023_(ML).ipynb "Part II"):
- We built a Linear Regression and Random Forest in order to evaluate and determine which model should be considered for our Machine Learning. 
- As the table below shows, Random Forest is the model recommended.
![regression](https://www.leafwebstudio.com/wp-content/uploads/2022/07/P2-reg-comp.png "regression")

## Recomendations
- For [Part I](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20I:%20sales_prediction2023.ipynb "Part I"):
  - As Section 8.2.1. shows in the notebook, we recommend finishing the code in order to determine how much the visibility index increase per store and product type. That way our recommendation would be more realistic than assuming the index increase 20% in total.
  - After the modification, is important to check the Pareto again in order to keep the focus point displayed throughout the case study.
- For [Part II](https://github.com/edleafvirtual/sales_predictions2023/blob/main/Part%20II:%20sales_prediction2023_(ML).ipynb "Part II"):
  - Append the NumPy Array (predicted values) to the original dataset to compare and evaluate how much the sales would be in 2023.
  - Make another visual analysis in order to manage the new insights.
  - Create a new simulation including the cost of the visibility improvement, where maybe not all product types require the improvement after the append.

## Limitations
- Not having access to the data administrator made us infer and play with the data in a way that maybe is not factible.
- One of the biggest assumptions is how the visibility index works. 
