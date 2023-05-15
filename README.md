# credit-risk-classification

The data has been split to train and test groups. 

Then, the variables (X) and response (Y) were determined.

Logistic Regression Model performed on data and the results of the modeling showed that:

"Healthy loans are predicted with a precision of 100%, which is optimal, and a recall of 99%, which is also optimal. High-risk loans has a smaller precision of 85%, and a recall of 91%, which we hope we can improve by dealing with the imbalance data.The f1 score, which balances prediction and recall is equal to 88%, which is only OK."

For the second part, "RandomOverSampler" was conducted and by resampling the data it was found that:

The model predicted significantly better the high-risk loans when including resampling. Particularly, there is an amazing improvement in the recall from 0.91 to 1.00! That means that all of the negative falses (declare healthy loan when they were a highly risky) now are correctly labeled as 1 (high-risk loan). This is awesome in terms of controling the cost associated to the default of loans. Without resampling, the bank would have to absorve the default cost of those 57 high-risk loans badly classified by the previous model. Fortunately, when applying the resample to control the imbalance, we see that that cost of default is totally prevented by the improved model.

The opportunity cost associated to the 102 loans wrongly classified as high-risk loans is still there, though. The resampling wasn't able to improve in recognizing that caracterization as we see the same 0.85 precision score in both models.

Healthy loans

Healthy loans are well classified in both models. Since it was a very good classification using original data, the addition of oversample did not improve significantly the classification.

Conclusions

There is a massive improvement in the overall accuracy of the logistic regression model classification on loan risks when using resampled data.
