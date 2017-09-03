# Predicting-Catalog-Demand-Using-Alteryx

## Business and Data Understanding
The key decision that needs to be made is whether or not to send the catalogs to the 250
customers. This decision depends on the various factors affecting the sale of products. The
dataset p1-customers.xlsx and p1-mailinglist.xlsx contains the detail about the various factors
related to the sale of products to the customers.

For Analysis Alteryx Software is used to easily prep, blend, and analyze all of their data using a repeatable workflow, 
then deploy and share analytics at scale for deeper insights. 

## Analysis, Modeling and Validation
Using Alteryx, a scatterplot was made for the dataset customers.xlsx. <br>
The target variable which is chosen is the Avg_Sale_Amount. <br>
Finding :-  Avg_Num_Products_Purchased vs Avg_Sale_Amount has a linear relationship. <br>
            Similar is the case with Customer_Segment.<br>
            

# Exploratory Data Analysis            
## Average Number of Products Purchased Vs Average Sales Amount           
![image](https://user-images.githubusercontent.com/16829371/30006619-5871b366-90ca-11e7-856d-71f817dd8c2c.png) <br>

## Customer Segment Vs Average Sales Amount    
![image](https://user-images.githubusercontent.com/16829371/30006625-99569446-90ca-11e7-87a8-2d2a1aa12f25.png) <br>

# Building Regression Model Using Alteryx

Building Multi linear regression model on this dataset using Avg_Sale_Amount as the target variable and Customer_Segment and Avg_Num_Products_Purchased as the predictor variable. <br>

# Linear Regression Report <br>

![image](https://user-images.githubusercontent.com/16829371/30006681-ca65e3ec-90cb-11e7-8abd-bd10612f98f4.png)

![image](https://user-images.githubusercontent.com/16829371/30006701-8621e0e0-90cc-11e7-85b0-0a6c1780c552.png)

# Alteryx Model <br> 

![image](https://user-images.githubusercontent.com/16829371/30006821-9143132e-90cf-11e7-94a6-7f69d1d0b0f8.png)

# Result <br>

On Scoring the Linear Regression Model on Mailing List of Customers , the total expected revenue from
the 250 customers is estimated. <br>
This is obtained by multiplying the Avg_Sale_Amount by the Score_Yes, i.e. the probability that the customers will respond to the catalog and make a purchase. <br>

Since, the average gross margin is 50% and subtracting the cost of printing catalog from this, we’ll get the net profit.<br>
i.e. (Total Expected Revenue x 0.5) – (6.5 x 250) <br>
 = (47224.871373 x 0.5) – (6.5 x 250) <br>
 = $21987.435687 <br>
 
Since, the profit exceeds the margin of $10,000, it is advisable to send the catalog to these 250 customers. <br>
By sending the catalog to the 250 customers, a profit of $21987.435687 can be expected. <br>






