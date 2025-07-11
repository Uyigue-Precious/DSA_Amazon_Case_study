# DSA_Amazon_Case_study

## Table Of Content
- [Project Overview](#Project-Overview)
- [Data Source](#Data-Source)
- [Dataset Overview](#Dataset-Overview)
- [Tools](#Tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#Data-Analysis)
- [Result/Findings](#Result/Findings)
- [Recommendation](#Recommendation)
- [ Limitations](#Limitations)

### Project Overview
This project showcases my data analysis skills using a real world e-commerce dataset scraped from Amazon product listings. As a Junior Data Analyst at RetailTech Insights, I explored product details and customer engagement data to extract valuable insights that inform product strategy, marketing decisions, and customer satisfaction.

### Dashboard
<img width="626" alt="AmazonCaseStudy" src="https://github.com/user-attachments/assets/e121dbef-ed3a-49a1-a73d-31817a8bbc81" />

### Data Source
Amazon Data: The primary dataset is "Amazon case Study.xlsx"

### Dataset Overview
Source: Amazon scraped product pages
xdfcf5v3
Records: 10,000+ rows

Fields: Product Name, Category, Price, Discount, Ratings, Review Count, Review Titles/Content

### Tools
- Power Qury - Data Cleaning
- Excel - Dashboard

### Data Cleaning/Preparation
In the initial data preparation phase, I performed the following tasks:
1. Data loading and inspection.
2. Handlingg Missing Values.
3. Data Cleaning and formating

### Exploratory Data  Analysis
EDA involved exploring the data to answer key question, such as:

1.	What is the average discount percentage by product category? 
2.	How many products are listed under each category? 
3.	What is the total number of reviews per category?  
4.	Which products have the highest average ratings? 
5.	What is the average actual price vs the discounted price by category? 
6.	Which products have the highest number of reviews? 
7.	How many products have a discount of 50% or more? 
8.	What is the distribution of product ratings (e.g., how many products are rated 3.0, 
4.0, etc.)? 
9.	What is the total potential revenue (actual_price × rating_count) by category? 
10.	What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)? 
11.	How does the rating relate to the level of discount? 
12.	How many products have fewer than 1,000 reviews? 
13.	Which categories have products with the highest discounts? 
14.	Identify the top 5 products in terms of rating and number of reviews combined

### Data Analysis
```Excel
- Price_Tiers
=IFS([@[discounted_price]]< 200,"budget_price",[@[discounted_price]] <= 500,"silver_pricie",[@[discounted_price]]> 500,"premium_pricing")

- Rating_Score
=[@rating]*[@[rating_count]]

- Potential_revenue
=[@[discounted_price]]*[@[rating_count]]
```

### Result/Findings
The Analysis result are summarized as follows:
1. HomeImprovement, Computer$Accessories, and Health&PersonalCare categories had the highest average discounts.
2. Categories like Electronics and Computer&Accessories and Home$kitchen had the most products respectively.
3. Electronics had the highest review volume.
4. Most rated Product were SurgeProtector, StreamingClient, CordManagement and Airfryer with 4.5 rating.
5. Electronics had the highest price difference.
6. USBCables has the heighest reviewed with 223 reviews.
7. 53 products had discounts of 50% or more.
8. Most products had ratings between 3–5.
9. Electronics led with the highest estimated revenue of about 59179753425.
10. Most products fall under the premium_pricing in the >₦500 tier.
11. There is a slight positive trend between discount and product rating, highly discounted products tend to receive higher ratings.
12. 326 products had under 1,000 reviews.
13. HomeImprovement and computer&accessories offered the biggest average discounts.
14. Products like "USB Cable", "SmartPhone", "SmartWatches", SmartTelevision" and Cables scored highest in quality + popularity.

### Recommendation
1. Focus Marketing on Electronics and High-Performing Products
- Since Electronics has the highest review volume, most products, and the highest estimated revenue, it should be prioritized for marketing campaigns, inventory expansion, and promotional strategies.

- Promote top-performing products like SmartPhones, SmartWatches, SmartTelevisions, and USB Cables to maximize visibility and sales.

2. Leverage Discount Strategy to Boost Ratings and Sales
- There's a positive trend between discounts and product ratings, meaning higher discounts may improve customer perception.
- HomeImprovement and Computer & Accessories had the highest average discounts —these categories can be used to pilot aggressive pricing campaigns.

3. Expand Product Range in High-Traffic Categories
- Categories such as Electronics, Computer & Accessories, and Home & Kitchen host the most products and engagement.
- Continue diversifying product listings in these categories to meet demand and maintain competitive advantage.

4. Highlight and Upsell Highly Rated Products
- Products like SurgeProtectors, StreamingClients, Airfryers, and CordManagement devices had the highest ratings (4.5).
- Position these as "Best Rated" or "Customer Favorites" to drive conversions and trust.

5. Optimize Pricing for Premium Segments
- A majority of products fall under the >₦500 premium pricing tier. Ensure pricing aligns with customer value perception by bundling, offering loyalty discounts, or emphasizing quality in marketing.

6. Improve Visibility for Underrated Products
- 326 products had fewer than 1,000 reviews which may affect trust and sales.
- Use incentives like early reviews, referral rewards, or sampling programs to boost engagement on these products.

7. Monitor and Scale What Works
- Track performance of high-discount + high-rating products to find your "sweet spot" for discounting without sacrificing profit.
- Reinvest in scaling top products that combine popularity (high reviews) and quality (high ratings).

### Limitations
I had to remove columns not neccessary for my analysis such as About_Product, user_id, User_name,, Review_content, Review_title, Img_link and product_link. 




  
