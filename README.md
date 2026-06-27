## Observations

The model achieved an accuracy of 86% on the test data, which is a good result 
for this dataset.

The dataset is imbalanced. Out of 10,000 customers, only about 20% (2037) 
actually churned, while 80% (7963) did not churn. Because of this imbalance, 
the model performs much better at predicting customers who did NOT churn 
(95% recall) compared to customers who DID churn (only 49% recall).

This means the model misses about half of the customers who actually churned. 
In a real business case, this is a problem, because the bank would want to 
correctly identify customers who are about to leave so they can take action 
to retain them.

The precision for the "Churned" class (71%) is better than its recall (49%), 
which means when the model predicts a customer will churn, it is often right, 
but it fails to catch many churn cases overall.

The model was trained for only 5 epochs with a simple architecture (one hidden 
layer of 64 neurons). Training accuracy and validation accuracy both improved 
steadily across epochs, showing the model was learning properly without 
overfitting.
