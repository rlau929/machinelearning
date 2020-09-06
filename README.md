# machinelearning
## Analysis
Balanced Random Forest Classifier:

True Positive: 66
False Positive: 2084
True Negative: 15020
False Negative: 35

precision for high risk is 0.03
recall for high risk is 0.65

precision for low risk is 1.00
recall for low risk is 0.88

f1 score for high_risk is 0.06
f1 score for low_risk is 0.93

balance accuracy score is 0.77

--------------------------------------------------------------------------
Easy Ensemble AdaBoost Classifier:

True Positive: 93
False Positive: 983
True Negative: 16121
False Negative: 8

precision for high risk is 0.09
recall for high risk is 0.92

precision for low risk is 1.00
recall for low risk is 0.94

f1 score for high_risk is 0.16
f1 score for low_risk is 0.97

balance accuracy score is 0.93

### Analysis and Final Recommendation

We performed two different classifiers: Balanced Random Forest (BRF) and Ensemble AdaBoost Classifier (EAC). Overall, EAC showed the best result compared to BRF. EAC showed fewer false negatives and the balance accuracy score is 0.93, significantly more than BRF at 0.77. The precision and recall is also improved for EAC compared to BRF. BRF precision for high risk is 0.03 and low risk is 1.00. BRF recall for high risk is 0.65 for high risk and 0.93 for low risk.

I recommend utilizing matplotlib.pyplot and visualize the data using plt.scatter. Another recommendation is to use the decision tree model and make a prediction using the tree model. The current data contains many columns that can determine the loan status. By using the decision tree, we can determine which prediction model fits best.

## Analysis
Naive Random Oversampling:

True Positive: 77
False Positive: 4680
True Negative: 12424
False Negative: 24

precision for high risk is 0.02
recall for high risk is 0.76

precision for low risk is 1.00
recall for low risk is 0.73

f1 score for high_risk is 0.03
f1 score for low_risk is 0.84

balance accuracy score is 0.74

--------------------------------------------------------------------------
SMOTE Oversampling:
True Positive: 73
False Positive: 6070
True Negative: 11034
False Negative: 28

precision for high risk is 0.01
recall for high risk is 0.72

precision for low risk is 1.00
recall for low risk is 0.65

f1 score for high_risk is 0.02
f1 score for low_risk is 0.78

balance accuracy score is 0.68

--------------------------------------------------------------------------
Undersampling:
True Positive: 68
False Positive: 9997
True Negative: 7107
False Negative: 33

precision for high risk is 0.01
recall for high risk is 0.67

precision for low risk is 1.00
recall for low risk is 0.42

f1 score for high_risk is 0.01
f1 score for low_risk is 0.59

balance accuracy score is 0.54

--------------------------------------------------------------------------
Combination Sampling:
True Positive: 73
False Positive: 7407
True Negative: 9697
False Negative: 28

precision for high risk is 0.01
recall for high risk is 0.72

precision for low risk is 1.00
recall for low risk is 0.57

f1 score for high_risk is 0.02
f1 score for low_risk is 0.72

balance accuracy score is 0.64

### Analysis and Final Recommendation
After performing different analysis using overampling, undersampling, and a combination of both over and undersampling, it is clear that the overall predictors are similar. However, to find out which is best to use, we have to analyze the data. After combing through the data, Naive Random Oversampling showed fewer false positive and false negatives. Additionally, the balance accuracy is much higher at 0.74 compared to the other predictors. Naive Random Oversampling (NRO) precision for high risk is 0.02 and low risk is 1.00. The recall for high risk is 0.76 and 0.73 for low risk. SMOTE Oversampling precision for high risk is 0.01 and low risk is 1.00. The recall for high risk is 0.72 and low risk is 0.65. Undersampling precision high risk is 0.01 and low risk is 1.00. Recall for high risk is 0.67 and low risk is 0.42. Lastly, combination sampling of precision high risk is 0.01 and low risk is 0.72. Recall for high risk is 0.72 and low risk is 0.57.

I recommend utilizing matplotlib.pyplot and visualize the data using plt.scatter. We can visually see if there are any outliers. If there is a significant amount of outliers, we can make a suggestion to use SMOTEENN since SMOTEENN perfectly handles outliers. Another recommendation is to use the decision tree model and make a prediction using the tree model. The current data contains many columns that can determine the loan status. By using the decision tree, we can determine which prediction model fits best.
