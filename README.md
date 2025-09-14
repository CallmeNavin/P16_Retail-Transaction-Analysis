# P16_Retail-Transaction-Analysis

**VERSION 1 - Market Basket Analysis**

**A. Project Overview**

- This project aims to explore associations between products and uncover buying patterns (MBA - Market Basket Analysis)

**B. Dataset Information**

_**Source**_

- Retail Transactions Dataset (from Kaggle)
- https://www.kaggle.com/datasets/prasad22/retail-transactions-dataset
- The dataset includes 01 files - Retail_Transactions_Dataset
- The Data uploaded have only 100 rows for each file. Please visit the below Kaggle link for full data

_**Period**_

- From 2020 - 2024

**C. Methodology**

- Python (Google Colab):
  + A. Data Cleaning:
    - I. Data Checking:
      + I.1. Check Column Type --> Column "Date" is in Object dtype
      + I.2. Check %Blank/Null --> Column "Promotion": 33.4% (but these are "None")
      + I.3. Check duplicate:
        - For whole row
        - For ID: Column "Transaction_ID"
      + I.4. Check Outliers: by IQR & export for preventing numbers of outliers is too high
        - Column "Total_Cost"
        - Column "Total_Items"
    - II. Data Handling
      + II.1. Change type to datetime: Column "Date"
        - Using pd.to_datetime
      + II.2. Handle 33.4% blank of Column "Promotion"
        - Add "keep_default_na= False" when read csv for preventing Python recording "None" value is N/A
    - III. Export cleaned data for the following version. After exporting, delete the row which make action download for MBA
    - IV. MBA
      + IV.1. Change dataset to "Transaction_ID – Item" type
        - IV.1.1. Split Column "Product"
        - IV.1.2. One-hot Encoding for Column "Product"
        - IV.1.3. Apply Apriori Algorithm, Association Rules. Finnaly filter Top 10 by Support, Top 10 by Confidence, Top 10 by Lift
- Using Power BI for Dashboard visualize & find insights.

**D. Key Findings & Actionable Plans**

_**Key Findings**_

- 

_**Actionable Plans**_

- 

**E. Further Version**

In further version, I will used this dataset to:
- Group customers based on purchasing behavior (Customer Segmentation) - Version 2
- Optimize pricing strategies and identify opportunities for discounts and promotions (Price Optimization) - Version 3
- Analyze store performance and customer trends (Retail Analytics) - Version 4

**About Me**

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights. I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact. For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
