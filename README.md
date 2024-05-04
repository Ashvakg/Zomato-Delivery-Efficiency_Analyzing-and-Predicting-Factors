# Delivery Efficiency & Predictive Analysis
Note: Zomato is a food delivery platform in India, similar to Just Eat Takeaway.com and Uber Eats.

# Power BI Dashboard for real-time insights
In the first half of March in Chennai, 
- Bicycles consistently outpaced motorcycles delivery time, indicating potential issues with motorcycle condition or efficiency
- With nearly 37% of deliveries being made by motorcycles, which are in poor condition are resulting in increased average delivery time.
- Additionally, vehicles in better condition delivered faster, underscoring importance of regular maintenance.
- We noted a correlation between sunny weather (usually the case in Chennai during March), higher success rates and faster deliveries.
- Furthermore, a direct link between road traffic density and delivery time was evident, highlighting the importance of real-time traffic data for route planning.
- The intermittent spikes and drops in delivery success rates suggest potential external factors influencing delivery performance such as traffic patterns or order volume fluctuations, warranting further investigation for optimized scheduling and resource allocation.
![dashboard final](https://github.com/Ashvakg/Zomato-Insights/assets/83398283/27b0ff29-f4fb-4af5-b94f-15ff96abc64a)
By prioritizing bicycle usage in Chennai during sunny weather and leveraging traffic data for route optimization, we can enhance delivery efficiency and drive success rates.

# Matplotlib Plots

- Plot_1: Box plot showing percentage of vehicle condition and time taken in minutes
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


