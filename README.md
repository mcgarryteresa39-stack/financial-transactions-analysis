# **Financial Transactions Analysis Project** – Hackathon 1
## TEAM D: Alona, Igor and Teresa

## **Financial Transaction Analysis to Understand Customer Needs** ##

![Screenshot](/images/project%20logo.png)

### **Business Requirement: Scenario Based**
A newly appointed Marketing Manager needs to understand the bank’s customer profile to design effective marketing communications. The project was split into 2 parts namely to understand:
- who the customers are
- the financial health of the bank 

This dataset was chosen to support that goal by enabling customer segmentation and insight generation.

### **Project Overview**

This repository contains a complete analytics workflow exploring user and card-level financial data. 

It includes data cleaning, aggregation, statistical testing, and visualization across Python and Tableau. 

The project focuses on identifying meaningful patterns in debt, income, and card ownership, with insights segmented by age bands and customer profiles. 

Final results are presented through reproducible Python scripts, Tableau dashboards, and a concise presentation deck. 

All datasets, analysis scripts, and visual outputs are organized for clarity and portfolio readiness.

### **GitHub File Structure**

![Team-D Github Data Structure](/images/Team-D_Github_Data_Structure.png)

### **Data Source**

https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets/data 

### **Project Plan**

A Trello board was created to support Project Planning.

**https://trello.com/b/qbunO8Nm/financial-transactions-analysis**

### **Datasets Content** 

This project contains 3 datasets: Customer Demographic (users_data.csv), Card data (cards_data.csv) and Transaction Information (transactions_data_final.csv).  

The features of the datasets are described below: 

**user_data.csv**
 - **id**  -  Numerical  -  A unique numerical identifier assigned to a customer (integer) 
  - **current_age**  -  Numerical  -  The current age of the individual in years (integer) 
 - **retirement_age**   -  Numerical  -   The projected retirement age in years (integer) 
 - **birth_year**  -  Numerical (converted to date) -  The calendar year of birth (integer) 
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
  - **id**  -  Numerical  -  A unique numerical identifier assigned to a card isssued by the bank (integer) 
 - **client_id**  -  Numerical  -  A unique numerical identifier assigned to a customer (integer) 
 - **card_brand**  -  Categorical  -  The name of the card issuer brand, as text/string 
 - **card_type**  -  Categorical  -  The type of card ("Debit", "Credit", "Prepaid"), as text/string 
 - **card_number**  -  Numerical  -  The primary 16-digit card number.   
 - **expires**  -  String  -  The card's expiration date, as text/string 
 - **cvv**  -  Numerical  -  The Card Verification Value (CVC/CVV2) security code  
 - **has_chip**  -  Categorical  -  A categorical indicator ("Yes", "No")   
 - **num_cards_issued**  -  Numerical  -  Numerical number of cards issued to the client 
 - **credit_limit**  -  String (converted to numerical)  -  The maximum amount of credit granted to the cardholder, as a text/string, contains a currency symbol 
 - **acct_open_date**  -  String/Date (converted to date)  -  The date the account was originally opened 
 - **year_pin_last_changed**  -  Numerical/ Date  -  The year the cardholder last updated their Personal Identification Number (PIN) 
 - **card_on_dark_web**   -  Categorical  -  A categorical/boolean indicator ("Yes", "No") resulting from a security scan 
 
 **transactions_data_final.csv:**
 - **year_month** - String (converted to date) - The month and the year of the transaction
 - **card_id** - Numerical - A unique identifier for the bank card used (integer)
 - **amount** - Numerical - The monthly financial amount of the transaction (floating-point number)
 - **client_id**  -  Numerical  -  A unique numerical identifier assigned to a customer (integer) 

### **Analysis techniques used**

Data cleaning, feature engineering and data preprocessing was performed to prepare the data file for the analysis. 

Analysis was performed using Python and both analysis and visualisation was performed in Tableau (**financial-transactions-analysis.twbx**.)  

## **Presentation Findings**
The presentation below sumamrises the core findings from the research, offering a comprehensive profile of the bank’s 2,000 customers — 
including their age range (18 to 101 years), gender distribution (49% male, 51% female), average income ($40,745), average credit score (712), 
and banking behaviors such as card usage and transaction volumes. 
It highlights who the bank’s key customers are, their financial health and how they manage their financial health. 

It will be used to ensure that products created by the bank are best suited to the needs of our customers.

## **Tableau Findings**

### **Strategic Insights**

- **Long-Term Loyalty Among 1990s Clients:** Analysis of client spending patterns reveals that individuals who joined the bank in the 1990s continue to use their cards actively for 10, 15, even 20+ years. This cohort demonstrates strong brand loyalty and sustained engagement, contributing significantly to long-term revenue.

- **Short-Term Engagement Among 2010s Clients:** In contrast, clients who joined during the 2010s exhibit intense card usage for only a few years before tapering off. For example, new account openings peaked in 2012–2013, but spending from these cohorts declined rapidly. This suggests that newer generations are less attached to a single provider and more likely to switch services.

### **Strategy Implications and Recommendations**

- **Service Quality & Experience:** To retain younger clients, the bank must prioritise exceptional service and seamless digital experiences.

- **Continuous Promotion**: Ongoing advertising and brand visibility are critical to attract and re-engage this more transient customer base.

- **Data-Driven Personalisation:** Tailoring offers based on age-band financial profiles (e.g., 60+ clients hold 4 cards and spend over $173M) can boost relevance and retention.

## **Presentation**

<img width="1043" height="571" alt="image" src="https://github.com/user-attachments/assets/d582c22e-4cbb-475a-8aff-6dd1bceea915" />

<img width="1061" height="609" alt="image" src="https://github.com/user-attachments/assets/ae18bf3c-97c7-4342-b3f1-7f1608b1f56e" />

<img width="1207" height="650" alt="image" src="https://github.com/user-attachments/assets/513dab4d-6ef5-4d5f-9d9d-54b5665f71cc" />

<img width="1163" height="726" alt="image" src="https://github.com/user-attachments/assets/c7dda821-e33d-4e94-aef3-a572843aedf6" />

<img width="1166" height="492" alt="image" src="https://github.com/user-attachments/assets/a65aa1f6-ee09-49b2-8554-25e5518dacc1" />

<img width="991" height="504" alt="image" src="https://github.com/user-attachments/assets/66926b7b-0359-4c0f-92ec-3190e728c1e0" />

# **Tableau Dashboard**

**This dashboard visualises how average credit card count and total debt vary across age groups, filtered by card brand and type.**

![Screenshot1](/images/Tableau.png)

**This visualisation displays trends in median credit card count, median total debt, and total spending across age groups, with color indicating gender. The data is filtered to include Amex, Discover, Mastercard, and Visa card brands; Credit, Debit, and Debit (Prepaid) card types; and all spending amounts. The age filter spans from 18 to 101 years and includes null values.**
![Screenshot1](/images/Age_Card_Debt_Spend.png)

**This chart compares the number of credit cards segmented by card brand and card type. Color indicates card brand, and labels show the count of each card type. The data is filtered to include both Females and Males.**

![Screenshot1](/images/Card%20Type.png)

**This chart compares the number of credit cards held by Female and Male users.**

![Screenshot1](/images/Gender%20Card%20Preference.png)

**This chart illustrates total transaction volume by card brand and card type, segmented by gender. Each bar shows the number of cards issued and the corresponding transaction amount, with color indicating gender. Filters include Credit, Debit, and Debit (Prepaid) card types, and Amex, Discover, Mastercard, and Visa brands.**

![Screenshot1](/images/Transaction%20by%20Cards.png)


**This line chart shows total yearly spending across all bank card brands from 2010 to 2018. Spending rose steadily from 2010 to 2013, plateaued at around 60 million through 2017, and then declined sharply in 2018.**

![Screenshot1](/images/Yearly%20Spend%20on%20all%20bank's%20cards.png)

**This analysis summarises key median financial and demographic metrics, including age (44), retirement age (66), total debt ($58,251), yearly income ($40,744.50), PCI statistic ($20,581), credit score (712), number of cards (3), and credit limit ($12,592.50).**

![Screenshot1](/images/Descriptive%20Statistics.png)

**This bar chart illustrates total spending across five credit score bands, highlighting how consumer behavior varies by creditworthiness. Each bar represents the aggregated amount spent by individuals within a specific credit score range, with detailed breakdowns including median debt, income, credit limit, and number of cards. Gender-based insights and individual credit score profiles further enrich the analysis.**

![Screenshot1](/images/Credit%20Score%20Histogram%20of%20Spending.png)

**This bar chart ranks the top 30 clients by total spending, with each bar representing an individual’s transaction volume. Color indicates gender, and annotations display each client’s age and number of cards issued, offering demographic insights into high-value customers.**

![Screenshot1](/images/30%20Top%20Spenders.png)

**This dual-line chart tracks the number of new accounts opened and the total spending by new clients over time, segmented by gender. The X-axis represents the year of account opening, while the Y-axes show account count and spending volume. The visualization reveals trends in client acquisition and financial engagement across different years.**

![Screenshot1](/images/New%20Clients%20by%20Year%20and%20their%20Spending.png)

**This bar chart presents financial profiles segmented by age bands, showing total spending alongside key metrics such as median credit score, number of cards, total debt, income, and client count. Each age group—from under 30 to over 60—reveals distinct financial behaviors and demographic patterns.**

![Screenshot1](/images/Banded%20Client%20Ages%20vs%20Financial%20Profile.png)

**This interactive geographic map displays individual clients across the United States, with each data point revealing detailed financial and demographic information such as income, credit score, age, gender, and card type. The visualization enables user-level exploration and supports deeper research into regional spending patterns and customer profiles. This amazing interactive GEO map was create in Tableau, where you can find complete information about each customer. Examples of research can be found below.** 

![Screenshot1](/images/Customers%20GEO%20map.png)
![Screenshot1](/images/Customers%20GEO%20map2.png)

**This dashboard, titled "Bank’s Story," presents a comprehensive geographic and demographic overview of the bank’s customer base across the United States. The map uses longitude and latitude to plot individual clients, with color indicating gender and size representing the total number of credit cards held. It highlights regions with high customer density—particularly in the eastern states—and reveals spending patterns among male and female clients. The dashboard includes multiple tabs that organize analytical reports, enabling detailed exploration of client behavior, financial metrics, and regional trends.**

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
