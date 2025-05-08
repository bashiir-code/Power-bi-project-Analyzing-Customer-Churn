# Power-bi-project-Analyzing-Customer-Churn
Telecom Customer Churn Analysis – Databel


Project Overview
----------------

This Case Study of Power BI is about analyzing the customer churn of a subscription-based telecom company, Databel. Customer churn is a major concern for subscription-based businesses, so understanding churn effectively becomes the main tool for customer retention and profit incrementation.

This project is a detailed customer survey of Databel in which we will reveal the identification and visualization of key metrics of customer churn that give the information about patterns and factors that make the churn. The researchers take a step further than only calculating the churn rate and give reasons, and possible consequences of the customer leaving the firm, ending with recommendations of how to mitigate churn.


Data Checking & Validation
----

Before getting into the heart of the problem, I assure myself that the set of data is perfect, complete, and handy for extracting significant ideas. 

This involves:
---

 Data Quality Assessment:
 ----
   ![Image](https://github.com/user-attachments/assets/43a548c0-562c-4894-ab84-4aa1592bcca3)
   
   After loading the dataset, I couldn't help but notice that the headers were in the very first row, so I rearranged them to be column names. After that, I double-checked the data structure to make sure that all columns were properly formatted with the correct data types. Not a single inconsistency was found, and the duplicate check, lastly, revealed that there were no duplicated records. When the dataset is both cleaned and structured, the next appropriate step of action is checking for missing values and conducting a preliminary statistical summary to pinpoint any peculiarities before proceeding with the deeper analysis. 


 Data Structure Review: 
 ----
   ![Image](https://github.com/user-attachments/assets/879c4918-74c8-4d05-bc80-412d01268a37)
   
  Numerous values were put in text form for storage and needed to be changed to numbers (whole, decimal, money) where needed. The data had a structure of being in one big table with no relationship checks needed. 
  If I will need to have a date table in the future, I will do it later.

 Preliminary Exploration:
 ---
   ![Image](https://github.com/user-attachments/assets/d73aa4b1-017c-4368-95b0-03c158eccff1).
    
   To establish the data, I developed two measures: the Count of ID to see the sum of all the 
   records and the Distinct Count of ID to ensure that there 
   are no missing or repeated values. With these measures, I was able to verify the dataset's 
   reliability and extent of completion. 
   
          DAX statement
          Number of Customers = COUNT('Databel - Data'[CustomerID]
          Number of Unique Customers = DISTINCTCOUNT('Databel - Data'[CustomerID]
     
   ![Image](https://github.com/user-attachments/assets/8c9551e3-be65-449c-b548-4dbcf27bc10c)
   
         DAX statement 
         Chunr Rate = [Number of Churned Customers] / [Number of Customers]
      
    
   After I did an in-depth examination of the churn by departments, I noticed a frightening 
   tendency: the churn rate stood at a good 27%. This statistic evoked some thoughts that 
   justify the need for further inspection to decrypt the factors behind such a high rate. The 
   exclusive reach to the data  is the basis for identifying patterns in holding on to the 
   customer or discovering the weak  areas that make clients move away.

   Since we have a Churn Reason column, we can look at the specific reasons customers are 
   churning. By aggregating and graphing this information, we can view the most common churn 
   drivers and focus on decreasing their impact. The next step is to examine the distribution 
   of churn reasons to determine areas of emphasis.

   ![Image](https://github.com/user-attachments/assets/8bddbff3-583b-40cd-aaa3-209cd936ee26)

  The analysis determines on firt hand that customer service and competitors are the biggest 
  drivers of churn. Both of these categories need further investigation into why customers are 
  going to competitors and what specifically they are experiencing with customer service. 
  Identifying trends within these reasons for churn will enable actionable initiatives to be 
  developed to improve retention.

  To find how the competitors and customer service would impact churn, we need to analyze 
  their percent of total cases of churn. By calculating their share, we can determine their 
  significance compared to other causes for churn. It will help identify what needs priority 
  fixing in relation to the problems affecting customer retention.

  I saw the Churn Category column had blank values, and this would affect the accuracy of the 
  analysis. Since there was already an "Other" category, I replaced the missing values with 
 "Other" to prevent inconsistency and obtain a more accurate estimation of churn distribution. 
  This modification prevents missing data and categorizes all churn cases appropriately.

  ![Image](https://github.com/user-attachments/assets/69b7e4e9-b87b-44d6-a056-b5ea2f9dc462)

  I used the Churn Category column to see the distribution of the churned customers by 
  quantity. By calculating the grand total, I was able to see how churn is distributed across 
  categories and determine the most critical causes for customer loss. This segmentation 
  provides a clear idea of where most attention must be given to avoid minimizing churn.

  ![Image](https://github.com/user-attachments/assets/fda08381-96f9-483c-a896-70b801cbbc51)
  The churn analysis revealed that 45% of the customers churned out due to competitors, and 
  this was the largest driver of churn. The second and third most common reasons were attitude 
  and dissatisfaction, both due to customer service issues. The "Other" category had a 
  frequency of 12%, and price was the least common reason for churn at 11%. This reveals that 
  the focus should be on improving customer service as well as competitor influence analysis, 
  rather than optimizing prices.


   Second, I will investigate where the highest churn rates are taking place. Knowing where customer attrition is having the largest effect, we can determine what the next action should be. Whether that is 
  improving service in those areas, modifying marketing efforts, or taking on primary causes of churn in those areas.

  ![Image](https://github.com/user-attachments/assets/0ac5f4cf-87ab-4489-858c-672ca8b27d8c)

  
  The analysis shows that the State of CA is the most affected, with a 63% churn rate. This highlights a critical issue in this region, requiring further investigation into the underlying causes. Understanding 
  the specific factors driving churn in CA will help in developing targeted strategies to improve customer retention.

  # Notes:
  
 From the initial part of the investigation, it's clear that our competitiveness is weak—something seems off, and we’re not performing well compared to others in the market.
 
 The overall churn rate is 27%, which is already quite high.

 California stands out with an abnormal churn rate of 63%, and currently, we don’t know the cause behind this.
 
 Additionally, 45% of the churn is due to competitors, which suggests that customers are leaving us for alternative services, possibly because of better offers or dissatisfaction on our side.


  
**Analyze Demographics**

# Age Groups Affect on Churn Rate
Let’s take a closer look at how different age groups are affecting the churn rate, this might help us understand the problem better and spot if certain age ranges are more likely to leave than others.

![Image](https://github.com/user-attachments/assets/87cb6411-cf9d-445c-ba1e-91730404840a)

We can see that the churn rate among seniors is close to 40%, meaning nearly half of our senior customers are leaving. That’s quite concerning and suggests we’re struggling to attract or retain older customers.

This result suggests that we should break down the age groups further to see which ones are most affected by churn, and which groups we’re still managing to attract and retain well.

![Image](https://github.com/user-attachments/assets/711c646a-69e7-4f4f-adfc-c667aa265158)

Age 45 is our largest customer group, with a churn rate of about 25%. There’s a clear trend: churn average increases with age, confirming our assumption that we’re struggling to retain older customers.

# Databel offers group contracts to customer from the household. That could have impact on the churn rate.

![Image](https://github.com/user-attachments/assets/2d8894d4-cf54-4fd7-a3fd-a4fdb12664f1)

We see that non-group customers have a higher churn rate, while customers in groups of 6 have the lowest churn. Interestingly, the average monthly bill doesn’t drop significantly as group size increases, so lower churn isn’t just about lower cost.

# Contract type and gender effect on churn rate 

![Image](https://github.com/user-attachments/assets/04c9df57-27b9-4070-a02a-1efeccccaf71)

From the visualization, we can see that monthly contracts have a significantly higher churn rate. Gender doesn't appear to have much impact, especially within contract types, the churn rates for males and females are very close.

# How unlimited data plan and GB consumption effects on churn rate

![Image](https://github.com/user-attachments/assets/2ca19e2b-5915-41fd-92b4-884c19823994)

Customers with unlimited data plans show a higher churn rate, and the highest churn within that group comes from those who use less than 5 GB per month.

# How international calls effect on churn rate in CA

![Image](https://github.com/user-attachments/assets/300fc00d-a8e0-4369-b7a1-d76bedbbdf7d)

72% of customers without an international plan still make international calls, which presents a great opportunity to launch a targeted promotion or introduce a lightweight international package for this segment.

Additionally, Databell should identify customers who have an international plan but rarely use it, and suggest downgrading their plan. This could improve customer satisfaction and reduce unnecessary churn.


**Investigating Issues with Customer Service**

![Image](https://github.com/user-attachments/assets/0c0b2021-f2a2-424e-b509-66c6fae746ad)
We can 








  

  

  


 
  

  
  

   

// TODO:
--
 
