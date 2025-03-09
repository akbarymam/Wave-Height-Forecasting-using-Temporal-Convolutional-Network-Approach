# Wave Height Forecasting using Temporal Convolutional Network Approach
Wave height prediction is crucial in several sectors, including environmental monitoring and resource management in coastal areas. Traditional methods, such as statistical re gression, fail to discern complex patterns in time series data, resulting in reduced predicted accuracy. This research highlights improved wave height forecasting using Temporal Convolutional Networks (TCN) for wave height prediction. The TCN is a deep learning architecture recognised for its efficacy in processing sequential data. We selected a case study on the coast of Pacitan, East Java, Indonesia, which confronts the Indian Ocean and is recognised for its significant wave activity. We utilise nine years of historical simulated time series wave data from high-resolution wave simulations. The data is segmented into training and testing sets across several circumstances to ascer tain which configuration yields superior predictive outcomes. We employ the model for predicting over periods of 3, 7, 14, and 21 days. Hyperparameter optimisation is conducted using RandomSearch and KerasTuner algorithm to improve model performance. We evaluate the accuracy of the TCN model in comparison to various deep learning model, including CNN and Transformer, by analysing performance metrics such as Root Mean Squared Error (RMSE) and Coefficient of Determination (R²). The results demonstrate that TCN improves forecasting accuracy, as shown by decreased RMSE with 0.0170 score and increased R² values of 0.9930 over the 3-day forecasting period.

We investigated wave condition is the coastal region in Pacitan Bay, East Java, Indonesia, that dominantly consisting of swell generated in the Indian Ocean. Pacitan Bay has an important role as it serves as a route or stopover for coal-carrying barges, especially when facing bad weather conditions or high waves. Accurate wave data in Pacitan’s coastal area is obtained using nested high-density wave simulations with the SWAN model. 

![image](https://github.com/user-attachments/assets/7bb5ef83-a45b-4410-ad57-f6978817e993)

This work uses a range of scenarios and training data periods to investigate, across 3, 7, 14, and 21-day intervals, how well the TCN forecasts results. Random search methods of hyperparameter tuning assist the TCN model to be optimum. Two methods of evaluation for the model are Coefficient of Determination (R²) and Root Mean Square Error (RMSE).

## Wave Data

![image](https://github.com/user-attachments/assets/d7b473ed-a590-4e9a-a13c-43b9dd2e0b2b)


This project utilises high-resolution wave data obtained through wave down scaling in the coastal area of Pacitan, East Java, Indonesia. The simulation was performed continously for nine years using SWAN wave model. incorporating global wind data sourced from ERA5 by ECMWF The simulation occurs within three nested domains.The smallest domain in the Pacitan region is located on the southern coast of Java Island,with coordinates spanning from 7°55’ to 8°17’ South latitude and 110°55’ to 111°25’ East longitude.

## Result

![image](https://github.com/user-attachments/assets/ae46baf2-8893-40ef-8887-f516966050cd)

To attain optimal model performance, the training data is segmented into various scenarios based on efficiency considerations and computing power limitations. This Scenarios used for comparative analysis to identify the most effective predictive outcomes, with each scenario covering 1 year (from March 31, 2022, to March 31, 2023), 3 years (from March 31, 2020, to March 31, 2023), and 5 years (from March 31, 2018, to March 31, 2023). To test these scenarios we performed a 21-day forecasting using the default parameters for the model.

![image](https://github.com/user-attachments/assets/9b3dc9ed-8f85-4039-bdb2-62925c973ca0)

Table above ilustrated the performance enhancement of the TCN after hyperparameter adjustment. The coefficient of determination (R²) values climbedwhile the RMSE values fell, signifying enhanced predictive accuracy for the model. In the TCN model, the R² value increased from 0.9734 to 0.9870, and the RMSE fell from 0.0272 to 0.0172.

![image](https://github.com/user-attachments/assets/59543d9b-ffa1-40b6-b094-c570b8828010)

At the final stage, we performed 3, 7, 14 and 21-day forecasting to compare the performance of each prediction step (day) as shown in Table above. This case indicated that TCN exhibited ideal performance across all predicting intervals, obtaining an R² value of 0.9930 and an RMSE value of 0.0170 in 3-day forecasting.

![image](https://github.com/user-attachments/assets/f11af67c-2ff5-4f75-a7b7-e02a14960fac)
![image](https://github.com/user-attachments/assets/88ae8012-4a01-47bf-b59c-d5e926a7cc7c)
![image](https://github.com/user-attachments/assets/9fe6a3db-e7a5-4b6d-8ec2-060adf5996ae)
![image](https://github.com/user-attachments/assets/d9c2cf64-5e23-46ca-937a-1267fa384ea4)



