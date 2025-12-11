# **Financial Transactions Analysis Project** – Hackathon 1
## TEAM D: Alona, Igor and Teresa

## **Financial Transaction** ##

![Screenshot](/images/project%20logo.png)

### **Business Requirement: Scenario Based**
A newly appointed Marketing Manager needs to understand the bank’s customer profile to design effective marketing communications. The project was split into 2 parts namely to understand:
- who the customers are
- the financial health of the bank 

This dataset was chosen to support that goal by enabling customer segmentation and insight generation.

### **Data Source**

https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets/data 

### **Project Plan**

A Trello board was created to support Project Planning.

**https://trello.com/b/qbunO8Nm/financial-transactions-analysis**

### **Datasets Content** 

This Financial Transactions Analysis Project contains 3 datasets: Customer Demographic (users_data.csv), Card data (cards_data.csv) and Transaction Information (financial_analysis.csv).  

The features of the datasets are described below: 

**user_data.csv**
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
    
 **cards_data.csv:**
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
 
 **financial_analysis.csv:**
 - **year_month** - Textual - The period of the transaction
 - **card_id** - Numerical - A unique identifier for the bank card used (integer)
 - **amount** - Numerical - The financial amount of the transaction (floating-point number)

### **Analysis techniques used**

Data clenaing, feature engineering and data preprocessing was performed to prepare the data file for the analysis. 

Analysis was performed using Python and both analysis and visualisation was performed in Tableau (**financial-transactions-analysis.twbx**.)  

## **Presentation**

<img width="1043" height="571" alt="image" src="https://github.com/user-attachments/assets/d582c22e-4cbb-475a-8aff-6dd1bceea915" />

<img width="1061" height="609" alt="image" src="https://github.com/user-attachments/assets/ae18bf3c-97c7-4342-b3f1-7f1608b1f56e" />

<img width="1207" height="650" alt="image" src="https://github.com/user-attachments/assets/513dab4d-6ef5-4d5f-9d9d-54b5665f71cc" />

<img width="1163" height="726" alt="image" src="https://github.com/user-attachments/assets/c7dda821-e33d-4e94-aef3-a572843aedf6" />

<img width="1166" height="492" alt="image" src="https://github.com/user-attachments/assets/a65aa1f6-ee09-49b2-8554-25e5518dacc1" />

<img width="991" height="504" alt="image" src="https://github.com/user-attachments/assets/66926b7b-0359-4c0f-92ec-3190e728c1e0" />

## **Tableau**

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

![Screenshot1](/images/Dashboard.jpg)


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
