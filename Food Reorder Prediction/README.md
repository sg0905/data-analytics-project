# **Food Reorder Prediction

This project focuses on predicting the likelihood of customers placing repeat orders, which can be highly beneficial for food delivery companies like Swiggy, Uber Eats, and Zomato. By leveraging customer data, including demographics, location, and feedback, companies can gain deeper insights into customer preferences and behaviors. This helps refine marketing strategies, boost customer retention, and improve overall user experience. Additionally, identifying high-demand regions can assist in better resource allocation, optimizing delivery routes, and improving delivery times. Such predictive analytics enhance operational efficiency and give companies a competitive advantage in the dynamic food delivery market.


**About the Dataset**

The dataset comprises information from customers who use online food delivery services. It includes data on demographics, geographical locations, and customer feedback related to their food ordering experience. The dataset can be analyzed to understand customer behavior, identify high-demand locations, and improve delivery times by strategically allocating delivery partners.

**Columns and Descriptions**


| Sl. No. | Column                      | Description                                          |
|---------|-----------------------------|------------------------------------------------------|
| 1       | Age                          | Age of the customer                                  |
| 2       | Gender                       | Gender of the customer                               |
| 3       | Marital Status               | Marital status of the customer                       |
| 4       | Occupation                   | Occupation of the customer                           |
| 5       | Monthly Income               | Monthly income of the customer                       |
| 6       | Educational Qualifications   | Educational qualification of the customer            |
| 7       | Family Size                  | Number of members in the customer’s family           |
| 8       | Latitude                     | Latitude coordinate of the customer's location       |
| 9       | Longitude                    | Longitude coordinate of the customer's location      |
| 10      | Pin Code                     | Pin code of the customer's location                  |
| 11      | Output                       | Indicates whether the customer will order again      |
| 12      | Feedback                     | Feedback provided by the customer  


:

**Data Preprocessing**


Choosing Required Columns: Only the necessary columns relevant to the prediction task were selected.
Handling Null Values: Missing data was addressed using appropriate strategies.
Handling Specific Attributes:
Age: Processed and binned into categories for better analysis.
Gender: Categorical values were encoded.
Marital Status: Converted to numerical format for modeling.
Occupation: Encoded based on types of occupation.
Monthly Income: Handled for better representation in the model.
Educational Qualifications: Transformed into a numerical format.
Feedback: Feedback data was cleaned and encoded.
Pin Code: Processed to extract useful information about location.
Output: Binary classification target indicating whether the customer will reorder.
Data Splitting: The dataset was split into training and testing sets.
Oversampling: Oversampling techniques (such as SMOTE) were applied to handle class imbalance.
Machine Learning Models

**Several machine learning models were tested to find the best performer:**


Decision Tree: Simple and interpretable, but not the best accuracy.
Random Forest: Provided the highest accuracy among all models.
SVM (Support Vector Machine): Strong performance, but not as accurate as Random Forest.
XGBoost Classifier: Powerful model but slightly less accurate than Random Forest.
Best Performing Model
Random Forest: Achieved the highest accuracy in predicting repeat orders.

**Model Testing**
After training, the Random Forest model was tested on unseen data to evaluate its performance.

**Data Preprocessor Design**
A custom data preprocessor was designed to handle new inputs efficiently, ensuring the data pipeline is streamlined for future predictions.