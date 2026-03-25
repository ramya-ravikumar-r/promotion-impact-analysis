# Promotion Impact Analysis on E-Commerce Sales

Regression analysis on 128,975 Amazon sales records to answer a critical business question: Do promotions actually drive revenue? Spoiler: the data says no — and the numbers prove it.


# Problem Statement
The XYZ E-commerce marketing team wanted to know whether their promotional campaigns were generating meaningful revenue lift across clothing and accessories categories. This project uses end-to-end EDA and regression modeling to quantify the relationship between promotions and sales — and delivers a counter-intuitive but data-backed finding.
Business Question: Do promotions positively and significantly impact revenue?

# Dataset
PropertyDetailSourceAmazon India Sales DatasetRecords128,975 transactionsCategoriesClothing & AccessoriesKey ColumnsOrder ID, Category, Amount, Promotion Applied, State, Fulfillment Status

# Approach
Raw Data → EDA → Feature Engineering → Regression Modeling → Business Insight
Exploratory Data Analysis — Key Findings
InsightDetailTop CategoryWomen's Fashion (Dresses, Tops, Sarees, Kurtis)Top States by VolumeMaharashtra, Karnataka, Tamil NaduOrders Fulfilled75,000+ successfully shippedPromotion DistributionMajority of orders had some promotion applied
Models Built & Compared
ModelR² ScoreRMSEInterpretationLinear Regression0.057HighPromotions explain only 5.7% of revenue varianceRidge Regression0.061HighMarginal improvementLasso Regression0.054HighSimilarRandom Forest0.82MediumHigh variance — overfitting riskDecision Tree0.9990.045Near-perfect fit — overfitting flag 

# Key Finding

Promotions alone do not drive revenue lift.
Linear models (the most generalizable) show R² = 0.057 — meaning promotions explain less than 6% of the variation in revenue. Category type, region, and order volume are far stronger drivers.

The Decision Tree's R² = 0.999 looks impressive but is a textbook overfitting case — it memorizes the training data rather than learning generalizable patterns. This distinction is the core strategic insight delivered to the marketing team.

# Tech Stack
Python Pandas NumPy Scikit-learn Matplotlib Seaborn Jupyter Notebook

# Business Recommendations Delivered

- Don't increase promotion spend expecting proportional revenue gains — the correlation is weak
- Focus on high-performing categories (Women's Fashion) and top states for targeted campaigns
- Investigate non-promotional drivers — product availability, pricing, and seasonality likely matter more
