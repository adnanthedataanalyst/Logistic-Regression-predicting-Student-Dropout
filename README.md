# Logistic Regression predicting Student Dropout

## Introduction

This project aims to develop a logistic regression model for predicting undergraduate student dropouts based on a dataset containing student demographics, academic performance, and socio-economic information. The goal is to create a robust predictive model that can assist educational institutions in allocating resources efficiently, implementing early interventions, and providing support to at-risk students. The analysis is conducted using R programming language, covering data loading, exploration, and logistic regression model building. Additionally, techniques such as confusion matrices and ROC curves are introduced to enhance the accuracy assessment of the predictive model.

**Note**: You can find the RMarkdown file containing codes and results, as well as the Excel file used in this study, in this repository.


 
## Problem Statement

Student dropout is a significant concern for educational institutions, as it not only affects the individual student's academic progress but also influences resource allocation and institutional planning. Identifying factors contributing to student dropout and building an accurate predictive model can enable timely interventions and support systems, ultimately reducing dropout rates. This project addresses the need for an effective logistic regression model to predict student dropouts based on relevant features.

### Key Question

- What factors contribute significantly to student dropout, and how can these factors be leveraged to develop an accurate predictive model?

## Method

### Data Collection

The dataset used in this analysis was collected from Kaggle, providing a diverse set of student information. This dataset includes variables such as demographics, academic performance, and socio-economic factors.

1. **Data Source:**  [Kaggle dataset](https://www.kaggle.com/datasets/thedevastator/higher-education-predictors-of-student-retention).
2. **Dataset Description: ** This dataset, collected by experts from the [VALORIZA Research Center and Polytechnic Institute of Portalegre](https://zenodo.org/records/5777340#.Y7FJotJBwUE), compiles information on students in diverse undergraduate degrees. It includes details from enrollment, such as academic path and socio-economic factors, as well as academic performance at the first and second semesters. The dataset is designed for building classification models to predict students' dropout and success at the end of the course duration.
3. **Code Description Integration:** Integrating Dataset Column Descriptions and Categories from Damiieibikun's GitHub repository appendix, found [here](https://github.com/Damiieibikun/Student-s-Dropout-Prediction-using-Supervised-Machine-Learning-Classifiers). This repository provides the missing information regarding the categorical labels used in the dataset.

### Data Loading and Exploration

The first step involves loading the dataset into R and exploring its structure, including variable names and data types. The dataset is then split into training and testing sets for model development and evaluation.

### Logistic Regression Models

Three logistic regression models (Model 1, Model 2, and Model 3) are built using different combinations of predictor variables. These models are trained on the training dataset and evaluated on the testing dataset. Model summaries provide insights into the significance of predictor variables.

### Predictions and Accuracy Assessment

Predictions are made on both the training and testing datasets using the developed logistic regression models. Confusion matrices are created to assess the model's performance in terms of true positives, true negatives, false positives, and false negatives. Accuracy metrics are calculated based on the confusion matrices.

## Results

The logistic regression models, especially Model 3, demonstrated significant accuracy in predicting student dropouts. The inclusion of variables with a significant impact, such as Application Mode, Tuition fees up to date, Age At Enrollment, Course, Scholarship Holder, and Curricular Units 2nd Sem Grade, further strengthens the model's predictive capabilities.

### Significant Impact Variables

The following variables were found to have a significant impact on student dropout:

- Application Mode
- Tuition fees up to date
- Age At Enrollment
- Course
- Scholarship Holder
- Curricular Units 2nd Sem Grade

#### Additional Threshold Optimization

Using a threshold of 0.3, we achieved an accuracy of 0.82. Threshold optimization based on ROC curves contributes to improved accuracy, providing a comprehensive understanding of the model's performance.


### [Tabealu Dashboard](https://public.tableau.com/views/StudentDropout/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)
This Tableau dashboard visually represents the robust predictive capabilities of logistic regression models in identifying students at risk of dropping out. The highlighted variables provide actionable insights, enabling educational institutions to implement evidence-based interventions and optimize their support systems for improved student outcomes.

## Conclusion

The findings of this study highlight the importance of specific variables in predicting student dropouts. The significant impact of Application Mode, Tuition fees up to date, Age At Enrollment, Course, Scholarship Holder, and Curricular Units 2nd Sem Grade emphasizes the need for tailored interventions targeting these aspects to prevent student attrition. Educational institutions can utilize the developed logistic regression model to identify at-risk students early, enabling proactive support and resource allocation. By understanding the key contributors to dropout, institutions can implement targeted strategies to enhance student success and retention.

## Project Recap:

1. Data Splitting:
-   Divided the dataset into testing and training sets for robust evaluation.

2. Training and Testing:
-   Trained the models using the training dataset.
-   Tested the models using the testing dataset.

3. Model Development:
-   Created logistic regression models (Model 1, Model 2, and Model 3) with varying predictor variables.

4. Threshold Optimization:
-   Initially used a threshold of 0.5, achieving 84% accuracy.
-   Utilized ROC curve analysis to optimize the threshold.

5. Improved Accuracy:
-   Chose a threshold of 0.3, resulting in an accuracy improvement to 82%.
-   Successfully balanced accuracy while reducing true negatives, enhancing the model's overall performance.
