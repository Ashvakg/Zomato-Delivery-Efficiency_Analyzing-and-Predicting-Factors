# Zomato Delivery Efficiency & Predictive Analysis

# Power BI Dashboard for real-time insights
![dashboard final](https://github.com/Ashvakg/Zomato-Insights/assets/83398283/27b0ff29-f4fb-4af5-b94f-15ff96abc64a)

# Matplotlib Plots

- Plot_1: Box plot showing percentage of vehicle condition and average time taken in minutes
![image](https://github.com/Ashvakg/Zomato-Insights/assets/83398283/c0a151be-96ec-4be4-bb8b-3afea0a47032)

- plot_2: Top 10 Cities with shortest time taken to deliver an order
![image](https://github.com/Ashvakg/Zomato-Insights/assets/83398283/a665379a-5265-4372-8820-ac7eaf4748a0)

- plot_3: Scatterplot correlation time taken to deliver and road traffic density
![image](https://github.com/Ashvakg/Zomato-Insights/assets/83398283/e0b77665-55d7-49b9-804e-43cecdc7042c)

# Machine Learning for Predictive Analysis
Built Machine Learning algorithms to predict time taken (minutes) to deliver an order 
( Refer: Zomato_Predicted.csv to view the data and Prediction_XGBoost for the algorithm, Linearregression)

- Linear Regression: with features Delivery_Person_Age, Ratings, Distance(Calculated using Haversine) Mae of 6.5
- Random Forest: Considering Features and with RFE(Ranking top 5 feautes)  Delivery_Person_Age, Ratings, Distance (Calculated using Haversine), Road_traffic_density, Vehicle_condition, Type_of_vehicle - Mae 5.2
- XGBoost with Considering features: Delivery_person_Age, Delivery_person_Ratings, Weather_conditions, Road_traffic_density, Vehicle_condition, Type_of_vehicle, Distance_km, City_Type, Type_of_order - Mae:4.8


