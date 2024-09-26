**Assignment 11.1**
https://github.com/Nandini1212/used_cars.git

**Summary**
The linked notebook above analyzes the provided used car data by running multiple models on the data to determine the most important car features relative to price.

# used_cars
Analyzing the used cars dataset in Python, here’s a step-by-step guide, starting with loading the data and performing some basic exploratory data analysis (EDA). This will serve as the foundation for building more complex analyses and models later.


**Key Observations:**

**High Mean Absolute Error (MAE):**

The MAE value of 82654 indicates that, on average, your model's predictions deviate from the actual price by about $82,654. This suggests that the model is not performing well and is making large errors in predicting car prices.

**Extremely Low R² Score:**

The R² score of 3.42e-05 (effectively zero) means that the model is explaining almost none of the variance in car prices. In other words, the features you are using (car age and odometer) are not contributing significantly to predicting the price.

**Interpretation:**
1. Car Age and Odometer alone are not sufficient to predict the price of a car accurately.
2. There might be more significant factors that influence the price, such as:
   1. Car Condition (e.g., new, excellent, good, etc.).
   2. Manufacturer and Model (e.g., luxury brands may hold value differently).
   3. Fuel Type (e.g., electric cars may be valued differently from gas-powered vehicles).
   4. Drive Type (e.g., AWD may be valued higher in certain regions).
   5. Transmission Type (manual vs automatic).
3. The high error and low R² suggest that the relationship between the chosen features and car price is weak or non-linear, meaning other approaches or features should be tested. 
    1. Include more features in the model (e.g., condition, manufacturer, fuel, title_status, etc.).
    2. Feature Engineering: Try creating interaction terms or transforming variables. For example, log-transforming skewed features (like price and odometer) may help.
