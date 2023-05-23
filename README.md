![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/b44236c9-91ef-4426-83f9-bb58b5b7cad8)


Customer churn is one of the biggest problems facing telecom companies at the moment.Research has shown that the average monthly churn rate among the top 4 wireless carriers in the US is 1.9%. A telecom company wants to know the reasons why customers churn and also find ways to ensure that customers do not churn.
Objectives


* Explore customer demographics, usage patterns, and service features to uncover potential churn drivers.
* Develop predictive models to forecast customer churn and evaluate their accuracy.
* Generate actionable insights and recommendations for the company to reduce churn and improve customer retention.
* Propose strategies and initiatives that can be implemented to mitigate churn, based on the identified insights and predictive models.

* ```State:``` The state in which the customer resides.
* ````Account length:``` The number of days the customer has been with the service provider.
* ```Area code:``` The telephone area code associated with the customer's phone number.
* ```Phone number:``` The customer's phone number.
* ```International plan:``` Whether the customer has an international calling plan (yes or no).
* ```Voice mail plan:``` Whether the customer has a voice mail plan (yes or no).
* ```Number vmail messages:``` The number of voice mail messages the customer has.
* ```Total day minutes:``` The total number of minutes the customer used during the day.
* ```Total day calls:``` The total number of calls the customer made during the day.
* ```Total day charge:``` The total charge for the customer's daytime usage.
* ```Total eve minutes:``` The total number of minutes the customer used during the evening.
* ```Total eve calls:``` The total number of calls the customer made during the evening.
* ```Total eve charge:``` The total charge for the customer's evening usage.
* ```Total night minutes:``` The total number of minutes the customer used during the night.
* ```Total night calls:``` The total number of calls the customer made during the night.
* ```Total night charge:``` The total charge for the customer's nighttime usage.
* ```Total intl minutes:``` The total number of international minutes the customer used.
* ```Total intl calls:``` The total number of international calls the customer made.
* ```Total intl charge:``` The total charge for the customer's international usage.
* ```Customer service calls:``` The number of customer service calls made by the customer.
* ```Churn:``` Whether the customer has churned or not (True or False).

EDA

![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/8c21e5cf-b68d-461c-9ae6-d4329a3958dc)

showing the distribution of customers across the top 10 states, with each bar representing the count of customers in a particular state


![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/24dea966-874e-4660-849a-5bd851c80e02)

This data represents three area codes which are not normally distributed

![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/0ca9b746-29a4-4cd4-99cc-9185916b7a6d)

The churn column is normally distributed 
* If the customer service is call is high chances of churn are high

![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/1783575d-a16a-4486-b52a-004c7bdff1ab)

The higher the customer service calls the higher the rate of the customer churn

![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/fc1f268b-85e3-4dcb-a9e1-01ae930eb1c3)

Time period the customer has been with the service provider does not affect the churn rate




Models: Logistic Regression
        Decision Tree
        Random Forest
        K Nearest Neighbor
        
Model Results

![image](https://github.com/shamwamachristine/Customer-Churn-Prediction/assets/124347570/de074d0c-90c1-4bc4-aa46-1a0a3338373c)


Conclusions

* Random Forest: The Random Forest model has the highest AUC score of 0.912, indicating better class separation compared to the other models. This suggests that the Random Forest model performs well in distinguishing between the classes.

* Decision Tree: The Decision Tree model has an AUC score of 0.822, which is lower than the Random Forest model but still indicates a good level of class separation. The Decision Tree model performs reasonably well in distinguishing between the classes
* Logistic Regression: The Logistic Regression model has an AUC score of 0.776936. While it has a lower AUC score compared to the Random Forest and Decision Tree models, it can still provide some level of class separation, although not as strong as the other models.
* KNN: The KNN model has the lowest AUC score of 0.673, indicating relatively weaker class separation compared to the other models. The KNN model may struggle to distinguish between the classes effectively.

Based on the AUC scores alone, the Random Forest model appears to be the best performer among the four models.











