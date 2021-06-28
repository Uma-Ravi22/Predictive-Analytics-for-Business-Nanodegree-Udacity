# Predictive-Analytics-for-Business-Nanodegree-Udacity

# Umadevi Balasubramanian

This repository contains projects for Udacity's Predictive Analytics for Business Nanodegree: https://www.udacity.com/course/predictive-analytics-for-business-nanodegree--nd008t
# Part 1: Problem Solving with Advanced Analytics
Learn a structured framework for solving problems with advanced analytics. Learn to select the most appropriate analytical methodology. 
Also was introduced both Linear Regression and Multiple Linear Regression.

## Project 1: Predicting Diamond Prices
This project is designed for three main reasons:

- To give you a feel for what you’ll be doing throughout the Nanodegree Program
- To introduce you to Udacity’s project submission and review process
- To make sure you feel comfortable with the basics before you begin. If it feels too easy, don't worry. We have some great stuff in store for you.

### Project Overview
A jewelry company wants to put in a bid to purchase a large set of diamonds, but is unsure how much it should bid. In this project, you will use the results from a predictive model to make a recommendation on how much the jewelry company should bid for the diamonds.

### US Number System
All numbers that will be presented in this Nanodegree program will be based on the US numbering system where 5,269 is "five thousand two hundred sixty nine" and 158.1 is "one hundred fifty eight point one" where 1 is a decimal number. This is very important so please take note of this.

### Project Details
A diamond distributor has recently decided to exit the market and has put up a set of 3,000 diamonds up for auction. Seeing this as a great opportunity to expand its inventory, a jewelry company has shown interest in making a bid. To decide how much to bid, the company’s analytics team used a large database of diamond prices to build a linear regression model to predict the price of a diamond based on its attributes. You, as the business analysts, are tasked to apply that model to make a recommendation for how much the company should bid for the entire set of 3,000 diamonds.
The following diagram represents the analysis at a high level. Since the model is already built, your analysis will focus on the right side of the diagram.

![image](https://user-images.githubusercontent.com/76995852/123613633-455f1b00-d80c-11eb-8253-ea564ddf97c4.png)

The linear regression model provides an equation that you can use to predict diamond prices for the set of 3,000 diamonds. The equation is below:

Price = -5,269 + 8,413 x Carat + 158.1 x Cut + 454 x Clarity

 Step 1 – Understand the data: There are two datasets.

- diamonds.csv contains the data used to build the regression model.
- new_diamonds.csv contains the data for the diamonds the company would like to purchase.

![image](https://user-images.githubusercontent.com/76995852/123613518-2b253d00-d80c-11eb-86c0-9d122dd967a1.png)

Both datasets contain carat, cut, and clarity data for each diamond. Only the diamonds.csv dataset has prices. You'll be predicting prices for the new_diamonds.csv dataset.

Carat represents the weight of the diamond, and is a numerical variable.
Cut represents the quality of the cut of the diamond, and falls into 5 categories: fair, good, very good, ideal, and premium. Each of these categories are represented by a number, 1-5, in the Cut_Ord variable.
Clarity represents the internal purity of the diamond, and falls into 8 categories: I1, SI2, SI1, VS1, VS2, VVS2, VVS1, and IF. Each of these categories are represented by a number, 1-8, in the Clarity_Ord variable.

### Note: Transforming category variables to ordinal variables like this is not always appropriate, but we’ve done it here for simplicity.
Step 2 – Calculate the predicted price for diamond: For each diamond, plug in the values for each of the variables into the linear model (equation). Then solve the equation to get the estimated, or predicted, diamond price. We suggest using a spreadsheet tool like Excel, Numbers, or Google Sheets. You could also do it in Alteryx and/or Tableau if you already have your license.

Step 3 – Make a recommendation: Now that you have the predicted price for each diamond, it’s time to calculate the bid price for the whole set. Note: The diamond price that the model predicts represents the final retail price the consumer will pay. The company generally purchases diamonds from distributors at 70% of that price, so your recommended bid price should represent that.

<HR>

 ## Project 2: Predicting Catalog Demand.
 
### The Business Problem
You recently started working for a company that manufactures and sells high-end home goods. Last year the company sent out its first print catalog, and is preparing to send out this year's catalog in the coming months. The company has 250 new customers from their mailing list that they want to send the catalog to.

Your manager has been asked to determine how much profit the company can expect from sending a catalog to these customers. You, the business analyst, are assigned to help your manager run the numbers. While fairly knowledgeable about data analysis, your manager is not very familiar with predictive models.

You’ve been asked to predict the expected profit from these 250 new customers. Management does not want to send the catalog out to these new customers unless the expected profit contribution exceeds $10,000.

### Details
- The costs of printing and distributing is $6.50 per catalog.
- The average gross margin (price - cost) on all products sold through the catalog is 50%.
- Make sure to multiply your revenue by the gross margin first before you subtract out the $6.50 cost when calculating your profit.
 
Write a short report with your recommendations outlining your reasons why the company should go with your recommendations to your manager.
 
### Steps to Success
 
Step 1: Business and Data Understanding
Your project should include:

A description of the key business decisions that need to be made.
Note: Clean data is provided for this project, so you can skip the data preparation step of the Problem Solving Framework.

Step 2: Analysis, Modeling, and Validation
Build a linear regression model, then use it to predict sales for the 250 customers. We encourage you to use Alteryx to build the best linear model with your data.

Note: For students using software other than Alteryx, if you decide to use Customer Segment as one of your predictor variables, please set the base case to Credit Card Only.

However, feel free to use any tool you’d like. You should create your linear regression model and come up with a linear regression equation.

Once you have your linear regression equation, you should use your linear regression equation to predict sales for the individual people in your mailing list.

Step 3: Writeup
Once you have your predicted or expected profit, write a brief report with your recommendation to whether the company should send the catalog or not.
Hint: We want to calculate the expected revenue from these 250 people in order to get expected profit. This means we need to multiply the probability that a person will buy our catalog as well. For example, if a customer were to buy from us, we predict this customer will buy $450 worth of products. At a 30% chance that this person will actually buy from us, we can expect revenue to be $450 x 30% = $135.
 
<HR>
# Part 2: Data Wrangling
Data Wrangling is at the core of all data activity. In this course you learn how to work with different data types,dirty data, and outliers. 
You will also learn how to reformat data and join data from different sources together.

## Project 3: Creating An Analytical Dataset.
 
### The Business Problem
Pawdacity is a leading pet store chain in Wyoming with 13 stores throughout the state. This year, Pawdacity would like to expand and open a 14th store. Your manager has asked you to perform an analysis to recommend the city for Pawdacity’s newest store, based on predicted yearly sales.

Your first step in predicting yearly sales is to first format and blend together data from different datasets and deal with outliers.

Your manager has given you the following information to work with:

The monthly sales data for all of the Pawdacity stores for the year 2010.
NAICS data on the most current sales of all competitor stores where total sales is equal to 12 months of sales.
A partially parsed data file that can be used for population numbers.
Demographic data (Households with individuals under 18, Land Area, Population Density, and Total Families) for each city and county in the state of Wyoming. For people who are unfamiliar with the US city system, a state contains counties and counties contains one or more cities.
 
<HR>
# Part 3: Classification Models
Classification models are a powerful tool for business analyst. In this course, you learn more about binary and non-binary classification models 
and how to use them to drive business insights.
 
## Project 4: Predicting Default Risk.
 
### The Business Problem
You work for a small bank and are responsible for determining if customers are creditworthy to give a loan to. Your team typically gets 200 loan applications per week and approves them by hand.

Due to a financial scandal that hit a competitive bank last week, you suddenly have an influx of new people applying for loans for your bank instead of the other bank in your city. All of a sudden you have nearly 500 loan applications to process this week!

Your manager sees this new influx as a great opportunity and wants you to figure out how to process all of these loan applications within one week.

Fortunately for you, you just completed a course in classification modeling and know how to systematically evaluate the creditworthiness of these new loan applicants.

For this project, you will analyze the business problem using the Problem Solving Framework and provide a list of creditworthy customers to your manager in the next two days.

You have the following information to work with:

- Data on all past applications
- The list of customers that need to be processed in the next few days
 <HR>

# Part 4: A/B Testing
Helping businesses make the best decisions is an essential part of Business Analysis. Planning and executing the analysis of an AB test allow 
you to provide confident recommendations. In this course, you learn how to create, execute, and analyze an AB test.
 
## Project 5: A/B Test - A New Menu Launch.
### The Business Problem
Round Roasters is an upscale coffee chain with locations in the western United States of America. The past few years have resulted in stagnant growth at the coffee chain, and a new management team was put in place to reignite growth at their stores.

The first major growth initiative is to introduce gourmet sandwiches to the menu, along with limited wine offerings. The new management team believes that a television advertising campaign is crucial to drive people into the stores with these new offerings.

However, the television campaign will require a significant boost in the company’s marketing budget, with an unknown return on investment (ROI). Additionally, there is concern that current customers will not buy into the new menu offerings.

To minimize risk, the management team decides to test the changes in two cities with new television advertising. Denver and Chicago cities were chosen to participate in this test because the stores in these two cities (or markets) perform similarly to all stores across the entire chain of stores; performance in these two markets would be a good proxy to predict how well the updated menu performs.

The test ran for a period of 12 weeks (2016-April-29 to 2016-July-21) where five stores in each of the test markets offered the updated menu along with television advertising.

The comparative period is the test period, but for last year (2015-April-29 to 2015-July-21).

You’ve been asked to analyze the results of the experiment to determine whether the menu changes should be applied to all stores. The predicted impact to profitability should be enough to justify the increased marketing budget: at least 18% increase in profit growth compared to the comparative period while compared to the control stores; otherwise known as incremental lift. In the data, profit is represented in the gross_margin variable.

You have been able to gather three data files to use for your analysis:

- Transaction data for all stores from 2015-January-21 to 2016-August-18
- A listing of all Round Roasters stores
- A listing of the 10 stores (5 in each market) that were used as test markets.

  <HR>
# Part 5: Time Series Forecasting
Time Series Forecasting is a powerful analytical tool. In this course, you learn how ETS and ARIMA models are used to forecast data and 
how they deal with trends and seasonality. These skills will be evaluated in the final project.
<HR>
# Part 6: Segmentation and Clustering
Segmentation and Clustering are effective methods for finding patterns in your data. In this course, you learn how to prepare data to be 
clustered appropriately and interpret results.
 
## Project 6: Combining Predictive Techniques.
 
The capstone project has three main tasks, each of which requires you to use skills you developed during the Nanodegree program.
 
### Task 1: Store Format for Existing Stores
Your company currently has 85 grocery stores and is planning to open 10 new stores at the beginning of the year. Currently, all stores use the same store format for selling their products. Up until now, the company has treated all stores similarly, shipping the same amount of product to each store. This is beginning to cause problems as stores are suffering from product surpluses in some product categories and shortages in others. You've been asked to provide analytical support to make decisions about store formats and inventory planning.
 
### Task 2: Store Format for New Stores
The grocery store chain has 10 new stores opening up at the beginning of the year. The company wants to determine which store format each of the new stores should have. However, we don’t have sales data for these new stores yet, so we’ll have to determine the format using each of the new store’s demographic data.

### Task 3: Forecasting
Fresh produce has a short life span, and due to increasing costs, the company wants to have an accurate monthly sales forecast.
Task 3: Forecasting Produce Sales
You’ve been asked to prepare a monthly forecast for produce sales for the full year of 2016 for both existing and new stores. To do so, follow the steps below.

Note: Use a 6 month holdout sample for the TS Compare tool (this is because we do not have that much data so using a 12 month holdout would remove too much of the data)

Step 1: To forecast produce sales for existing stores you should aggregate produce sales across all stores by month and create a forecast.

Step 2: To forecast produce sales for new stores:

- Forecast produce sales (not total sales) for the average store (rather than the aggregate) for each segment.
- Multiply the average store produce sales forecast by the number of new stores in that segment. 
- For example, if the forecasted average store produce sales for segment 1 for     March is 10,000, and there are 4 new stores in segment 1, the forecast for the new stores in     segment 1 would be 40,000.
- Sum the new stores produce sales forecasts for each of the segments to get the forecast for all new stores.
 
Step 3: Sum the forecasts of the existing and new stores together for the total produce sales forecast.
