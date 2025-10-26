Pokémon K-Means Clustering

K-Means clustering was applied to Pokémon stats with k = 2 to 8.

Best number of clusters: k = 2 (based on silhouette score)
So adding more clusters did not improve cohesion much. So



Fraud Detection with Decision Tree

Confusion matrix:
True negatives: 1,270,662
False positives: 219
False negatives: 274
True positives: 1,369
Performance metrics:
Precision for fraud = 0.86, Recall = 0.83, F1-score = 0.85
ROC AUC = 0.916
Top important features: newbalanceOrig (0.41), oldbalanceOrg (0.37), amount (0.17), step (0.037)

Interpretation: The model is pretty good at identifying non fraud transactions and good at detecting fraud. Account balances and transaction amount are the most predictive features.