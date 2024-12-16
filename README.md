# Price-Optimization

### Overview

Price optimization involves analyzing historical data to determine the most effective pricing strategies for maximizing a company’s profitability. This project focuses on identifying the optimal price points for products using advanced data analysis techniques and machine learning models. Various factors such as competitor pricing, product features, freight costs, and customer behavior have been incorporated to provide actionable insights.

### Motivation

Efficient pricing strategies are critical for a company’s success, as they directly impact profitability, customer satisfaction, and market competitiveness. By leveraging historical data and predictive modeling, this project aims to:

- Maximize revenue and profit.
- Understand the influence of key variables on product demand and pricing.
- Explore advanced techniques like utility optimization and fuzzy logic for dynamic pricing.
- Evaluate the role of price elasticity and competitor pricing.

### Key Features

Feature Importance Analysis: Understand the variables influencing product demand and pricing using machine learning feature importance metrics.

- Price Elasticity Modeling: Analyze the impact of price changes on demand and revenue.
- Revenue and Profit Optimization: Identify price points that maximize revenue and profit using simulations.
- Dynamic Pricing with Fuzzy Logic: Adjust pricing dynamically based on demand thresholds and competitor data.
- Customer Segmentation: Cluster customers based on purchase behavior for targeted pricing strategies.

### Dataset

The dataset includes:

- Pricing Data: Historical pricing of products.
- Competitor Data: Prices of competing products.
- Freight Costs: Associated delivery costs.
- Customer Behavior: Purchase quantities and patterns.

The dataset used in this project is stored in Retail Price Optimization.zip, which includes retail_price.csv. It contains features like:

- unit_price: Historical price of the product.
- freight_price: Delivery costs.
- comp_1, comp_2, comp_3: Competitor prices.
- qty: Quantity sold.

### Methodology

##### Data Cleaning and Preprocessing:
- Ensured that features like unit_price and freight_price were properly formatted as single-column Series.
- Handled missing or invalid values by replacing them with appropriate statistics like the mean.

##### Feature Engineering:
- Scaled numeric features using MinMaxScaler.
- Created interaction features with PolynomialFeatures for advanced analysis.

##### Modeling:
- Built a Random Forest model to predict product demand.
- Evaluated the model using Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² Score.

##### Price Optimization:
- Simulated revenue for a range of prices to identify the optimal price point.
- Incorporated profit analysis by factoring in freight costs.

##### Advanced Techniques:
- Applied fuzzy logic to dynamically adjust pricing based on demand thresholds.
- Performed utility optimization to maximize the difference between price and cost.

##### Competitor Analysis and Segmentation:
- Analyzed the correlation between competitor prices and demand.
- Clustered customers based on behavior for refined pricing strategies.

### Results

- Revenue Maximization: Identified the optimal price point of $1.00, which yielded maximum revenue of $1994.73.
- Profit Optimization: Calculated profit-maximizing price points by incorporating freight costs.
- Price Elasticity: Analyzed the responsiveness of demand to price changes and identified elastic and inelastic price ranges.
- Dynamic Pricing: Implemented fuzzy logic to adjust prices in response to high or low demand.
- Customer Segmentation: Used KMeans clustering to segment customers and understand distinct purchase behaviors.

### Visualizations

- Feature importance bar plots to highlight the most influential factors.
- Elasticity curves to demonstrate demand responsiveness.
- Revenue and profit curves to visualize optimal price points.
- Scatter plots showing original vs adjusted prices with fuzzy logic.
- Heatmaps displaying correlations between variables like competitor pricing and demand.

### Source

https://www.kaggle.com/datasets/suddharshan/retail-price-optimization/data
