# Airbnb-Analysis
Data analysis of the New Zealand Airbnb market using Pandas, Seaborn and Matplotlib. Investigates 50k+ listings to reveal pricing premiums in Queenstown-Lakes, supply dominance in Auckland, and the financial impact of room types.
# Airbnb Data Analysis: Pricing, Spatial Trends, and Host Dynamics

## 📊 Project Overview
This repository contains a comprehensive data analysis of an Airbnb dataset consisting of over **50,000+ rental listings** across various regional districts. The primary objective of this project is to uncover actionable insights into short-term rental market trends, local pricing optimization, spatial density, and host characteristics. 

By utilizing data cleaning, exploratory data analysis (EDA), and data visualization techniques, this project provides data-driven strategies for travelers looking for value and property hosts aiming to maximize revenue.

---

## 🛠️ Tools & Technologies Used
* **Language:** Python
* **Libraries:** 
  * **Pandas & NumPy** – For structural data manipulation, addressing extensive missing values, and engineering baseline aggregates.
  * **Matplotlib & Seaborn** – For statistical data visualization, plotting distributions, and geographic-based category counting.
* **Environment:** Jupyter Notebook / Visual Studio Code

---

## 🧼 Data Preprocessing & Cleaning Workflow
The raw dataset contained `50,932` records and `18` features with substantial null values. The following pipeline was developed to prepare the data for analysis:
* **Missing Value Imputation (Numerical):** Handled missing data in key business indicators like `price`, `reviews_per_month`, `calculated_host_listings_count`, and `host_id` by substituting them with their respective dataset `mean` values.
* **Missing Value Imputation (Categorical):** Replaced null fields within structural descriptive strings (`name`, `host_name`, `neighbourhood_group`, `neighbourhood`, and `room_type`) with an `'Unknown'` placeholder. 
* **Null Boundary Handling:** Imputed empty `last_review` timestamps with a string flag `'No Review Date'`.
* **Feature Filtering:** Dropped or bypassed completely vacant, non-value adding features like `license` to optimize DataFrame shape.

---

## 🚀 Key Insights & Findings

### 💰 Regional Pricing Strategies
* **Premium Regions:** The **Queenstown-Lakes District** commands the highest real estate premium on short-term rentals, maintaining the highest average price profile (**~$620.14** per night) and an aggressive median price point of **$457.00**.
* **Budget Regions:** Local regions like **Kawerau District** offer the cheapest alternatives with average nightly prices settling near **$159.50**.

### 📍 Local Ward Outliers (Top 10 Most Expensive vs. Cheapest)
* **High-Demand Micro-Markets:** On a localized ward level, **Galatea-Murupara Ward** and **Queenstown-Wakatipu Ward** lead as the most expensive destinations, pushing average listing prices beyond **$674.00** per night.
* **The Sweet Spot Value:** Property listings located in **Burwood Ward** represented the highest savings marker, posting the cheapest entry rates with an average baseline of **$109.43** per night.

### 🏠 Room Type Variations & Distributions
* **The Entire Home Advantage:** Listings configured as an **"Entire home/apt"** dominate market volume with **41,757 listings** and capture premium margins at an average cost of **~$378.01** per night.
* **Shared Accommodations:** Private rooms offer mid-tier affordability at **~$163.23** per night, while **Shared rooms** fall to the bottom of the financial threshold at an average of just **$76.74** per night.

### 🗺️ Spatial Density & Supply Hubs
* **The Metros Lead:** Geographic clustering analysis shows that **Auckland** holds the highest density of short-term rental supply, encompassing **9,463 active listings**—accounting for **18.6%** of the entire regional market share.

---
