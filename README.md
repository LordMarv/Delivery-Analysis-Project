# Delivery-Analysis-Project
Delve into the world of food delivery with the Zomato Delivery Dataset.  Analyzing delivery person ratings, delivery times, and vehicle conditions to evaluate performance and identify areas for improvement.

<h1>ZOMATO DELIVERY PERFORMANCE ANALYSIS</h1>

![Dashboard Preview](zamato%20capture.PNG)

<h3>Case Study Outline</h3>

<h4>Business Problem:</h4>

Zomato wants to understand what makes deliveries fast, reliable, and well-rated, and where performance is breaking down. We will analyse delivery person ratings, delivery times, and vehicle conditions to identify areas of improvement.

 The goal of this analysis, in simple terms, is to understand who performs best, under what conditions, and why.
 
<h4>Tools:</h4>

Excel, Power Query, and Pivot tables.

<h3>Data Overview</h3>

Source: Zomato Delivery Operations Dataset

<h4>Features:</h4>

•	ID: Unique identifier for each delivery.

•	Delivery_person_ID: Unique identifier for each delivery person.

•	Delivery_person_Age: Age of the delivery person.

•	Delivery_person_Ratings: Ratings assigned to the delivery person.

•	Restaurant_latitude: Latitude of the restaurant.

•	Restaurant_longitude: Longitude of the restaurant.

•	Delivery_location_latitude: Latitude of the delivery location.

•	Delivery_location_longitude: Longitude of the delivery location.

•	Order_Date: Date of the order.

•	Time_Ordered: Time the order was placed.

•	Time_Order_picked: Time the order was picked up for delivery.

•	Weather_conditions: Weather conditions at the time of delivery.

•	Road_traffic_density: Density of road traffic during delivery.

•	Vehicle_condition: Condition of the delivery vehicle.

•	Type_of_order: Type of order (e.g., dine-in, takeaway, delivery).

•	Type_of_vehicle: Type of vehicle used for delivery.

•	Multiple_deliveries: Indicator of whether multiple deliveries were made in the same trip.

•	Festival: Indicator of whether the delivery coincided with a festival.

•	City: City where the delivery took place.

•	Time_taken (min): Time taken for delivery in minutes.

<h3>DATA CLEANING PROCESS</h3> using Power Query:

•	Removed duplicates from the data starting from ID

•	Filtered out incorrect or null values from Restaurant longitude and latitude, as well as Delivery_location longitude and latitude.

•	Converted Order_date to a datetime data type

•	Added a new column called prep_time. Prep_time =time_order_picked-time_ordered

•	Added a distance column by calculating distance from restaurant to delivery location using the haversine formula

<h3>KEY FINDINGS:</h3>

<h3>Delivery Time:</h3>

•	High Traffic and Traffic jams significantly increase delivery time; this is seen as both have an average delivery time of 27 and 31 minutes, respectively.

•	Cloudy and foggy weather tends to cause the worst delays among the weather conditions, with each having an average delivery time of 29 minutes

•	Festival period analysis has a strong correlation with delivery time. The average time period during festival time and off-time shows that festival analysis is a strong predictor of delays

•	The Delivery analysis shows the peak order hour to be the 21st hour, and the delivery time is among the highest, with an average delivery time of 31 minutes.

<h3>Delivery Person Performance:</h3>

•	The average rating for all Delivery persons combined is 4.64. which is considerably above average showing customers are satisfied with the service rendered all round.

•	While all ages have a high average rating, the analysis shows that the Younger delivery persons have a higher average delivery rating, with the ages 20 and 23 having averages of 4.69 each.

•	The Correlation between ratings and Vehicle condition is weak. This means that vehicle condition is not a strong indicator of poor ratings.

<h3>Distance:</h3>

•	According to the distribution of distance against delivery time, it appears that distance alone has no bearing on the delivery time. Perhaps other factors in conjunction with distance may cause delay.

•	The average distance is 27km

<h3>Multiple Deliveries:</h3>

•	Multiple deliveries do increase the average delivery time, as seen with the variable 3, which has an average time of 48 minutes,


<h3>RECOMMENDATIONS:</h3> 

•	Prioritize investigating the habits and working patterns of the top-rated delivery person to identify what brings such high results.

• Use Findings to organise training and inform onboarding programs across all age groups to drive performance ratings.

•	The business should cap multiple deliveries to at most 2 to reduce delivery time.

•	The business should invest in real-time routing tools during peak hours and festival periods.

•	The business should encourage delivery operations during festival periods.  


