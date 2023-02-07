# Customer Churn
Example and Short Explanation of Customer Churn for Stuller

To do any type of Customer Churn Analysis, we must first understand what customer churn means to the business.
With respect to Stuller or Jewelry Manufacturing,
It could be defined by when Jewelry Shops (Customers) haven't placed an order in x amount of days.

After doing a little bit of research, I found that the inventory turnover ratio for Jewelry stores are 134 days.Or in simple words, it is the number of how many times the company has sold and replenished its inventory.

Assuming a buffer of 2 extra weeks, we can assume that "if a customer has not placed an order within (134+14days) = 148 days, they have churned.

# Data
We get this data by finding the average time between orders and taking anywhere from the 85th-95th percentile of these averages as our target variable, or the thing we want to predict. In this case it is "Churn".

# Outputs
- The Output of the prediction is either "0" (Not Churned), or "1" (Churned)
- This is a Binary Classification Problem
-----------------------------
Since I could not find any data on Jewelry specifically, I have done a similar binary classification of churn with telecom data from DataCamp.

# Results
After comparing various models we find out that RandomForestClassfier has the best accuracy on the test set!

However, 
- Accuracy may not be the best method of evalauting the performance of classification models
- The target variable wsa highly imbalanced as you see in the figures with "not churned" being higher than "Churned" which could highly influence the model
- Recall and Precision would've been some additional metrics we could've used to evaluate the performance of the models.
------------------------------
# Links
- https://www.readyratios.com/sec/industry/5944/
- https://corporatefinanceinstitute.com/resources/accounting/inventory-turnover-ratio/
