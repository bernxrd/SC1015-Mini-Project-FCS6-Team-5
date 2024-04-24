# SC1015-Mini_Project

## About
Mini-project for SC1015 (Introduction to Data Science and Artificial Intelligence). 
Dataset used: List of Nvidia and AMD chips with detailed statistics about their features, manufactured from 2006 to 2024.

# Contributors
Lab Group FCSE Team 5: 
- Chen Xinyu
- Bernard Iskandar
- Shao YingZhan

## Problem Formulation

Objectives:

1. Given a set of chip statistics or features, develop a predictive model to estimate chip performance.The response variable for chip performance is FP32 in Gflops as it is the most commonly used variable for comparison of performance. 
2. Identify important features that affect FP32 in Gflops. 
       
Motivation / Application:

Chip companies generally create a range of chips that prioritises different features to cater to different market segments and sectors. The predictive model can be helpful for manufacturers to predict the performance of their chips based on the chips' statistics and help manufacturers to better evaluate different design options and make informed decisions to optimize their chip performance.

Extra objective: Since pixel rate and texture are close indicators of computing performance, we attempted to use pixel rate and texture rate with FP32 in Gflops as part of a multioutput regressor model as well. 
     
## Data Preparation and Cleaning
- Data Preparation:
     - We scraped Techpowerup.com for data on Nvidia and AMD chips manufactured from 2006 to 2024. 
 
- Data Cleaning:
     - We first dropped columns most likely to have no effect on chip performance, such as OpenGL.
     - We also dropped columns that are repeated.
     - We then dropped columns with incomplete information.
     - We then dropped columns that will not be used as predictor variables, such as texture rate and pixel rate.
     - We standardised the units of measurement for each variables. For instance, FP32 values in Tflops are converted to Gflop and Memory Size in GB to MB.
  
In the cleaned dataset, we have 14 predictor variables and 1 response variable (FP32 in Gflops).

## Exploratory Data Analysis

Multi-Variate data analysis: 
- plotted the histogram of Arbitrary generations of chips (based on the chip Architecture).
- plotted violin plot to observe the distribution of all numerical variables.
- plotted heatmap to observe correlation between each variable.

## Machine Learning Models

1. Random Forest Regression
2. XGBoost
3. Gradient Boosting Regression
4. Multi-Output Regression (Extra)

## Conclusion 
- Transistors (millions) and GPU Clock (MHz) are most important features. Thus, research should focus on this two variable to improve chip performance. 
- Memory Size, Bus Width and Memory Clock have significant impact as well, indicating that memory configurations impact GPU performance alongside processing capabilities.Memory configurations could be a key indicator in differentiating the chip in the market. 
- Certain Architecture like Architecture_RDNA 3.0 and Architecture_Ampere improves  GPU capabilities. Research and development in architecture to improve product performance and market positioning. 



## What did we learn
-  Scraping data from website into excel sheet. 
-  All machine learning models used in this project.
-  Level of importance of each feature for predicting FP32.
-  Goodness of fit of each machine learning model for our particular dataset to predict FP32. 



