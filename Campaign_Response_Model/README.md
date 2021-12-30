# Campaign Response Model
Campaign Response Model is the model that try to classify the customers who will respond to the new campaign based on data that collected from customers.<br />
## Let Explore!
Let see about our data this time! Here "Retail_Data_Response.csv" and "Retail_Data_Transactions.csv"! This data is about infomation about each customers that collected. Then, we want to predict that how probability of any customers will response to next marketing campaign by the dataset.<br />
## Prepare data
so we got these data "Retail_Data_Response.csv" and "Retail_Data_Transactions.csv" that we know Recency, Frequency, Monetary Value and CLV value from calculated "Retail_Data_Transactions.csv".<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786850-bd42aa11-7035-43df-b3ac-824f9f0128da.png)<br />
<br />
And we know how they response to last campaign from "Retail_Data_Response.csv".<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786874-510e1879-c404-4bf3-a01a-b46538c9407d.png)<br />
<br />
Then we merge 2 table into one.<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786894-8e861b96-43b7-44e7-a65c-2753da0af196.png)<br />
<br />
## Creating train and test dataset
we split data into dataset,train dataset and test dataset<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786925-8efec96e-3e3b-4db0-8713-199ad09f16fe.png)<br />
<br />
and we found that our data is unbalanced.<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786938-68b08c07-b719-4973-bfb6-dff7546546ff.png)<br />
<br />
Then we need to fix it by SMOTE.<br />
<br />
![image](https://user-images.githubusercontent.com/95345008/147786949-6d768fde-e98a-45b4-88e3-ced6f8ab43ef.png)<br />
<br />
## Classification
### Logistic Regression
### Logistic Regression XGBoost
### Random Forests
### Support Vector Machine

## Conclusion
After we fixed imbalanced data, it's more reliable (AUC score is quite high). then we input the data into 3 model of classification then compare results which is better than other. We found that ... model have the highest AUC score and also there aren't overfit because AUC score of test dataset is acceptable. Then, we could use this model for predict response rate to more customers with that accaracy.
