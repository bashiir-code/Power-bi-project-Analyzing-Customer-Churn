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
    
   To establish the data, I developed two measures: the Count of ID to see the sum of all the records and the Distinct Count of ID to ensure that there 
   are no missing or repeated values. With these measures, I was able to verify the dataset's reliability and extent of completion. 

   ![Image](https://github.com/user-attachments/assets/1ef18a20-18a9-4031-ae7f-d1b0384c8429).
    
   After I did an in-depth examination of the churn by departments, I noticed a frightening tendency: the churn rate stood at a good old 27%. This statistic evoked some thoughts that justify the need for further 
   inspection to decrypt the factors behind such a high rate. The exclusive reach to the data is the basis for identifying patterns in holding on to the customer or discovering the weak areas that make clients 
   move away.
   

 
