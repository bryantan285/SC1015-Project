**Heart Disease Prediction Mini Project**

Overview

In this mini project, we aim to predict and determine the causal factors for heart disease using a dataset containing 12 variables. Our dataset comprises 7 numerical variables and 5 categorical variables. We have selected 7 variables for analysis: age, sex, resting blood pressure, cholesterol level, maximum heart rate, old peak, and the presence of heart disease.

Aim of this project

To use machine learning to predict the occurrence of heart disease using various factors. We also hope that more prediction models will be applicable in hospitals not only for heart disease but also for various other conditions.

Exploratory Analysis

Conducted statistical distribution analysis to understand the relationships between numerical variables.

Utilized boxplot, histogram, and violin plot for visualization.

Created a heatmap of the correlation coefficient matrix to identify correlations between variables.

Data Cleaning

We identified that there were 172 outliers with a cholesterol level of 0 and removed them from the dataset as they are invalid and felt that the outliers were messing up the models.

After training the models with the new dataset, the resulting data showed a higher prevalence of negative heart disease cases.

We also observed changes in the correlation coefficients post data cleaning, with the most significant changes in the old peak variable (from 0.4 to 0.5).

Correlation Analysis

Categorized variables into good predictors and poor predictors of heart disease based on correlation coefficient heatmap.

Good predictors: age, maximum heart rate, and old peak.

Poor predictors: Fasting blood sugar, cholesterol, and resting blood pressure.

Machine Learning models used for Prediction & Analysis

1. **Linear Regression** - We chose this due to its simplicity and interpretability, making it easier to understand the relationship between the dependent and independent variables. Experimenting with various factor combinations, we sought to identify significant factors affecting the presence of heart disease. Initially, we explored all factors and gradually narrowed down to using only the "good" factors, characterized by higher correlation coefficients.
1. **Dummy Classifier** - To act as a benchmark for other models as it classifies the data using simple rules. It also makes predictions without looking for patterns, which is beneficial for complex, complicated and biased datasets.
1. **Random Forest** - Given its reputation for high accuracy and robustness against overfitting, the Random Forest Classifier was selected as a viable alternative. Upon evaluation, it outperformed the Dummy Classifier as expected. Although exhibiting more True Positives, it also incurred some False Positives.
1. **Multi-class decision tree** - It operates as a non-parametric model, signifying their lack of assumptions regarding data distribution. This attribute grants them flexibility, enabling the handling of diverse distributions effectively. Moreover, decision trees autonomously determine the most pertinent features within the dataset.
1. **Up-sampling data -** We Increased the number of Patients with heart disease of the dataset to balance it with patients without heart disease. This balanced dataset enables machine learning models to learn more effectively from both classes, thereby reducing the risk of biased predictions that favor the majority class.

Conclusion/What we learnt:

- Hands-on experience gained using various classification models for data analysis.
- Employed data manipulation techniques like up-sampling to improve prediction analysis.
- Acknowledged that 100% accuracy is not achievable, but identified factors better at predicting heart disease.
- Initial assumption about cholesterol as a leading predictor was disproved by low correlation with heart disease.
- Heatmap analysis showed patients with and without heart disease clustered around cholesterol levels of 200-300.
- Advanced models performed well in mitigating data overfitting compared to the dummy classifier.
- Emphasized the importance of maintaining a balanced dataset for improved prediction accuracy and reliability.

Slides

The slides show the summary of our project. It covers the overall objectives of our project, data cleaning, exploratory analysis using different models and visualization as well as the conclusions and lessons that we learnt.

Individual Contributions

Seann: 

- Machine Learning exploration
- Decision Tree Classifier
- Random Forest Classifier
- Dummy Classifier

Wei Jie:

- Linear Regression
- Determined Explained Variance (R^2) and Mean Squared Error (MSE)
- Comprehend and conclude findings, commented the codes

Bryan:

- Exploratory Analysis and data visualization
- Evaluation of variables and resampling of data
- Video editor and slides design

**References**

<https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction>

<https://slidesgo.com/theme/coronary-heart-disease>

