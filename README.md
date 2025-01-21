 # **Credit Card Analysis**

## **Table of Contents**

- [Problem Statement](#problem-statement)
- [Datasource](#data-source)
- [Data Preparation](#data-preparation)
- [Data Analysis (DAX)](#data-analysis-dax)
- [Data Visualization Dashboard](#data-visualization-dashboard)
- [Insights](#insights)



## **Problem Statement**
Mitron Bank, a legacy financial institution headquartered in Hyderabad, seeks to launch a new line of credit cards to expand its product offerings and market presence. To evaluate the feasibility and potential success of this initiative, the bank has partnered with AtliQ Data Services for a pilot project.

AtliQ Data Services has been tasked with analyzing a sample dataset of 4,000 customers from five cities, containing details on their online spending and other demographic and behavioral attributes. The goal is to uncover actionable insights and trends that can help Mitron Bank tailor its credit card offerings to meet customer needs and align with market trends.

The analysis should deliver data-driven recommendations that address the following objectives:

    Identify customer segments with the highest potential for credit card adoption.
    Understand spending patterns and preferences to design targeted rewards and benefits.
    Evaluate regional differences and city-specific trends to optimize marketing strategies.
    Highlight any gaps or opportunities in the current market that the new credit card can address.

The success of this pilot project and the acquisition of the full project depends on AtliQ Data Services' ability to deliver a compelling and insightful analysis that demonstrates a clear value proposition to Mitron Bank's strategy director and his team.
    

## **Data source**
**File Name:** `dim_customers.csv`
                `Fact_Spend.csv`
- **Description:** Dataset provided by Mitron Bank for pilot analysis of 4,000 customers across five cities.
**Datasets** 
-     Fact_spend: Details about spending behavior, including customer ID, spending month, payment type, spending, and spending category.
    Dim_customer: Customer details, such as customer ID, gender, city, age group, average income (for a period of 6 months), marital status, and occupation.
- **Columns:**
  - `Customer_ID`: Unique identifier for each customer.
  - `Age_group`: Age group of the customer.
  - `Gender`: Gender of the customer (`Male`, `Female`).
  - `City`: Customer's city of residence.
  - `Income_Level`: Income category (`Low`, `Medium`, `High`).
  - 'Avg_income_utilization% : average percentage of income utilized by the customer.
  - `Total_Spend`: Total spend across all categories.
  - `Current_Credit_Card`: Whether the customer owns a credit card (`Yes`, `No`).
  - `Credit_Score`: Customer's credit score.
  - `Spending_Category`: Major category of spend (`Travel`, `Shopping`, `Dining`, etc.).
  - `marital status`: Marital status of the customer (Single, Married).
  - `occupation`: Profession or occupation of the customer.
  - `Total_Spend`: Total amount spent by the customer.
  - `Month`: Total spends in Month wise
  - `Payment_type`: The payment method used (e.g., Credit Card, Debit Card, UPI, etc.).
  - `category`: The spending category (e.g., Travel, Dining, Groceries, etc.).
    
## **Data cleaning & data transformation**
- Checked for null and duplicate values
- Categorized average income into three categories: low, middle, and high (conditional column).
- Created a custom column, payment category, to classify payment types into card and digital.
- Calculated average spending
## **Data Model**

![image](https://github.com/user-attachments/assets/a5b21d1d-bf67-42f2-80cd-5aeee7bfa6a9)


## **Data Analysis (DAX)**
 - avg income utilization % = AVERAGE('dim_customers'[Avg_income_utilization%])

## **Data Visualization (Dashboard)**
## Dashboard:



## **Insights**


