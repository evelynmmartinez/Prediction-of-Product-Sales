# **Prediction of Product Sales for Big Mart**
## **Big Mart's prediction of Sales**
### **Author:** Evelyn Martinez

### **Project Overview:**
This project focuses on predicting product sales for Big Mart, a food chain retailer. The primary objective is to analyze the data related to products and outlets to provide insights and recommendations for improving sales.

##### Data Dictionary
For a comprehensive understanding of the data, refer to the Data Dictionary for detailed explanations of the various features and their meanings.

##### Source of data:https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
<img width="528" alt="data_dictionary" src="https://github.com/evelynmmartinez/Prediction-of-Product-Sales/assets/136510004/379ccacd-532a-4b71-957b-ceb33d770903">\

The data used in this project is sourced from the Big Mart Sales III competition on Analytics Vidhya. The dataset contains valuable information about products, outlets, and sales, providing a foundation for our analysis.

#### Key Visualizations:
To gain initial insights, we have created two key visualizations:

#### Sales by Item Visibility: A visual representation of how item visibility affects sales.
![item_visibility](https://github.com/evelynmmartinez/Prediction-of-Product-Sales/assets/136510004/d691b3a3-e3c4-4326-b00d-1d9f4fa58520)


#### Item Count by Category: A figure illustrating the distribution of items across different category types.
![item_type](https://github.com/evelynmmartinez/Prediction-of-Product-Sales/assets/136510004/eb5c553d-3455-46ec-a0d2-6d6d29116af3)

### Results and Business Recommendations:
Our analysis has led to valuable insights into sales patterns and trends. Through rigorous modeling and fine-tuning, we selected the Random Forest model as the optimal choice for predicting product sales. After tuning, this model exhibited improved performance metrics, including a reduced Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE), indicating more accurate predictions. 

### Linear Regression Coefficient Plot:
![coefficients_top15](https://github.com/evelynmmartinez/Prediction-of-Sales/assets/136510004/7a813c2a-1cf1-428f-8643-9efa000013ba)
 
**The top three most important coefficients are:**

- Outlet_Type_Supermarket_Type3: The model shows that Supermarket Type 3 significantly impacts sales compared to other store types. It suggests around 1,590 more units sold in this kind of supermarket compared to the rest.

- Outlet_Type_Supermarket_Type1: Similarly, Supermarket Type 1 also has a positive effect on sales, with around 234 more units sold compared to other types of supermarkets in the dataset.

- Item_Type_Seafood: The model indicates that 'Seafood' items sell about 95 more units compared to other types of food items.
  
### Feature Importance - Decision Tree Regressor
![feature importance_dec tree regressor](https://github.com/evelynmmartinez/Prediction-of-Sales/assets/136510004/b8c82d94-a930-465e-993a-c471d67be128)

 Item_MRP: This feature is the most critical according to the model. The (MRP) has the highest impact, indicating that price variations significantly influence sales.

Outlet_Type_Grocery Store: The type of outlet being a "Grocery Store" holds the second most substantial importance in predicting sales. 

Item_Visibility: The visibility of items in stores plays a notable role. It suggests that higher visibility or exposure of items positively influences their sales.

Outlet_Type_Supermarket Type3: This outlet type has moderate importance in predicting sales. Items sold in this supermarket significantly impact the sales.

Item_Weight: The weight of the item also holds moderate importance (importance score of 0.0534) in predicting sales. 

Outlet_Establishment_Year: The year of establishment of the outlet carries some importance, suggesting a moderate effect on sales predictions.

Outlet_Size, Outlet_Location_Type, Item_Type_Fruits and Vegetables, Item_Type_Snack Foods, and others: These features have lower importance scores, indicating a comparatively lesser influence on the predicted outcome
![image](https://github.com/evelynmmartinez/Prediction-of-Sales/assets/136510004/10abd423-09bf-49b4-9706-61cbf7b1f795)

### summary plot - bar version

![shap_explained](https://github.com/evelynmmartinez/Prediction-of-Sales/assets/136510004/0a830a7b-5074-40f1-abe3-76dbbdb71dbd)
**SHAP vs. your original feature importances**

- The features with the same rank are Item_MRP and Outlet_Type_Grocery Store. The only third feature in this model is Outlet_Type_Supermarket Type 3 and in the feature importance model, it was Item_Visibility. 

### a summary plot - dot version

![shap_summary_dot](https://github.com/evelynmmartinez/Prediction-of-Sales/assets/136510004/eba1fdd0-c071-432c-a828-42e0c2553003)
- The Item_MRP is the most impactful feature, suggesting a prediction of more sales in relation to the Item_MRP. 
- The Outlet_Type_Grocery Store has a negative distribution in the plot. Suggesting this type of outlet impacts the sales negatively. 
- The Outlet_Type_Supermarket Type 3 skews more towards a positive prediction of sales if the outlet is a type 3. 

