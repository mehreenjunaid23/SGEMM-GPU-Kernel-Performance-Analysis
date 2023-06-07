# CS3072_Data_Science_final_project

# SGEMM GPU Kernel Performance Analysis
This repository contains the code and analysis for the project "SGEMM GPU Kernel Performance Analysis: Analyzing the Impact of Different Features on GPU Kernel Performance with Regression Analysis".

# Introduction
Graphics Processing Units (GPUs) have become an essential component of modern computing systems due to their ability to perform highly parallel computations. The performance of a GPU kernel, which is a fundamental building block of many GPU-accelerated applications, depends on various factors such as the size of the input data, the precision of the floating-point arithmetic, and the type of GPU used. Understanding the impact of these features on GPU kernel performance is crucial for optimizing GPU-accelerated applications [1].
In this project, we aim to analyze the SGEMM GPU kernel performance dataset [2][3] to explore the impact of different features on GPU kernel performance. The SGEMM dataset is a widely used benchmark dataset that contains performance measurements for the SGEMM GPU kernel, which is a matrix-matrix multiplication kernel. The dataset includes information about various features such as matrix dimensions, precision, and GPU types.

# Problem Statement
The performance of GPU kernels is critical for the overall performance of GPU-accelerated applications. However, the performance of a GPU kernel depends on various factors such as the size of the input data, the precision of the floating-point arithmetic, and the type of GPU used. Therefore, it is essential to understand the impact of these features on GPU kernel performance.

The SGEMM GPU kernel performance dataset provides a valuable resource for analyzing the impact of different features on GPU kernel performance. However, the dataset is large and complex, and it is not immediately clear which features have the most significant impact on the performance of the SGEMM kernel. Therefore, the problem statement of this project is to explore the SGEMM dataset and identify the features that have the most significant impact on GPU kernel performance. Additionally, we aim to develop a regression model that can estimate the performance of the SGEMM kernel based on these features. The proposed regression model can be used to optimize the performance of GPU-accelerated applications that use the SGEMM kernel.

# Data Preprocessing
Before performing the analysis, the dataset is preprocessed to prepare it for further exploration. The dataset is read from the "sgemm_product.csv" file, and a subset of 1000 rows is selected for analysis. Summary statistics of the dataset are computed, and exploratory data analysis (EDA) is conducted to understand the distribution of performance times and the correlation between variables.

# Feature Selection
To identify the features that have the most significant impact on GPU kernel performance, a feature importance analysis is performed using the random forest algorithm. The random forest model is trained on the dataset, and the variable importance plot is generated to visualize the importance of each feature.

# Building Regression Model
A linear regression model is built to estimate the performance of the SGEMM kernel based on the selected features. The model is trained on the preprocessed dataset, and the model summary is printed to examine the regression coefficients and statistical significance of the features.

# Model Evaluation
The performance of the regression model is evaluated using regression metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared (coefficient of determination). The model is tested on a separate testing set, and the predicted performance values are compared to the actual values. A scatter plot is created to visualize the relationship between the actual and predicted values.

# Conclusion
The regression analysis is conducted on a dataset containing 1000 rows and 18 columns to predict the performance of the SGEMM GPU kernels. The regression model exhibits excellent performance with low errors and a high degree.
