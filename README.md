# 🏡 Airbnb Market Analysis

![Image Alt](https://github.com/wilhmhkm/Airbnb_Market_Analysis_Tableau/blob/94a20a328664a332a02d5877c8c52deac1cbe086/Project%20Dashboard.jpg)

<p align="center">
  <a href="https://public.tableau.com/views/Video5-AirBnBFullProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link">View Interactive Dashboard Here</a>
</p>

## 📌 Executive Summary
In this project, I built an end-to-end data analytics workflow in Tableau using an Airbnb dataset from Seattle. My goal was to identify the most profitable locations and property types for launching an Airbnb rental business.

I take raw, unstructured data and turn it into actionable insights that directly answer business questions. Through the dashboard, I break down where to invest by highlighting high-performing zip codes, how to price using average daily rates, when to rent by analyzing seasonality trends, what to buy by evaluating the optimal bedroom count, and how competitive the market is through listing distribution.

The final output is an interactive dashboard designed not just for visualization, but for real decision-making, while also demonstrating how I approach business problems analytically from end to end.

---

## 🛠️ Tools & Technologies
- **Tableau Public** – Data visualization and dashboard development  
- **Microsoft Excel** – Data preprocessing and consolidation  
- **Kaggle Dataset (Seattle Airbnb Open Data)** – Data source  
- **Data Modeling Techniques** – Joins, filtering, aggregation  

---

## 🚀 Data Processing Steps

I start by importing the Airbnb dataset, which includes listings for property details, calendar data for pricing and availability, and reviews for customer feedback. I then consolidate multiple CSV files into a single Excel file to create a unified working dataset.

Next, I identify the key fields that matter for analysis. This includes location data such as zip code and coordinates, financial metrics like price and fees, and property attributes such as bedrooms and bathrooms. I also remove irrelevant columns to keep the dataset focused and efficient.

I join the datasets using Listings.id with Calendar.listing_id and Reviews.listing_id. After validating the joins to ensure accuracy, I remove unused tables like Reviews to improve performance and keep the model clean.

I filter the dataset to focus on 2016 data only to maintain consistency. I remove null values and invalid entries such as listings with zero bedrooms. I also reduce the dataset size so it performs efficiently within Tableau.

I convert numerical fields like bedrooms into categorical dimensions to make analysis more intuitive. I also create calculated metrics such as average price and distinct listing count to support deeper insights.

I build five key visualizations to answer core business questions. These include average price by zip code, a geographical price distribution map, revenue trends over time, average price by bedroom count, and listing count by bedroom count.

Finally, I bring everything together into a single interactive dashboard. I enable filtering for better user control and structure the layout to guide the viewer through a clear, logical story.

---

## 📊 Key Insights

From the analysis, I find that certain zip codes such as 98134 consistently show higher average prices, and these high-value areas tend to cluster geographically, indicating strong location-based demand.

I observe clear seasonality trends, with peak revenue occurring during the summer months and year-end holidays. In contrast, demand drops noticeably in the early months of the year, particularly January and February.

Larger properties with five to six bedrooms command significantly higher prices. However, smaller units dominate the market supply, even though they generate lower revenue per listing.

Competition is highest in the one-bedroom segment, where listings are heavily concentrated. In contrast, four to six bedroom properties face much lower competition.

There is a clear trade-off in the market. Smaller units offer higher volume but lower pricing, while larger homes have lower volume but deliver stronger profitability per listing.

---

## 💡 Recommendations

I focus on zip codes with consistently high average prices and strong demand signals, as these areas offer better returns.

I prioritize four to six bedroom homes, where pricing power is stronger and competition is lower, creating a more favorable investment position.

I align listing strategies with peak demand periods, particularly during the summer and year-end holidays, to maximize revenue potential.

I reduce exposure to highly competitive segments such as one-bedroom listings, where differentiation and pricing power are limited.

To deepen the analysis further, I would incorporate additional factors such as customer reviews and ratings, occupancy rates, and more advanced pricing strategies like weekly and monthly optimization.
