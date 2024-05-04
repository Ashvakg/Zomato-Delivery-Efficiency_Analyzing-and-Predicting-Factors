# Delivery Efficiency & Predictive Analysis
Note: Zomato is a food delivery platform in India, similar to Just Eat Takeaway.com and Uber Eats.

# Delivery Time:
The graph displays the average time taken to deliver orders across various cities, likely based on historical data. The cities are unnamed, but the average time for each city is represented by a bar.

# Delivery Success Rate:

Another section of the graph shows the delivery success rate, possibly categorized by month and day of the week. However, the details are difficult to discern due to the resolution.

# Correlation Between Delivery Time and Road Traffic Density:
There's a graph suggesting a correlation between delivery time and road traffic density. It appears to show higher delivery times in areas with high traffic density (Jam).

# Factors Affecting Delivery Efficiency:

The image presents several factors that likely influence delivery efficiency:
Delivery location concentration (possibly order density in a specific area)

# Impact on delivery efficiency by vehicle condition (fair, good, excellent, poor)

# Impact on delivery efficiency by weather conditions and vehicle type (sunny, stormy, sandstorms, windy, cloudy, fog)

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


