# Directional Analytics for Day Trading in Stock Market

6-day consecutive closing price for the stock under consideration is being taken. These 6 days consecutive closing prices will be tabulated week on week for the entire dataset and will be utilized as 6 different feature variables for building the classification Model.

The difference between 7th and 8th day Closing price is determined. If the 8th day closing price is seen an increase from the 7th day by 0.7% or more, the direction of the closing price can be made as positive.

If the 8th day closing price is seen a decrease from the 7th day by -0.7% or less, the direction of the closing price can be made as negative. Between -0.7% and 0.7%, the direction of the closing price for the stock under consideration can be treated as sideways. 

For data within the 0.7% and -0.7% band, usually the advice to the investor will be to hold on to existing portfolios and wait for the direction of the closing price to show as either negative or positive change. If there is a negative change, usually the advice to the investor will be to not to invest in such a circumstance. If there is a positive change the investor will be suggested to invest.

It is to be determined how many times the positive changes are identified by predicting and how many times positive changes are there in the actual data. This will be utilized to evaluate how many times true positives were detected and how many times the false positives were predicted in the prediction. Similar process to be followed for detecting true negatives and false negatives. Similar process to be followed for detecting true neutrals and false neutrals. Based on prediction accuracy, it can be suggested whether to invest or not to invest to the prospective investor.


Computation is being done to evaluate whether it is positive change, negative change or no change between 7th and 8th day closing price. The rule is being set to determine as to what has to be seen as direction change.0.7% change,1% change and 1.5% change -these are different classes of direction for which rule is being set which is to be followed for computing the direction change as either positive change, negative change or no change.

once it is determined say for example 0.7% change has the best prediction accuracy among all different classes of direction namely 0.7% change,1% change and 1.5% change then the range of consecutive days to be utilized as feature variable is increased to 10 days. Therefore,10-day consecutive closing price for the stock under consideration is being taken. These 10 days consecutive closing prices will be tabulated week on week for the entire dataset and will be utilized as different feature variables for building the classification Model.

Similar process is again repeated for range of consecutive days to be utilized as feature variable increased to 14 days. The prediction accuracy is determined to confirm that say 0.7% change has the best prediction accuracy among all different classes of direction even when range of consecutive days to be utilized as feature variable is increased to 14 days.

Technical Indicators

Similarly, all technical indicators can be utilized in Technical Analysis to build another sets of classification Models. All different types of technical indicators namely momentum indicators, trend indicators, volatility indicators, volume indicators can be utilized as feature variables based on the input dataset and different classification models can be built to determine their prediction accuracy. 

Generally Open price, High price, low price, close price and volume for the stock under consideration will be utilized to derive feature variables from technical indicators. These derived feature variables will then be used as the feature variables to predict the direction of the close price. The Actual direction of the close price is estimated as percentage change of the close price between upper-band +0.5% and lower band -0.5% for all technical indicators-based classification Models.

Modelling Algorithms used are Logistic Regression Classifier,Decision Tree Classifier,Random Forest Classifier,K Neighbours Classifier and XG Boost Classifier.

Metrics used for Data Evaluation are precision,recall,accuracy score and Roc AUC score.
