# STML2_Homework-2

# *Predicting Diabetes Using Support Vector Machines (SVMs)*


## *Project Overview*
This project explores the use of Support Vector Machine (SVM) models to predict diabetes occurrence based on a variety of demographic, health, and lifestyle factors.  
The goal is to understand how simple, easily available health and behavior information can be used to build predictive models for early identification of diabetes risk.
We used 3 types of SVM kernels — Linear, Radial Basis Function (RBF), and Polynomial — and compared their performances.


## *Dataset Details*
- **Source:** IPUMS Health Surveys, National Health Interview Survey (NHIS) 2022
- **Access Link:** https://github.com/mendible/5322/blob/main/Homework%202/nhis_2022.csv 


## *Methodology*
1. **Feature Selection and Cleaning:**
   - Selected various numeric columns related to demographics, health measures, and lifestyle behaviors.
   - Removed missing values to create a clean dataset.

2. **Data Splitting:**
   - Split the cleaned data into 70% training and 30% testing sets.

3. **Model Training:**
   - Trained three SVM models using different kernels:
     - **Linear Kernel:** Assumes data is linearly separable.
     - **Radial Basis Function (RBF) Kernel:** Allows nonlinear boundaries.
     - **Polynomial Kernel:** Models more complex relationships based on a polynomial degree.
   - Used default parameters with minor hyperparameter tuning as necessary.

4. **Model Evaluation:**
   - Compared models using classification accuracy on the test set.
   - Created a cartoon SVM decision boundary plot using toy data to visualize the behavior of nonlinear decision boundaries.
   

**Key Observations:**
- All models achieved similar high accuracy (~91%), suggesting that the selected features offer strong linear separability.
- Complex nonlinear kernels like RBF and Polynomial did not significantly outperform the simpler linear kernel.


## *Discussion:*
Important predictors identified by the models included:
- Age
- BMI category
- Sleep duration
- Work hours
- Physical activity levels

The results align with medical research, confirming that older age, higher BMI, lack of exercise, and poor sleep habits are strongly linked to higher diabetes risk.
The similar performance across models suggests that even simple linear models can be effective for early diabetes risk prediction based on basic health metrics.


## *Conclusion:*
The project demonstrates that support vector machine models can predict diabetes occurrence with high accuracy using simple, easily measurable features.  
Given the similar performances of linear and nonlinear kernels, linear models offer an efficient, scalable option for building early screening tools in healthcare systems.

Such predictive models could be used by policymakers and health practitioners to encourage preventive health behaviors, reduce diabetes incidence, and optimize early intervention efforts.


## *Files Included:*
- `Practical_Homework-2.ipynb`:  
  Full Jupyter Notebook containing the full code including all data cleaning steps, feature selection, model training, evaluation, and visualization.

- `Poster.pdf`:  
  A summary poster designed for presentation purposes.

- NHIS 2022 Dataset
- NHIS CodeBook


## *Citation:*
Reference:  
Lynn A. Blewett, Julia A. Rivera Drew, Miriam L. King, Kari C.W. Williams, Daniel Backman, Annie Chen, and Stephanie Richards.  
*IPUMS Health Surveys: National Health Interview Survey, Version 7.4* [dataset]. Minneapolis, MN: IPUMS, 2024.  
[https://doi.org/10.18128/D070.V7.4](https://doi.org/10.18128/D070.V7.4)
