# Customer Coupon Acceptance Analysis

# Will a Customer Accept the Coupon?
# Context:

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

# Overview:

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

# Data:

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

# Deliverables:

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing github repository as your first portfolio piece.

# Methodology:

CRISP-DM framework was used to do the analysis of the dataset

## Business Understanding: 
The first step was to understand the problem statement defined in module #5.1 exercise
## Data Understanding: 
Spent time to look at the initia data, then perform data description, data exploration and data quality. 
## Data Preparatation:
After analyzing the data, focused on fixed all missing values and incorrect data to create a good dataset that can be used for the remainder of the project
In some cases, I had to reformat the data to ensure it has the correct datatype
This allowed for data analysis, reporting, and making conclusions

The Jupyter notebook uses Python, Panda, Numpy, Matplotlib, Seaborn, and Plotly packages.

# Results:
Based on the data analysis, a few key observations have been done:
- If a customer has been to a location, the rate of acceptance is high for Coffee House, Bar, and Cheap Restaurant
- If the customer has not been to a location, the rate of acceptance is low for Expensive Restuarant
- Age did not matter for both Coffee House and Cheap Restaurants. All age groups acceptance is higher
- For Bar visits, age group does matter. Customers between 25 and 35 have higher chance of acceptance

# Next Steps:
- Analyze the data further for weather condition, time of day, income, and age.
- Analyze if the customer will consider the coupon if it was for opposite the direction
- Analyze how the destination choice impacts acceptance - Traveling to Home, Work, or no urgent place.
- Analyze if the age and gender has a critical impact on the coupon acceptance. Also, does having a partner or friend along with the customer influence acceptance of coupon

# Repository Structure: 
- /data - folder holds the coupons.csv data file used by the jupyter notebook
- README.md - this file provides all the details about the project
- Coupon Analysis_JF.ipnb jupyter notebook has the python code for this project
