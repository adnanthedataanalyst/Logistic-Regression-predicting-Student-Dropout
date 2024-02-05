# Logistic Regression predicting Student Dropout

## Introduction

This project aims to develop a logistic regression model for predicting student dropouts based on a dataset containing student demographics, academic performance, and socio-economic information. The goal is to create a robust predictive model that can assist educational institutions in allocating resources efficiently, implementing early interventions, and providing support to at-risk students. The analysis is conducted using R programming language, covering data loading, exploration, and logistic regression model building. Additionally, techniques such as confusion matrices and ROC curves are introduced to enhance the accuracy assessment of the predictive model.

**Note**: You can find the RMarkdown file containing codes and results, as well as the Excel file used in this study, in this repository.

## Problem Statement

Student dropout is a significant concern for educational institutions, as it not only affects the individual student's academic progress but also influences resource allocation and institutional planning. Identifying factors contributing to student dropout and building an accurate predictive model can enable timely interventions and support systems, ultimately reducing dropout rates. This project addresses the need for an effective logistic regression model to predict student dropouts based on relevant features.

### Key Question

- What factors contribute significantly to student dropout, and how can these factors be leveraged to develop an accurate predictive model?

## Method

### Data Collection

The dataset used in this analysis was collected from Kaggle, providing a diverse set of student information. This dataset includes variables such as demographics, academic performance, and socio-economic factors.

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

Threshold optimization based on ROC curves contributes to improved accuracy, providing a comprehensive understanding of the model's performance.

## Conclusion

The findings of this study highlight the importance of specific variables in predicting student dropouts. The significant impact of Application Mode, Tuition fees up to date, Age At Enrollment, Course, Scholarship Holder, and Curricular Units 2nd Sem Grade emphasizes the need for tailored interventions targeting these aspects to prevent student attrition. Educational institutions can utilize the developed logistic regression model to identify at-risk students early, enabling proactive support and resource allocation. By understanding the key contributors to dropout, institutions can implement targeted strategies to enhance student success and retention.