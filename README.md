# ANALYTICAL REPORT FOR MARKETING TEAM

---
## Summary of Analytical Process
The following enlisted analytical processes administered on the customer dataset to ensure the dataset is clean and accurate
for further analysis

### 1. **Understanding the data**
Every analytics task to solving a problem(business or non-business) first begin with a in-depth familiarity of the data’s 
Available in the dataset. This step emphasis on not only understanding each uniqueness of features but also the sector our data belongs to in the industry and knowing the data types
and categories that we will be handling e.g. categorical and numerical data and whether they are ordinal, discrete or Continuous

---
### 2. Performing data wrangling
Preparing the data for further analysis is preponderant with this step. loading  our dataset to Python 
(Programming language) environment, cleaning our dataset to make sure any values like null, missing and outlier that will affect the efficiency of the analysis is removed or engineered 
with arithmetic methods like mean, median and mode. This steps also entails data engineering and  data enriching.

FEATURE SELECTION AND ENGINEERING
Selecting the feature or column that align with our business problem, and also altering this column to 
pin-point some specific value from the data e.g. filtering the month from a date column etc.

---
### 3. Feature Scaling
This is a method applied on our feature of interest mostly, which in our customer dataset is the customer_retention_score and customer_profitability_score. The method makes sure that the features 
involved contribute squarely to our analysis permeating a normal distribution of our feature data, thereby ameliorating or eliminating skewness from our data of interest

---
### 4. MODELING
Having thoroughly completed the step above, then our dataset is now ready and fit for modelling. KMeans was used to model the customer ratings dataset. 
KMeans is an unsupervised python model that studies the particular behavior pattern of a dataset and group  the values with similar behavior pattern into a cluster designated by number which ranges 
from 0 to target number clusters input in the model. In our customer ratings dataset, number of cluster input is 2, this saw the model clustering the customer dataset into 2, designating 0(cluster1) 
as Loyal customer with positive customer_retention_score and 1(cluster2) designating Less Loyal customer with a negative customer_retention_score simultaneously with their respective Customer_profitability_score.This model was used because it best align with our business objective of grouping our customers based on retention
Score and profitability score respectively and using this information to further understanding our customer sets.

## Explanation of clear and actionable insights
Using the KMeans modelling, customer was group into four category viz:
- **Loyal and Profitable Customer Group**
- **Loyal and less-Profitable Customer Group**
- **Less Loyal and Profitable Customer Group**
- **Less Loyal and Less-Profitable Customer Group**

---
### LOYAL AND PROFITABLE CUSTOMER GROUP(Count:73)
Customer in this category  have a positive retention score and profitability score, which connotes from customer guild that this set of customers have a positive manner or behaviour  to our service
and thus have a good loyal attitude to Banana bikes over our competitors regardless of price differences or level of convenience. A positive profitability score of this set of customers also indicates 
that they have been consistent with this loyalty behaviour with Banana Bikes overtime or for a long time.  

**Marketing strategy:** 
With this set of customers the  goal is to enhance their satisfaction and continually encourage repeat purchase possible 
marketing options include:  

- **Exclusive Rewards:** 

	Offer exclusive rewards such as discounts, early access to new products, or special gifts for loyal customers.  

- **Tiered Benefits:** 
	
 	Create a tiered loyalty program where the more they spend, the better the rewards, encouraging higher spend.  

- **Birthday/Anniversary Discounts:** 

	Offer special discounts on their birthdays, anniversaries, or other significant dates.  

- **Incentivized Referrals:** 
	Encourage them to refer friends and family by offering rewards for successful referrals, such as discounts or bonus
 	points in a loyalty program.

---
## Loyal and Less-Profitable Customer Group (Count: 60)
Customer in this category  have a positive retention score and negative profitability score, which connotes from customer 
guild that this Set of customers have a positive manner or behaviour  to our service and thus have a good loyal attitude to Banana bikes over our Competitors regardless of price differences or level of 
convenience. A negative profitability score further gave an insights that this set of customers are not  consistent with patronizing Banana Bikes over time, this an issue I believe we should look into and
have the appropriate marketing strategy in place to improve the consistent patronage of Banana Bikes by this customer group.  

**Possible marketing strategy:**  
The goal is to improve their profitability while maintaining or enhancing  loyalty. Below are possible marketing strategy 
that can help achieve this goal.  
- **EMAIL CAMPAIGNS:**  
	
 	Send personalized emails that highlight products they may like, based on their purchase history, along with limited-time offers.
- **SUBSCRIPTIONS:**  
	
 	Offer a subscription service for products they frequently purchase. This ensures regular sales and can lock in the customer 
        for a longer period.
- **SEASONAL PROMOTIONS:**  
	
 	Leverage seasonal promotions to offer these customers special deals that are time-limited. This creates urgency and can
        lead to increased purchases during promotional periods.

---
## Less Loyal and Profitable Customer Group:
After thorough modelling and analysis, no record was found for this set of customer Groups.  

---
## Less Loyal and Less Profitable Customer Group(Count: 67)
Customers in this category have negative retention score and profitability score respectively. This connotes that customers in the category do not have a positive manner towards our services, 
consequently this customers are less loyal and only patronize during cost effective promotions or convenience of course as a result of this they are less profitable  

**Possible marketing strategy:**
The goal is to increase engagement, and satisfaction and possible marketing strategy includes.  
 
- **Double Points/Rewards:**

	Occasionally offer double points or rewards on purchases. This can motivate less engaged customers 
	to make a purchase to earn extra rewards.  

- **Early Access to Sales:**

	Offer this customer segment early access to sales or new product launches. Exclusivity can make 
	them feel valued and encourage them to shop more often.  
		       
- **Content Marketing:**

	Provide valuable content that educates and engages this group. For example, tutorials, product guides, or
	even lifestyle content that aligns with their interests can build a deeper connection  
		    
- **Win-Back Campaigns:**

	Reach out to customers who haven't made a purchase in a while with a special "We Miss You" offer.
	Highlight what's new and improved since their last purchase.  

- **Targeted Promotions:**

	Offer personalized discounts or promotions tailored to their past purchases or browsing behaviour. For 	example,
	if they tend to buy lower-priced items, offer discounts on higher-margin products they haven't tried yet.

---
## After Modelling:
The following aggregates were ascertain: Number of loyal customers stood at **133** which is **66.5%** of the customer base with a customer retention score of **5.64** and profitability score of **0.88**. This figures indicate the company marketing and promotion strategy is yielding result, but there is also need for continuous improvement.  
 
**Number of Non-Loyal customer** was **67** which is **33.5%** of the customer base: This figure is a huge cause for alarm. Why? Because the rule of thumb is an efficient customer base should have loyalty % that is three times the non-loyalty customer ratio i.e. **3:1**. For this case, it is obviously not so. This figures is an excellent indicator of a poor performing marketing/promotion strategies, it connotes some of the marketing strategy were administered to the wrong customer group or the unit lacks ample financial commitment to capture more major marketing strategies for various customer group thereby making difficult to explore more marketing strategies.

---
## Recommendation:
Continue to improve and innovate on the marketing strategies of the loyal customer group, while aggressively administering sales promotion like Buy 1 get one free, opening a lottery win grand price based 
on continues patronage, and rewards exclusively for loyal customer groups.
The buy 1 get one free will encourage sales and the lottery win will further strength and crystalize the sales, while the exclusive rewards for loyal customers will buy considerable level of loyalty 
that may boost loyalty percentage.  

---
Please Find attached [`Customer set report`](customer_matrix.ipynb) 













