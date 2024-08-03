# Mart Sales Prediction

## Description
This project aims to predict the sales of products in various outlets of Big Mart using machine learning techniques. The dataset contains information about products and their sales in different outlets. The goal is to build a predictive model that can estimate the sales of products based on various features.

## Project Structure
- **Big Mart Sale_Final.R**: The main R script that contains the data loading, preprocessing, and modeling code.
- **Train_UWu5bXk.csv**: The training dataset containing historical sales data.
- **Test_u94Q5KV.csv**: The test dataset for which sales predictions need to be made.
- **SampleSubmission_TmnO39y.csv**: A sample submission file in the required format for submission.
- **README.md**: This file, providing an overview of the project.

## Requirements
The following R packages are required to run the project:
- [`data.table`](command:_github.copilot.openSymbolFromReferences?%5B%22data.table%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A1%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For reading and manipulating data.
- [`dplyr`](command:_github.copilot.openSymbolFromReferences?%5B%22dplyr%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A2%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For data manipulation and joining.
- [`ggplot2`](command:_github.copilot.openSymbolFromReferences?%5B%22ggplot2%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A3%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For plotting.
- [`caret`](command:_github.copilot.openSymbolFromReferences?%5B%22caret%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A4%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For modeling.
- [`corrplot`](command:_github.copilot.openSymbolFromReferences?%5B%22corrplot%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A5%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For making correlation plots.
- [`xgboost`](command:_github.copilot.openSymbolFromReferences?%5B%22xgboost%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A6%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For building the XGBoost model.
- [`cowplot`](command:_github.copilot.openSymbolFromReferences?%5B%22cowplot%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A7%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition"): For combining multiple plots.

## Installation
To install the required packages, you can use the following commands in R:
```r
install.packages("data.table")
install.packages("dplyr")
install.packages("ggplot2")
install.packages("caret")
install.packages("corrplot")
install.packages("xgboost")
install.packages("cowplot")
```

## Usage
1. **Load Packages**: The script starts by loading the necessary packages.
2. **Read Datasets**: The training and test datasets are read using the [`fread`](command:_github.copilot.openSymbolFromReferences?%5B%22fread%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A10%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition") function from the [`data.table`](command:_github.copilot.openSymbolFromReferences?%5B%22data.table%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A1%2C%22character%22%3A8%7D%7D%5D%5D "Go to definition") package.
3. **Explore Data**: The script displays the column names and structure of the training and test datasets.
4. **Preprocess Data**: The script adds a new column [`Item_Outlet_Sales`](command:_github.copilot.openSymbolFromReferences?%5B%22Item_Outlet_Sales%22%2C%5B%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Crehan%5C%5COneDrive%5C%5CDocuments%5C%5CVS%20CODE%20WORKSPACE%5C%5CR%20project%5C%5CBig%20Mart%20Sale_Final.R%22%2C%22_sep%22%3A1%2C%22external%22%3A%22file%3A%2F%2F%2Fc%253A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%2520CODE%2520WORKSPACE%2FR%2520project%2FBig%2520Mart%2520Sale_Final.R%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Frehan%2FOneDrive%2FDocuments%2FVS%20CODE%20WORKSPACE%2FR%20project%2FBig%20Mart%20Sale_Final.R%22%2C%22scheme%22%3A%22file%22%7D%2C%22pos%22%3A%7B%22line%22%3A28%2C%22character%22%3A6%7D%7D%5D%5D "Go to definition") to the test dataset and performs other preprocessing steps (not shown in the excerpt).

## Example
Here is an example of how to run the script:
```r
# Load packages
library(data.table)
library(dplyr)
library(ggplot2)
library(caret)
library(corrplot)
library(xgboost)
library(cowplot)

# Read datasets
train = fread("Train_UWu5bXk.csv")
test = fread("Test_u94Q5KV.csv")
submission = fread("SampleSubmission_TmnO39y.csv")

# Display column names
names(train)
names(test)

# Display structure of datasets
str(train)
str(test)

# Add Item_Outlet_Sales to test data
test[, Item_Outlet_Sales := NA]
```

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements
- The dataset is provided by Big Mart for the purpose of this competition.
- The R community for providing the necessary packages and documentation.

## Contact
For any questions or issues, please contact Rayyan Ahmed at rayyanahmed265@yahoo.com or https://www.linkedin.com/in/rayyan-ahmed9477/
