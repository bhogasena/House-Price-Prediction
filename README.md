# Regression Model using Ridge and Lasso Regularisation for House price Prediction

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.
 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

*   Which variables are significant in predicting the price of a house, and
*   How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.
     
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
Required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

Bike Sharing dataset [here](https://github.com/bhogasena/House-Price-Prediction/blob/main/train.csv) and Data dictionary [here](https://github.com/bhogasena/House-Price-Prediction/blob/main/data_dictionary.txt).

## Conclusions
# Final Inferences

- Ridge model optimal lamda value : **3.5**
- Lasso Model optimal lamda value: **0.001**
- Ridge Model Train R-Square is **0.9409985125478542** and Test R-Square is **0.9154572141126628**.
- Lasso Model Train R-Score:**0.935200485496919** and Test R-Score: **0.9201671252287877**
- So Lasso Model is performing better than Ridge for this prediction and also it's complexity is lower as it eliminated many of the features as we can see coefficients are zero.
- Top 10 Significant features and their co-efficients.
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>features</th>
      <th>coefficient</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>120</th>
      <td>OverallQual_10</td>
      <td>1.449774</td>
    </tr>
    <tr>
      <th>119</th>
      <td>OverallQual_9</td>
      <td>0.658890</td>
    </tr>
    <tr>
      <th>10</th>
      <td>GrLivArea</td>
      <td>0.346456</td>
    </tr>
    <tr>
      <th>85</th>
      <td>Neighborhood_StoneBr</td>
      <td>0.339560</td>
    </tr>
    <tr>
      <th>265</th>
      <td>SaleType_New</td>
      <td>0.307852</td>
    </tr>
    <tr>
      <th>118</th>
      <td>OverallQual_8</td>
      <td>0.276677</td>
    </tr>
    <tr>
      <th>69</th>
      <td>Neighborhood_Crawfor</td>
      <td>0.274849</td>
    </tr>
    <tr>
      <th>128</th>
      <td>OverallCond_9</td>
      <td>0.266331</td>
    </tr>
    <tr>
      <th>78</th>
      <td>Neighborhood_NoRidge</td>
      <td>0.262616</td>
    </tr>
    <tr>
      <th>139</th>
      <td>Exterior1st_BrkFace</td>
      <td>0.237273</td>
    </tr>
  </tbody>
</table>

#### Below are the few variables description on house price prediction.

- OverallQual10 - if overall material and finish of the house is Very Excellent, house price will increase by 1.45 times.
- OverallQual_9 - if overall material and finish of the house is Excellent, house price will increase by 0.66 times.
- GrLivArea     - A unit increase in the above grade (ground) living area square feet increase the house price by 0.346456 times.
- Neighborhood_StoneBr     - if Physical locations within Ames city limits is StoneBr price house tends to increase by 0.339560 times.
                          

## Technologies Used
- numpy - version 1.21.6
- matplotlib - version 3.2.2
- seaborn - version 0.11.2
- plotly - version 5.5.0
- statsmodels - version 0.10.2
- sklearn - version 1.0.2

## Contact
Created by [@bhogasena] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
