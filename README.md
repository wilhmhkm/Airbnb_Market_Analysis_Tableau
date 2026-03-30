# 🏡 Airbnb Market Analysis

![Image Alt](https://github.com/wilhmhkm/Airbnb_Market_Analysis/blob/5cb27c9d99921cda640b185e6f1d2fa9e92423db/Dashboard%201.png)

## 📌 Executive Summary
This project presents an end-to-end data analytics workflow using Tableau, focused on analyzing an Airbnb dataset from Seattle. The objective is to identify the most profitable locations and property types for launching an Airbnb rental business.

The dashboard transforms raw data into actionable insights, helping answer key business questions:
- 📍 Where to invest (high-performing zip codes)
- 💰 Pricing strategy (average daily rates)
- 📅 When to rent (seasonality trends)
- 🏠 What to buy (optimal bedroom count)
- ⚔️ Market competition (listing distribution)

The final result is an interactive dashboard designed for decision-making and portfolio demonstration.

---

## 🛠️ Tools & Technologies
- **Tableau Public** – Data visualization and dashboard development  
- **Microsoft Excel** – Data preprocessing and consolidation  
- **Kaggle Dataset (Seattle Airbnb Open Data)** – Data source  
- **Data Modeling Techniques** – Joins, filtering, aggregation  

---

## 🚀 Data Processing Steps

### 1. Data Collection & Preparation
- Imported Airbnb dataset including:
  - Listings (property details)
  - Calendar (pricing & availability)
  - Reviews (customer feedback)
- Merged multiple CSV files into a single Excel file

### 2. Data Understanding
- Key fields identified:
  - Location: Zip code, latitude, longitude
  - Financials: Price, fees
  - Property attributes: Bedrooms, bathrooms
- Removed irrelevant columns

### 3. Data Modeling (Joins)
- Joined datasets using:
  - `Listings.id = Calendar.listing_id`
  - `Listings.id = Reviews.listing_id`
- Validated joins to ensure accuracy
- Removed unused tables (e.g., Reviews) to improve performance

### 4. Data Cleaning & Optimization
- Filtered dataset to **2016 only**
- Removed:
  - Null values
  - Invalid entries (e.g., 0 bedrooms)
- Reduced dataset size to fit Tableau limits

### 5. Feature Engineering
- Converted numerical fields (e.g., bedrooms) into categorical dimensions
- Created calculated metrics:
  - Average price
  - Distinct listing count

### 6. Data Visualization
Built 5 key visualizations:
1. Average Price by Zip Code (Bar Chart)
2. Price Distribution Map (Geographical View)
3. Revenue Trend Over Time (Time Series)
4. Average Price by Bedroom Count
5. Listing Count by Bedroom Count

### 7. Dashboard Creation
- Combined all visualizations into a single dashboard
- Enabled interactive filtering
- Structured layout for storytelling and clarity

---

## 📊 Key Insights

### 📍 Location Matters
- Certain zip codes (e.g., 98134) show significantly higher average prices
- High-value areas are geographically clustered

### 📅 Strong Seasonality
- Peak revenue periods:
  - Summer months
  - Year-end holidays
- Low demand observed in early-year months (Jan–Feb)

### 🏠 Bedrooms Drive Pricing
- Larger properties (5–6 bedrooms) command higher prices
- Smaller units dominate supply but yield lower revenue per listing

### ⚔️ Market Competition
- High competition:
  - 1-bedroom listings
- Low competition:
  - 4–6 bedroom listings

### 💰 Revenue vs Volume Trade-off
- Smaller units:
  - High volume, lower pricing
- Larger homes:
  - Lower volume, higher profitability

---

## 💡 Recommendations

### 1. Invest in High-Value Locations
Focus on zip codes with high average prices and strong demand.

### 2. Target Larger Properties
Invest in 4–6 bedroom homes to maximize pricing power and reduce competition.

### 3. Optimize Rental Timing
List properties during peak seasons:
- Summer
- Year-end holidays

### 4. Avoid Oversaturated Segments
Reduce focus on highly competitive 1-bedroom listings.

### 5. Expand Future Analysis
Enhance insights by including:
- Customer reviews and ratings
- Occupancy rates
- Pricing strategies (weekly/monthly)
