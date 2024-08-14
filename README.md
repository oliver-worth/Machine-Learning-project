# Megaline Mobile Plan Recommendation Model
![Best Cell Phone Plans](mobileplan.png)
## Project Overview
Megaline, a mobile carrier, has identified that many of their subscribers are still using legacy plans. To encourage users to switch to newer plans—Smart or Ultra—Megaline aims to develop a predictive model that analyzes subscribers' behavior and recommends the most suitable plan. The goal of this project is to create a classification model with an accuracy threshold of 0.75 to correctly predict whether a subscriber should be on the Smart or Ultra plan.

## Data Source
The dataset provided contains monthly behavior data for subscribers who have already switched to one of the newer plans. The data includes:

- calls: Number of calls made by the subscriber.
- minutes: Total duration of calls in minutes.
- messages: Number of text messages sent.
- mb_used: Internet traffic used in megabytes.
- is_ultra: Indicator of the subscriber's current plan (Ultra - 1, Smart - 0).

## Objective
- Primary Goal: Develop a classification model to predict whether a subscriber should be recommended the Smart or Ultra plan based on their behavior data.
- Accuracy Threshold: Achieve an accuracy of at least 0.75 on the test dataset.
- 
## Tools and Libraries
- Pandas: For data manipulation and analysis.
- Scikit-learn: For model building, training, and evaluation.
- Project Instructions
- Data Loading: The dataset is loaded from the specified path.
- Data Splitting: The data is split into training, validation, and test sets.
- Model Development: Various models, including Decision Trees, Random Forest, and Logistic Regression, were trained and evaluated.
- Hyperparameter Tuning: Hyperparameters for each model were adjusted to optimize performance.
- Model Evaluation: The model's performance was evaluated using accuracy, precision, recall, and F1 score metrics on the test set.

## Results Summary
Confusion Matrix Breakdown:

Smart Plan (Class 0):

- Precision: 82% of the predictions for the Smart Plan were correct.
- Recall: 92% of the actual Smart Plan users were correctly identified.
- F1 Score: 86%, combining both precision and recall.

Ultra Plan (Class 1):

- Precision: 74% of the predictions for the Ultra Plan were correct.
- Recall: 53% of the actual Ultra Plan users were correctly identified.
- F1 Score: 61%, combining both precision and recall.

## Overall Model Performance:

- The model performs well in identifying subscribers for the Smart Plan, with high precision and recall.
- The model struggles more with identifying Ultra Plan users, particularly in terms of recall, where it only correctly identifies 53% of the Ultra Plan users.
## Conclusion
- The developed model meets the accuracy threshold of 0.75, but there is a noticeable imbalance in performance between predicting the Smart and Ultra plans.
- The model is highly effective at predicting the Smart Plan but needs further refinement to improve recall for the Ultra Plan.
- Future work could focus on improving the model's ability to correctly identify Ultra Plan users, potentially through additional data preprocessing, feature engineering, or experimenting with different modeling techniques.
