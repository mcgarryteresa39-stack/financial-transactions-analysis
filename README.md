# **Financial Transactions Analysis Project** – Hackathon 1
## TEAM D: Alona, Igor and Teresa
![Screenshot](/images/project%20logo.png)
### **Datasets Content** 

This Financial Transactions Analysis Project contains 3 datasets: Customer Demographic (users_data.csv), Card data (cards_data.csv) and Transaction Information (financial_analysis.csv).  

Card Information dataset includes: 
 1. Credit and debit card details 
 2. Includes card limits, types, and activation dates 
 3. Links to customer accounts via card_id 
 4. Essential for understanding customer financial profiles 

User Data dataset includes: 
 1. Demographic information about customers 
 2. Account-related details 
 3. Enables customer segmentation and personalized analysis 

Transaction Data:
1. Detailed transaction records including amounts, timestamps, and merchant details
2. Covers transactions throughout the 2010s
3. Features transaction types, amounts, and merchant information
4. Perfect for analyzing spending patterns and building fraud detection models

The features of the datasets are described below: 
**user_data.csv**
 - **id** -  Numerical - The unique ID of the customer
 - **current_age**  -  Numerical  -  The current age of the individual in years (integer) 
 - **retirement_age**   -  Numerical  -   The projected retirement age in years (integer) 
 - **birth_year**  -  Numerical  -  The calendar year of birth (integer) 
 - **birth_month**  -  Numerical  -  The month of birth (as a number (1 through 12)) 
 - **gender**  -  Categorical  -  Textual data/string indicating the individual's gender 
 - **address**  -  String  -  Textual data/string containing the address 
 - **latitude**  -  Numerical   
 - **longitude**  -  Numerical    
 - **per_capita_income**  -  String (converted to numerical)  -  Average income per person as a text/string, contains a currency symbol 
 - **yearly_income**  -  String (converted to numerical) - The customer's annual income as a text/string, contains a currency symbol 
 - **total_debt**  -  String (converted to numerical) -  Debt data stored as a text/string, contains a currency symbol 
 - **credit_score**  -  Numerical  -  A whole number score representing creditworthiness 
 - **num_credit_cards**  -  Numerical  -  A count of the number of credit cards the individual possesses (integer)
    
 **Cards_data.csv:**
 - **id"** -  Numerical - The unique ID of the customer
 - **client_id**  -  Numerical  -  A unique numerical identifier assigned to a customer (integer) 
 - **card_brand**  -  Categorical  -  The name of the card issuer brand, as text/string 
 - **card_type**  -  Categorical  -  The type of card ("Debit", "Credit", "Prepaid"), as text/string 
 - **card_number**  -  Numerical  -  The primary 16-digit card number.   
 - **expires**  -  String  -  The card's expiration date, as text/string 
 - **cvv**  -  Numerical  -  The Card Verification Value (CVC/CVV2) security code  
 - **has_chip**  -  Categorical  -  A categorical indicator ("Yes", "No")   
 - **num_cards_issued**  -  Numerical  -  Numerical number of cards issued to the client 
 - **credit_limit**  -  Textual  -  The maximum amount of credit granted to the cardholder, as a text/string, contains a currency symbol 
 - **acct_open_date**  -  String/Date  -  The date the account was originally opened 
 - **year_pin_last_changed**  -  Numerical/ Date  -  The year the cardholder last updated their Personal Identification Number (PIN) 
 - **card_on_dark_web**   -  Categorical  -  A categorical/boolean indicator ("Yes", "No") resulting from a security scan 
 
 **financial_analysis.csv**
 - **year_month** - Textual - The period of the transaction
 - **card_id** - Numerical - A unique identifier for the bank card used (integer)
 - **amount** - Numerical - The financial amount of the transaction (floating-point number)

### **Data download source**

https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets/data 

### **Business Requirement: Scenario Based**
A newly appointed Marketing Manager needs to understand the bank’s customer profile to design effective marketing communications. The project was split into 2 parts namely to understand:
- who the customers are
- the financial health of the bank 

This dataset was chosen to support that goal by enabling customer segmentation and insight generation.

### **Project Plan**

A Trello board was created to support Project Planning.
https://trello.com/b/qbunO8Nm/financial-transactions-analysis

### **Analysis techniques used**

Data clenaing, feature engineering and data preprocessing was performed to prepare the data file for the analysis. 

[you can see Tableau file](/tableu/financial-transactions-analysis.twbx)

Analysis was performed using Python and both analysis and visualisation was performed in Tableau (**financial-transactions-analysis.twbx**.)  

![Screenshot1](/images/Tableau.png)

In Tableau was also presented two line charts, with a common X-axis representing current age (from 18 to over 101 years old), illustrate how the number of credit cards and the amount of total debt affect the number of credit cards and the amount of total debt, namely display a data visualization comparing average credit card usage and total debt levels across different age groups. 

![Screenshot1](/images/Age_Card_Debt_Spend.png)

The trends of median of Num Credit Cards, median of Total_Debt and sum of Amount for Current Age.  Colour shows details about Gender. The data is filtered on Card Brand, Card Type and Amount. The Card Brand filter keeps Amex, Discover, Mastercard and Visa. The Card Type filter keeps Credit, Debit and Debit (Prepaid). The Amount filter keeps all values. The view is filtered on Current Age, which ranges from 18 to 101 and keeps Null values.


![Screenshot1](/images/Card%20Type.png)

Count of Card Type broken down by Card Brand vs. Card Type.  Colour shows details about Card Brand.  The marks are labelled by count of Card Type. The data is filtered on Gender, which keeps Female and Male.

![Screenshot1](/images/Gender%20Card%20Preference.png)

Sum of Num Credit Cards for each Gender.  Colour shows details about Gender. The data is filtered on Card Type and Card Brand. The Card Type filter keeps Credit, Debit and Debit (Prepaid). The Card Brand filter keeps Amex, Discover, Mastercard and Visa.

![Screenshot1](/images/Transaction%20by%20Cards.png)


Sum of Amount for each Card Brand broken down by Card Type.  Colour shows details about Card Brand.  The marks are labelled by count of Card Type and sum of Amount. The data is filtered on Gender and Amount. The Gender filter keeps Female and Male. The Amount filter ranges from -638,25 to 21885,76.

![Screenshot1](/images/Yearly%20Spend%20on%20all%20bank's%20cards.png)

The line chart illustrating the "Yearly Spend on all bank's cards" from the year 2010 to 2018. The line chart summarizes the total annual spending across all bank cards, revealing clear trends: initial growth (2010-2013) showed steady, consistent growth over three years, rising to around 60 million by 2013; period of stability (2013-2017) total costs significantly stabilized at a peak level around 60 million and a sharp decline (2017-2018).

![Screenshot1](/images/Descriptive%20Statistics.png)

The view is broken down by Statistic Type (Parameters), Age Stat., Retirement Age Stat., Total Debt Stat., Yearly Income Stat., PCI Stat., Credit Score Stat., Cards Num Stat. and Credit Limit Stat. The data is filtered on Gender, Card Brand and Card Type. The Gender filter keeps Female and Male. The Card Brand filter keeps Amex, Discover, Mastercard and Visa. The Card Type filter keeps Credit, Debit and Debit (Prepaid).

![Screenshot1](/images/Credit%20Score%20Histogram%20of%20Spending.png)

The stacked bar chart visualization "Credit Score Histogram of Spending" analyzes cost amounts across different credit score ranges. The visualization summarizes the behavior of customers grouped by credit rating quality. The largest amount of spending falls on the Good credit rating range, indicate that customers in the “Good” credit rating range have stable income, debt, and credit card usage patterns, showing high overall spending relative to their limits.

![Screenshot1](/images/30%20Top%20Spenders.png)

The bar chart "30 Top Spenders" ranks clients by their total spending amount and summarizes which clients spend the most and provides demographic insights into those individuals

![Screenshot1](/images/New%20Clients%20by%20Year%20and%20their%20Spending.png)

Two linked line charts, sharing a common X-axis representing the "New Clients by Year and their Spending" from 1994 to beyond 2019, track both the volume of new accounts opened and the associated spending for these clients, categorized by gender (blue and orange lines), summarizing customer acquisition and spending trends over a 25-year period.

![Screenshot1](/images/Banded%20Client%20Ages%20vs%20Financial%20Profile.png)

The bar chart "Banded Client Ages vs Financial Profile," analyzes and  summarizes a strong positive correlation between client age and the total spend by card, the average financial metrics (Credit Score, Cards held, Debt, and Income) are remarkably consistent between the 31-40 and 51-60 age groups. Both groups maintain a "Good" credit score around 710 and average debt and income levels.

We also have created an amazing interactive GEO map in Tableau, where you can find complete information about each customer. Examples of research can be found below

![Screenshot1](/images/Customers%20GEO%20map.png)
![Screenshot1](/images/Customers%20GEO%20map2.png)

Map based on Longitude and Latitude. Colour shows details about Gender. Size shows sum of Num Credit Cards.  Details are shown for various dimensions.
It summarises the geographic and demographic profile of the bank's customer base. A key observation is that the bank has a high concentration of customers in densely populated areas of the United States, particularly in the eastern states, where spending is high among both men (orange) and women (blue). The map effectively highlights the places where the bank's services are used the most, allowing for analysis of regional spending habits and customer demographics.

In summary, we create a very informative data visualization dashboard "Bank's Story" that organizes various analytical representations of a banking dataset. You can see visible tabs with different reports or analytics. The navigation structure summarises a comprehensive data analysis workflows focused on the bank's customers.

![Screenshot1](/images/banks%20story.png)

There you will find the 'The dashboard to check the bank's results'  toolbar to verify the bank's results below

![Screenshot1](/images/Screenshot.png)


And a single, unified file **clients_card_data.csv** was created. 

 
Then we moved on to the process of extracting, transforming, and loading the data, also using Python in a Jupyter Notebook (including checked data types to ensure that numeric columns were numbers). 

After cleaning and data preparation, we can describe that our dataset contains information about 

```
 count    2000.000000 
 mean       45.391500 
 std        18.414092 
 min        18.000000 
 25%        30.000000 
 50%        44.000000 
 75%        58.000000 
 max       101.000000 
```

We have determined that our dataset contains the following demographic indicators by age where: 

```
 age_group
 ≤30      520 
 31–40    345 
 41-50    380 
 51–60    325 
 60+      430 
```


```
age_group
≤30      47971.0
31–40    46834.0
41-50    44962.0
51–60    48914.0
60+      40341.0
```
![Screenshot1](/images/Mean%20Yerly%20Income%20by%20Age.png)

The bar chart illustrates the relationship between age and average annual income. The data indicates that our customers achieve high income between the ages of 51 and 60. After age 60, income levels decline. Income levels in the 30-60 age group remain mostly in the range of $45,000 to $49,000, indicating overall stability.


The EDA steps were performed by using the Python modules pandas, matplotlib, seaborn and plotly. 

Histograms visualized that the most common income level is around 20,000, most customers earn less than 40,000, also we have customers with high income levels – up to 160,000 and above, which illustrates significant income inequality;

![Screenshot2](/images/Distribution%20of%20Per%20Capita%20Income.png)

 visualized the classification by gender and age. Using a scatterplot, we indicated the relationship between income and age to examine the growth rate of income by age. The scatterplot visualizes data that suggests that there is a wide range of income across all age groups, with no discernible strong linear correlation.

![Screenshot2](/images/Gender%20Distribution.png)
![Screenshot2](/images/Distribution%20of%20Current%20Age.png)
![Screenshot3](/images/Distribution%20of%20Income%20by%20Age.png)

 We have also illustrated the level of debt on graphs for further analysis. 
 We analyzed and visualized the distribution of credit scores with histogram, which showed that most customers have good or excellent credit scores (above 650), while a smaller number of people have very low scores (below 550). The scores are heavily concentrated in the mid-700 range. The Distribution of Number of Credit Cards histogram showed that it is common among customers to have 1 to 4 credit cards, while having 5 or more cards is rarer. 

![Screenshot](/images/Distribution%20of%20Total%20Debt.png)
![Screenshot](/images/Distribution%20of%20Credit%20Scores.png)
![Screenshot](/images/Distribution%20of%20Number%20of%20Credit%20Cards.png)

The dataset contains mostly numeric data with the relevant types listed below. The income distribution (per capita income and annual income) is highly skewed by a few high-income individuals.

```
per_capita_income    int64
yearly_income        int64
total_debt           int64
dtype: object
   per_capita_income  yearly_income  total_debt
0              29278          59696      127613
1              37891          77254      191349
2              22681          33483         196
3             163145         249925      202328
4              53797         109687      183855
       per_capita_income  yearly_income     total_debt
count        2000.000000    2000.000000    2000.000000
mean        23141.928000   45715.882000   63709.694000
std         11324.137358   22992.615456   52254.453421
min             0.000000       1.000000       0.000000
25%         16824.500000   32818.500000   23986.750000
50%         20581.000000   40744.500000   58251.000000
75%         26286.000000   52698.500000   89070.500000
max        163145.000000  307018.000000  516263.000000
```

as we can see below
```
                            OLS Regression Results                            
==============================================================================
Dep. Variable:             total_debt   R-squared:                       0.347
Model:                            OLS   Adj. R-squared:                  0.346
Method:                 Least Squares   F-statistic:                     353.0
Date:                Mon, 08 Dec 2025   Prob (F-statistic):          7.09e-184
Time:                        12:09:41   Log-Likelihood:                -24140.
No. Observations:                2000   AIC:                         4.829e+04
Df Residuals:                    1996   BIC:                         4.831e+04
Df Model:                           3                                         
Covariance Type:            nonrobust                                         
====================================================================================
                       coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------------
const             5.869e+04   1.02e+04      5.745      0.000    3.87e+04    7.87e+04
num_credit_cards -5924.8101    594.809     -9.961      0.000   -7091.321   -4758.299
yearly_income        1.2376      0.041     30.081      0.000       1.157       1.318
credit_score       -46.9941     14.480     -3.245      0.001     -75.392     -18.596
==============================================================================
Omnibus:                      166.521   Durbin-Watson:                   2.013
Prob(Omnibus):                  0.000   Jarque-Bera (JB):              970.130
Skew:                           0.079   Prob(JB):                    2.18e-211
Kurtosis:                       6.408   Cond. No.                     5.53e+05
==============================================================================

Notes:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.
[2] The condition number is large, 5.53e+05. This might indicate that there are
strong multicollinearity or other numerical problems.
```

This analysis shows that approximately 34.7% of the variability in a customer's total debt can be explained by the number of credit cards, annual income, and credit score. All three predictor variables have a statistically significant relationship with total debt. The results show that higher income is associated with higher levels of debt, while more credit cards and higher credit scores are associated with lower levels of debt.

![Screenshot](/images/Total%20Debt%20vs%20var.png)

Scatter plots illustrate the relationship between total customer debt and three potential factors: number of credit cards, yearly income, and credit score. Yearly income has the strongest correlation, showing that higher income is generally associated with higher levels of debt.
Credit scores show that higher scores are associated with lower levels of debt.

![Screenshot](/images/Mean%20Total%20Debt%20by%20Credit%20Score%20Group.png)

The bar chart Mean Total Debt by Credit Score displays the average total debt across five credit rating categories. Highest debt levels has the group "Fair" with the highest average total debt, $78,340. Lowest debt levels has  the "Exceptional" group with total debt at $58,448. The "Good", "Very_Good", and "Exceptional" groups have a relatively consistent debt level, in the range around the $58,000 to $60,000.

![Screenshot](/images/PCA%20Clusters.png)

The visualizations compare K-Means clustering results with k=3 and k=4 after applying PCA. The k=3 uses diagonal decision boundaries, the k=4 provides a more accurate segregation of data points, which appear more clearly separated into four groups. 

The plot uses the Elbow Method to determine the optimal number of clusters for a K-Means
```
Silhouette Score for 3 clusters: 0.093
Silhouette Score for 4 clusters: 0.088
```
This shows that 3 is the optimal number of clusters for this dataset.

![Screenshot](/images/Elbow%20Method.png)


### **Summary of Findings**

Key observations on card brand share: 
The dominant brand is Mastercard at 52.2%. The second largest brand is Visa at 37.8%. Together, Mastercard and Visa account for exactly 90% of the total card share displayed. The smaller brands are Amex at around 6.5% and Discover at just 3.4%. 

```
            Count  Proportion  Proportion (%)
card_brand                                   
Mastercard   3209    0.522128           52.21
Visa         2326    0.378458           37.85
Amex          402    0.065408            6.54
Discover      209    0.034006            3.40
```

Overall distribution: Market share is highly concentrated between the two leading brands, while all others have a negligible share. 

![Screenshot](/images/summary.png)

![Screenshot](/images/customer%20Overview.png)

![Screenshot](/images/Executive%20summary.png)

![Screenshot](/images/table.png)

This analysis will facilitate the development of targeted marketing communications by providing important information about customer profiles.

In the future, the data analysis we provide will enable us to improve operational efficiency and increase the bank's revenues. The information obtained as a result of customer segmentation is crucial for optimising marketing activities, which directly leads to improved operational efficiency and increased revenues for the bank.

### **Ethical considerations**

In accordance with GDPR, no personally identifiable information (PII) was included in the analyses. All data used in this project is public and available for use. 

### **Unfixed bugs**

After conducting a set of tests, we haven't found any bugs. Initial problems have been fixed. 


### **Main Data Analysis libraries**

**Core Languages:** Python 
**Data Processing (ETL):** Pandas, NumPy, kagglehub 
**Visualisation:** Matplotlib, Seaborn,  Scipy, Scikit Learn, Tableau 
**Version Control:** Git & GitHub 

### **Credits**

The Code Institute course materials for the course “Data Analysis with Artificial Intelligence” were used as a template for the code in this project. 
The code for feature development was adapted from (https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets/data) 

All files were created and uploaded to GitHub 
