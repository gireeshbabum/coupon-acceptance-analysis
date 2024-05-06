Analyzing Coupon Acceptance Trends among Drivers

Path to python notebook :  https://github.com/gireeshbabum/coupon-acceptance-analysis/blob/main/coupon-acceptance-analysis/notebooks/couponcode.ipynb

Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

Deliverables

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing github repository as your first portfolio piece.


Data Description

Keep in mind that these values mentioned below are average values.
The attributes of this data set include:
1. User attributes
    * Gender: male, female
    * Age: below 21, 21 to 25, 26 to 30, etc.
    * Marital Status: single, married partner, unmarried partner, or widowed
    * Number of children: 0, 1, or more than 1
    * Education: high school, bachelors degree, associates degree, or graduate degree
    * Occupation: architecture & engineering, business & financial, etc.
    * Annual income: less than $12500, $12500 - $24999, $25000 - $37499, etc.
    * Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    * Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    * Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    * Number of times that he/she eats at a restaurant with average expense less than $20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    * Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
2. Contextual attributes
    * Driving destination: home, work, or no urgent destination
    * Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
    * Weather: sunny, rainy, or snowy
    * Temperature: 30F, 55F, or 80F
    * Time: 10AM, 2PM, or 6PM
    * Passenger: alone, partner, kid(s), or friend(s)
3. Coupon attributes
    * time before it expires: 2 hours or one day


Output

Based on the analysis, here are some hypotheses about drivers who accepted the bar coupons:

1. Overall Acceptance Rate: The proportion of bar coupons accepted is approximately 41%. This indicates that a significant portion of the distributed bar coupons were accepted.

2. Frequency of Bar Visits: Drivers who went to a bar more than 3 times a month had a notably higher acceptance rate (approximately 77%) compared to those who went 3 or fewer times (approximately 37%). This suggests that frequent bar-goers are more inclined to accept bar coupons.

3. Age and Bar Visits: Drivers over the age of 25 who visit bars more than once a month had a higher acceptance rate compared to all other drivers, indicating that older individuals who frequent bars may be more receptive to bar coupons.

4. Passenger Demographics and Occupations: Drivers who go to bars more than once a month, had passengers that were not kids, and had occupations other than 'Farming Fishing & Forestry' showed a higher acceptance rate. This implies that certain passenger demographics and occupations may influence the likelihood of accepting bar coupons.

5. Marital Status and Bar Visits: Drivers who go to bars more than once a month, had passengers that were not kids, and were not widowed also exhibited a higher acceptance rate, suggesting that marital status may play a role in accepting bar coupons.

6. Age Group: Drivers under the age of 30 who visit bars more than once a month had a slightly higher acceptance rate compared to all other drivers, indicating that younger individuals who frequent bars may also be more inclined to accept bar coupons.

7. Income and Restaurant Visits: Drivers who visit cheap restaurants more than 4 times a month and have an income less than 50K displayed a higher acceptance rate, implying that lower-income individuals who frequent cheap restaurants may be more receptive to bar coupons.

Overall, these findings suggest that various factors such as age, frequency of bar visits, passenger demographics, occupation, marital status, and income level may influence the likelihood of drivers accepting bar coupons.


Based on the analysis, here are some hypotheses regarding drivers who accepted the CoffeeHouse coupons:

1. Overall Acceptance Rate: Approximately 49.9% of the CoffeeHouse coupons distributed were accepted, indicating a moderate level of acceptance among drivers.

2. Frequency of CoffeeHouse Visits: Drivers who visited a CoffeeHouse more than 3 times a month had a significantly higher acceptance rate (67.5%) compared to those who visited 3 or fewer times (44.9%). This suggests that frequent CoffeeHouse visitors are more likely to accept CoffeeHouse coupons.

3. Age and CoffeeHouse Visits: Drivers over the age of 25 who visited CoffeeHouses more than once a month exhibited a higher acceptance rate (62.6%) compared to other drivers, indicating that older individuals who frequent CoffeeHouses may be more receptive to CoffeeHouse coupons.

4. Passenger Demographics and Occupations: Drivers who visited CoffeeHouses more than once a month, had passengers that were not kids, and had occupations other than 'Farming Fishing & Forestry' demonstrated a higher acceptance rate (64.2%). This suggests that drivers with specific passenger demographics and occupations are more likely to accept CoffeeHouse coupons.

5. Marital Status and CoffeeHouse Visits: Similarly, drivers who visited CoffeeHouses more than once a month, had passengers that were not kids, and were not widowed also showed a higher acceptance rate (63.5%). This indicates that marital status may influence the likelihood of accepting CoffeeHouse coupons.

Overall, these findings suggest that various factors such as age, frequency of CoffeeHouse visits, passenger demographics, occupation, and marital status may influence the likelihood of drivers accepting CoffeeHouse coupons.


