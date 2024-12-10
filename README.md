
## **Project Name: Customer Personality Analysis (Team Project 1)**

### **Project Overview**
Customer Personality Analysis is a comprehensive examination of a company's ideal customer base. It enables businesses to gain deeper insights into their customers' preferences, behaviors, and pain points. This understanding helps tailor products and services to meet the specific needs of different customer segments, improving customer satisfaction and driving business growth.

Business Case : https://github.com/camellikna/Team_Project/blob/main/BusinessCase.md

Code :(https://github.com/camellikna/Team_Project/blob/main/src/Data_Preprocessing_Clustering.ipynb

Data : https://github.com/camellikna/Team_Project/blob/main/data/raw/marketing_campaign.csv

### **Team Members**
- Camelia Najafi
- Omar Khan
- Gang Huo
- Heidi Ghafoor
- Iryna Horodetska

### **Project Phases**
The project is divided into the following key phases:
1. **Writing the Business Case**  
   Defining the objectives, scope, and value proposition of the customer personality analysis.

2. **Loading and Exploring Data**
   Try to get data and check it and find null value
   
3.**Data Cleaning and Feature Engineering**

  3.1 Remove redundant columns and Remove the two columns with 1 unique value
  3.2 Convert the data type of Dt_Customer to DateTime
  3.3 Calculate the Tenure (Days as Customer) of each customer
      The newest customers' maximum Recency is 50 days from their last purchase date. Let's assume that NOW date (anchor_date = '2014-08-29') is 2 months (61 days) after their Dt_Customer date.
      
  3.4 Clean the invalid and Outlier Age
  3.5 Handling outliers and missing values of Income
  3.6 Segmenting Marital_Status and Education
     Remove all the leading and trailing spaces in columns names
     Segment 'Marital_Status' into two groups
     Segment 'Education' into three groups
     

4.**Feature Engineering**
  4.1 Calculate Total spendings on all the products
  4.2 Calculate Total number of purchases on all the products
  4.3 Calculate Total accepted compaign offers
  4.4 Calculate Total children living in the household
  4.5 Rename columns for clarity
       'MntWines': 'Wines','MntFruits':'Fruits','MntMeatProducts':'Meat','MntFishProducts':'Fish','MntSweetProducts':'Sweets','MntGoldProds':'Gold'

  4.6 Create a feature "Has_Child" to indicate parenthood status
        Analyze the correlations among the three spending features

5.**Exploratory Data Analysis and Data Visualization**
  5.1 Analyze the correlations among the three spending features
  
![image](https://github.com/user-attachments/assets/5c44f908-0ef5-46ea-8a67-f7e931b2555a)

TotalNumPurchases and Spending are strongly correlated. To simplify the clustering analysis, we choose only one key feature, i.e. Spending. 

  5.2 Exploring the distribution of features
  
  ![image](https://github.com/user-attachments/assets/e8044a13-fbaf-450b-ba9d-9c9d8976f77e)
  ![image](https://github.com/user-attachments/assets/e7a15d67-49af-4c39-894d-c35e6d57c7b5)



**Clusters Conclusions**
Stars (Cluster 0):

Highest income (78k), highest spending (1430) and high purchasing frequency
More than 90% has no child, less than 10% has one child
More than 60% has a partner
Mainly graduate or postgraduate
Occasionally accept promotions
Show lowest number of web visits
Span all ages
High consumers for meat, wines, fish and sweets
High Potential (Cluster 2):

Majority are medium income (63k), some are high income, few below medium income
Moderate spending (860) but highest purchasing frequency
Majority have a parnter
More than 90% has one child, small portion has two children, very few has no child
Majority are mature and adult, very few young or senior people
Mainly graduate or postgraduate
Rarely accept promotions
Need attention (Cluster 3):

Medium income (42k) and low spending (170)
Majority have two children, small portion have three children
Majority are adult and mature
Majority have a partner
Low purchasing frequency
Occasionally made some purchases with a discount
Do not accept promotions
Leaky bucket (Cluster 1):

Low income (33k) and low spending (140)
Majority have one child, some have no child
Have relatively larger portions of adult and young people
Majority have a partner
Low purchasing frequency
Do not accept promotions




### **Project Timeline**

- **2024-10-16**  
   Initial session: We reviewed multiple datasets and discussed their relevance to our project. After careful consideration, we decided that each group member would explore datasets related to retail, narrowing down our choices to five options.

- **2024-10-17**  
   Dataset selection: The team finalized the choice of the dataset and began initial data exploration.

- **2024-10-18**  
   Data surfacing: Continued to surface and analyze the selected dataset, preparing for further stages of analysis and visualization.

### **Conclusion**
Our project is aimed at delivering actionable insights by analyzing customer personality traits to help businesses in the retail sector align their products and services with customer preferences.
In this session , we talked about cleaning data



