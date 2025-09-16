# P16_Retail-Transaction-Analysis

**VERSION 1 - Market Basket Analysis**

**A. Project Overview**

- This project aims to explore associations between products and uncover buying patterns (MBA - Market Basket Analysis).

**B. Dataset Information**

_**Source**_

- Retail Transactions Dataset (from Kaggle).
- https://www.kaggle.com/datasets/prasad22/retail-transactions-dataset.
- The dataset includes 01 files - Retail_Transactions_Dataset.
- The Data uploaded have only 100 rows for each file. Please visit the below Kaggle link for full data.

_**Period**_

- From 2020 - 2024

**C. Methodology**

- Data Cleaning: handle missing values (Promotion ~33%), remove duplicates, detect outliers (IQR), and convert date types.
- Data Handling: export cleaned dataset for analysis.
- Market Basket Analysis (MBA): 
  + Reshape data to Transaction–Item format.
  + One-hot encoding for products.
  + Apply FPGrowth and generate Association Rules.
  + Filter rules by Support, Confidence, and Lift.

**D. Key Findings & Actionable Plans**

_**Key Findings**_

- After filtering by Lift > 1, several potential associations emerge:
  + Peanut Butter → Toothpaste (Support ~0.26%, Confidence ~7.3%, Lift ~1.03).
  + Canned Soup → Toothpaste (Support ~0.26%, Confidence ~7.2%, Lift ~1.02).
  + Ironing Board → Toothpaste (Support ~0.25%, Confidence ~7.1%, Lift ~1.01).
→ Although support is relatively low (<0.3%), these rules suggest non-random relationships between FMCG items and a personal care product (Toothpaste).

_**Actionable Plans**_

- Cross-sell bundles: propose small promotions or product bundles combining Toothpaste with Peanut Butter or Canned Soup.
- Placement strategy: experiment with positioning Toothpaste closer to FMCG shelves (e.g., food and daily essentials).
- Test & Learn: since support remains limited, conduct A/B testing in a controlled setting before scaling up.

**E. Appendix**

Top 10 Products by Support

![Top 10 Products by Support](https://github.com/CallmeNavin/P16_Retail-Transaction-Analysis/blob/main/Version%201%20-%20MBA/Visualization/Top%2010%20by%20Support.png)

Top 10 Products by Confidence

![Top 10 Products by Confidence](https://github.com/CallmeNavin/P16_Retail-Transaction-Analysis/blob/main/Version%201%20-%20MBA/Visualization/Top%2010%20by%20Confidence.png)

Top 10 Products by Lift

![Top 10 Products by Lift](https://github.com/CallmeNavin/P16_Retail-Transaction-Analysis/blob/main/Version%201%20-%20MBA/Visualization/Top%2010%20by%20Lift.png)

**F. Further Version**

In further version, I will used this dataset to:
- Group customers based on purchasing behavior (Customer Segmentation) - Version 2.
- Optimize pricing strategies and identify opportunities for discounts and promotions (Price Optimization) - Version 3.
- Analyze store performance and customer trends (Retail Analytics) - Version 4.

**About Me**

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights. I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact. For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
