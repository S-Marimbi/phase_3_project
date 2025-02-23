# phase_3_project
# Telecom Churn Prediction

## Overview
SyriaTel, a telecommunications company, is experiencing high customer churn, leading to revenue loss. The goal of this project is to build a machine learning classifier that predicts customer churn based on customer behavior and demographic features. With these insights, SyriaTel can proactively address customer concerns and improve retention strategies.

## Business and Data Understanding

### Business Context
- Customer churn is a major challenge in the telecommunications industry due to intense competition.
- Retaining customers is more cost-effective than acquiring new ones.
- Understanding churn behavior enables targeted interventions that improve customer satisfaction and reduce revenue loss.

### Stakeholders
1. **Business Executives** – Need strategic insights to reduce churn and increase profitability.
2. **Marketing Team** – Uses predictions to create customer retention campaigns.
3. **Customer Service Team** – Focuses on high-risk customers to improve engagement.
4. **Data Science Team** – Develops and refines predictive models for better churn identification.

### Dataset
- The dataset contains customer information, including service usage patterns, account details, and contract type.
- The target variable is **churn** (binary: 1 for churn, 0 for retention).
- Key features include customer tenure, monthly charges, total call minutes, and contract type.

## Modeling
### Approach
1. **Baseline Model:** Started with **Logistic Regression** as a simple baseline.
2. **Decision Tree Model:** Applied hyperparameter tuning to improve performance.
3. **Random Forest Model:** Implemented an ensemble approach to enhance accuracy and generalization.

### Hyperparameter Tuning
- **Decision Tree:** Tuned `max_depth`, `min_samples_split`, and `min_samples_leaf` for optimal results.
- **Random Forest:** Increased the number of estimators and adjusted tree depth to balance bias and variance.

## Evaluation
### Metrics Used
- **Accuracy**: Measures overall correctness of predictions.
- **Precision**: Ensures that when churn is predicted, it is correct.
- **Recall**: Captures the proportion of actual churns correctly identified.
- **F1-score**: Balances precision and recall for better performance assessment.

### Results Comparison
- **Logistic Regression:** Provided a baseline but lacked predictive power.
- **Decision Tree:** Improved performance but risked overfitting.
- **Random Forest:** Achieved the highest accuracy and F1-score, making it the most reliable model for deployment.

## Conclusion
### Key Findings
- **Random Forest performed the best**, accurately identifying churn-risk customers.
- **Important features** influencing churn include **monthly charges, tenure, and total call minutes**.
- **False positives** could lead to unnecessary customer interventions, increasing costs.
- **Model limitations** include sensitivity to shifting customer behaviors and potential dataset biases.

### Recommendations
- **Targeted retention strategies**: Focus on high-risk customers identified by the model.
- **Customer engagement improvements**: Personalized offers based on key churn predictors.
- **Regular model updates**: Retrain the model periodically to adapt to changing customer behavior.
- **A/B Testing**: Experiment with different retention campaigns to optimize intervention strategies.

This analysis equips SyriaTel with data-driven insights to minimize churn and enhance customer loyalty.

