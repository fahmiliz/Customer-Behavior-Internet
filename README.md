# Customer-Behavior-Internet
# Use Case Summary
- Use case summary
- Objective Statement
. To reduce risk in tenure with the value is 0
. Get insight average of tenure with the customer **TIDAK MEMILIKI PARTNER** and **TIDAK MEMILIKI DEPENDEN**
. Get insight of MonthlyCharges from customer **MEMILIKI PARTNER** and **TIDAK MEMILIKI DEPENDENTS** with Maximum value
. Get insight sum of customer with **TIDAK MEMILIKI PARTNER** and **MEMILIKI DEPENDENTS**
. Get insight of average **TOTAL CHARGES** from **NON - SENSOR CITIZEN** Customer with **PHONE SERVICE** and **INTERNET SERVICE FIBER OPTIC**

- Challenges
. There is Zero value in Tenure
. Format Total Charges data is Object

- Methodology
. Data cleaning
. Manipulation
. Mathematics Analysis

- Business Benefit
. Help business department to create the product development based on Customer behavior
. Know the most of product, customer using for internet service
# Business Understanding
- How much the maximum Monthly Charges with the Customer **MEMILIKI PARTNER** and **TIDAK MEMILIKI DEPENDENTS**?
- How many the customer with category **TIDAK MEMILIKI PARTNER** and **MEMILIKI DEPENDENTS**
- How many the average of **TOTAL CHARGES** of Customer **NON SENIOR CITIZEN** with **PHONE SERVICE** and **INTERNET SERVICE FIBER OPTIC**?

# Data Cleaning
- There are tenure with 0 Value. We need to remove them from analysis

# Manipulation Data
- There are wrong format in TotalCharges data. We need to change the format into Float

# Mathematics Analysis
- **MEAN** to get average value
- **MAX** to get maximum value

# Exploratory Data Analysis
- How much the maximum Monthly Charges with the Customer **MEMILIKI PARTNER** and **TIDAK MEMILIKI DEPENDENTS**?
  Partner	Dependents	tenure	MonthlyCharges
0	  No      No      23.303354	    118.65
1	  No      Yes	    23.986072	    116.15
2	  Yes	    No	    42.709014	    118.60
3	  Yes	    Yes	    41.578161	    118.75
Maximum MonthlyCharges value for customers who have partners but do not have dependents is 118.60

- How many the customer with category **TIDAK MEMILIKI PARTNER** and **MEMILIKI DEPENDENTS**
Partner  Dependents
No       No            3280
         Yes            359
Yes      No            1653
         Yes           1740
Name: customerID, dtype: int64
It can be seen that there are 359 customers who do not have partners but have dependents

- How many the average of **TOTAL CHARGES** of Customer **NON SENIOR CITIZEN** with **PHONE SERVICE** and **INTERNET SERVICE FIBER OPTIC**?
SeniorCitizen  PhoneService  InternetService
0              No            DSL                1508.513021
               Yes           DSL                2344.751771
                             Fiber optic        3226.492737
                             No                  655.759775
1              No            DSL                1455.687019
               Yes           DSL                2542.344194
                             Fiber optic        3147.553430
                             No                  932.299038
Name: TotalCharges, dtype: float64
It can be seen that the average value of TOTAL CHARGES from NON-SENIOR CITIZEN customers (Senior Citizen = 0) who have PHONE SERVICE and have FIBER OPTIC INTERNET SERVICE is 3226,492

#Recommendation
- Plot data into scattered, line, boxplot or anything to improving of analysis
