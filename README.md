# SC1015-Mini_Project

## About


## 1. Problem Formulation
- Dataset we used:
- Outcome of our project:
     - Identify important attributes that correlate strongly to output performance FP32 (GFLOPS)
     - Why FP32? because it is the industry standard
     - Modify the factors to improve the GPU performance
       
- Motivation:
     - As technology of manufacturing of chips advances, we cannot improve all aspects of chip manufacturing, so we suggest to focus on attributes that are very strongly correlated to output performance.

## 2. Data Preparation and Cleaning
- Data Preparation:
     - We scrape ___ website for data using API
 
- Data Cleaning:
     - We then identify which factors that may be useless for example OpenGL.
     - We also drop columns that are repeated.
     - We then drop columns with incomplete information.
     - We also drop columns that are not related with chip attribute but related to performance output for example, Texture Rate, Pixel Rate, FP16, FP64

## 3. Exploratory Data Analysis
Multi-Variate data analysis: 
In our cleaned dataset, we have 17 attributes and 1 response variable (FP32 (GFLOPS))
We plotted the count of Arbitrary generations of chips (based on the chip Architecture)
We use violin plot to see the distribution of all numerical variables
We also plotted the correlation heatmap




## 4. Machine Learning

Models Used:
1. Random Forest Regression
     xxx



## 5. Conclusion 
-  Data Driven Insights
-  Model Comparison
-  What did we learn


Generational performance 

Compare generational gaps 

Compare the performance progress of the two companies over the years 

Compare transistor density 

Predictive modeling of future GPU generations 

Predict Nvidia or AMD is doing better 

