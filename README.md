
**sales prediction for food items sold at various stores**

**Author: Anecho Jeremy Stewart**

**Business problem:**

The goal of this is to help the retailer understand the properties of products and outlets that play crucial roles in predicting sales.

**Data:**

The data provided includes information as follows: 

    1.Item_Identifier 
  
    2.Item_Weight
  
    3.Item_Fat_Content
  
    4.Item_Visibility
  
    5. Item_Type
  
    6. Item_MRP
   
    7. Outlet_Identifier
  
    8. Outlet_Establishment_Year
  
    10. Outlet_Size
  
    11. Outlet_Location_Type
  
    12. Outlet_Type

    13. Item_Outlet_Sales
  
The data was provided by Coding Dojo as part of teh Data Science program.


**Methods**

1. I converted the ordinal data of Outlet size into numerical values.
2. I utilized the mean strategy of the simple imputer to fill in the missing values in the numerical columns.
3. To fill in the missing values in the data, I employed the frequency strategy of the simple imputer.
4. Next, I scaled the data and used the One Hot Encoder to convert all the values into numeric ones, preparing the data for preprocessing.
5. Using the column transformer, I instantiated the Linear Regression model.
6. However, the Linear Regression model exhibited overfitting on the training set and did not perform well on the test data.
7. Consequently, I replaced it with the Random Forest Regressor, which yielded better results with an R2 value of 59% on the test data. This model can be applied to new data, and the RMSE can be taken into account during its usage.

**IMAGES**

![image](https://user-images.githubusercontent.com/57034956/225642723-437ed2dd-5ea5-4e60-8f49-66c42e587893.png)  ![image](https://user-images.githubusercontent.com/57034956/225643175-d0dd71ab-6c51-4976-9357-5073d9f68a33.png)

![image](https://user-images.githubusercontent.com/57034956/225643255-2d83a3f7-965a-48b7-9ebc-c32b33ea6952.png)  ![image](https://user-images.githubusercontent.com/57034956/225642544-665dfc28-543e-49e0-90e1-01dfc823d1fc.png)


**MODEL**

The final model after preprocessing used the Random Forest Regressor to predict sales. It is giving an RMSE of 1113.

**RECOMMENDATION**

**LIMITATIONS AND NEXT STEPS**

For further information: jeremyalekai@gmail.com
