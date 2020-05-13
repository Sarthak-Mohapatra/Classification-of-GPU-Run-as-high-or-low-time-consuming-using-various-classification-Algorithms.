# Classification of GPU Run Process as high or low time-consuming using various classification Algorithms.
In this project, we will learn and implement SVM, Decision Trees and XGBoost Algorithms method. The purpose of this project is to 
compare different classification algorithms and test its capabilities for classifying records in a dataset. The dataset contains 
information about GPU kernel performance on matrix multiplication (A * B = C) where, A, B and C are metrices. 
Our goals are highlighted below:

• Implementing SVM, Decision Trees and XGBoost Algorithms to classify the GPU run time as high or low time-consuming process.

In this project, we have performed various experimentations by using different kernels with SVM algorithm, pruning Decision Trees 
and XGBoost to avoid overfitting. Based on various performance measures, the algorithms were evaluated and the best algorithm for 
each dataset was finalized.

## Table of Contents
- General Info
- Variable Description
- Technologies and Methods
- Project Report
- Status
- Contact


## General Info
For this project, we have used the SGEMM GPU kernel performance Data Set available for download at UCI ML Website. The dataset measures 
the running time of various matrix multiplication processes where each matrix is of shape 2048 × 2048. The total number of observations 
in the dataset is 241600. For each test, four runs were performed, and their results were presented in the file. 

For our project, we have taken the average of four runs and based on the Median value, our target/dependent variable was created with 
values higher than median run classified as '1' and below median values were classified as '0'.

## Variable Description
Following table explains the variables in the dataset:
1.  MWG          : per-matrix 2D tiling at workgroup level: {16, 32, 64, 128} (integer)
2.  NWG	         : per-matrix 2D tiling at workgroup level: {16, 32, 64, 128} (integer)
3.  KWG          : inner dimension of 2D tiling at workgroup level: {16, 32} (integer)	
4.  MDIMC        : local workgroup size: {8, 16, 32} (integer)	
5.  NDIMC        : local workgroup size: {8, 16, 32} (integer)
6.  MDIMA        : local memory shape: {8, 16, 32} (integer)	
7.  NDIMB        : local memory shape: {8, 16, 32} (integer)	
8.  KWI	         : kernel loop unrolling factor: {2, 8} (integer)
9.  VWM	         : per-matrix vector widths for loading and storing: {1, 2, 4, 8} (integer)
10. VWN	         : per-matrix vector widths for loading and storing: {1, 2, 4, 8} (integer)
11. STRM         : enable stride for accessing off-chip memory within a single thread: {0, 1} (categorical)	
12. STRN         : enable stride for accessing off-chip memory within a single thread: {0, 1} (categorical)	
13. SA           : per-matrix manual caching of the 2D workgroup tile: {0, 1} (categorical)	
14. SB           : per-matrix manual caching of the 2D workgroup tile: {0, 1} (categorical)	
15. Run1 (ms)    : performance times in milliseconds for 4 independent runs using the same parameters. They range between 13.25 and 3397.08.	
16. Run2 (ms)    : performance times in milliseconds for 4 independent runs using the same parameters. They range between 13.25 and 3397.08.	
17. Run3 (ms)    : performance times in milliseconds for 4 independent runs using the same parameters. They range between 13.25 and 3397.08.	
18. Run4 (ms)    : performance times in milliseconds for 4 independent runs using the same parameters. They range between 13.25 and 3397.08.
19. Avg Run Time : Average Run Time (Average of the 4 runs)

## Technologies and Methods
- Python (Pandas, Numpy, Matplotlib, Seaborn, Scikit-Learn)
- Microsoft Excel
- SVM (Linear, RBF and Polynomial kernel), Decision Tree, XGBoost, K-Fold Cross-validation

## Project Report
The project report is uploaded to the Git-Hub site and can be referenced here: [Project Report](https://github.com/Sarthak-Mohapatra/Classification-of-GPU-Run-as-high-or-low-time-consuming-using-various-classification-Algorithms./blob/master/GPU%20Run%20Time%20classification%20-%20Report.pdf)

## Status
Project is: *finsished*

## Contact
If you loved what you read here and feel like we can collaborate to produce some exciting stuff, or if you just want to shoot a question,
please feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/sarthakmohapatra1990/).
