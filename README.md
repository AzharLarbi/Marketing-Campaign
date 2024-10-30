# Marketing Campaign Response Prediction 

This project is focused on predicting customer responses to a marketing campaign using logistic regression, decision trees, and random forests. By analyzing and pre-processing data on customer demographics, previous campaign interactions, and spending habits, we aim to create a reliable model that can forecast customer responses and help optimize future campaigns.

# Project Overview

This project leverages customer data to predict responses to a marketing campaign, helping businesses better target potential responders and improve the efficiency of marketing efforts. The model was initially tested using logistic regression, then refined with decision trees and random forests for potentially higher accuracy and interpretability.

# Data Description

The dataset includes information about customer demographics, spending on various products, interaction with previous campaigns, and response to the current campaign. Key features include:

Customer Information: Income, marital status, education level, number of children and teenagers at home.

Campaign Information: Previous campaign responses (binary), latest campaign response (target), days since last purchase, and complaints.

Spending: Amounts spent on various product categories over the last two years (e.g., meat, wines, sweets).

The target variable is Response: 1 if the customer accepted the campaign offer, 0 otherwise.


# Exploratory Data Analysis (EDA)

During EDA, several insights were drawn:

Income Distribution: Higher income customers showed a stronger likelihood of responding to the campaign.

Campaign Response History: Customers who responded to previous campaigns have a higher probability of responding to the latest campaign.

Education Level: Graduate and Ph.D. holders showed relatively higher response rates.

Complaints: Customers who previously lodged complaints showed a lower likelihood of responding.

# Data Preprocessing

Preprocessing steps included:

Handling Missing Values: Missing values in Income were replaced with the mean.

Feature Scaling: Numerical features were scaled using Min-Max scaling to normalize values.

Categorical Encoding: One-hot encoding was applied to categorical variables (e.g., education level, marital status).

Data Split: The dataset was split into training, validation, and test sets for reliable model assessment.

# Modeling

1. Logistic Regression

An initial logistic regression model was trained as a baseline. It achieved an accuracy of around 92% on the training set, indicating some predictive power.

2. Decision Tree Classifier

Using decision trees, we identified key features influencing customer response, such as the latest campaign response (AcceptedCmp5). The decision tree model achieved approximately 85% validation accuracy after hyperparameter tuning, including adjustments to max_depth.

3. Random Forest Classifier

The final model implemented was a Random Forest Classifier, which performed with around 87% accuracy on the validation set, slightly surpassing the decision tree model. Key hyperparameters tuned included n_estimators, max_depth, max_leaf_nodes, and min_samples_split.

# Evaluation

Evaluation metrics for model accuracy were derived across training, validation, and test sets:

Accuracy: All models were evaluated based on prediction accuracy on validation and test sets, with random forest performing the best.

Confusion Matrix: Visualizations helped assess true positives, false positives, true negatives, and false negatives.

Feature Importance: For tree-based models, feature importance scores were calculated to understand the most influential predictors.

# Further Improvement

Potential improvements to the model include:

Hyperparameter Tuning: Further tuning using grid search or random search could improve model performance.

Alternative Models: Testing additional models such as gradient boosting or ensemble techniques.

Additional Feature Engineering: Creating features that represent interactions between spending patterns and previous responses to campaigns.

# Usage

Load Data: Import and preprocess the marketing campaign dataset.

Run EDA: Use provided visualizations to explore relationships in the data.

Train Models: Follow the notebook steps to train and evaluate the logistic regression, decision tree, and random forest models.

Evaluate: Run the final model on the test set and evaluate using accuracy and feature importance.

# Business Insights

Here are some business insights derived from the model and the data analysis of this marketing campaign:

1. Income Influence on Campaign Response:

   The likelihood of a customer responding to a campaign increases with their income. Targeting higher-income households might improve the campaign success rate.

   This suggests that future marketing efforts could focus on high-income segments to optimize resources and maximize response rates.

2. Previous Campaign Engagement as a Predictor:

   Customers who have engaged in previous campaigns are more likely to respond positively to future campaigns. If a customer accepted one or more of the prior five campaigns, there’s an increased chance they would accept new offers.

   Focusing on re-engaging customers who accepted past campaigns could yield higher conversion rates.

3. Customer Complaints and Campaign Effectiveness:

   Customers who have previously lodged complaints are significantly less likely to respond to campaigns.

   This suggests an opportunity to enhance customer service experiences, particularly for high-value customers, to reduce complaints and improve campaign response rates.

4. Education Level as a Factor:

   Customers with graduate and Ph.D. education levels are more likely to respond to campaigns than those with lower education levels.

   Tailoring offers and messaging to appeal to well-educated segments, perhaps focusing on premium products or more personalized experiences, might be effective.

5. Targeted Campaign Timing and Frequency:

   Recency and purchase frequency metrics indicate that customers who recently interacted with the company, whether through purchases or visits, are more likely to respond to campaigns.

   Timing future campaigns to align with recent engagement windows could increase response rates.
