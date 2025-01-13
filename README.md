# Price-Optimization

### Overview

This project showcases how fuzzy logic and advanced machine learning techniques revolutionize price optimization. By analyzing historical sales data and key factors like competitor pricing, product features, freight costs, and customer behavior, the project identifies the optimal price points that maximize revenue and profitability.

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

### Problem Statement

Pricing is a pivotal aspect of business strategy, directly impacting profitability and competitiveness. However, static pricing models often fail to adapt to fluctuating market conditions, such as demand shifts, competitor actions, and seasonal changes.

This project aims to solve the following challenges:

- Dynamically adjusting prices based on demand patterns.
- Mitigating risks of overpricing or underpricing.
- Incorporating external factors like competitor pricing to refine strategies.

With fuzzy logic, businesses can mimic human decision-making, enabling a nuanced, adaptive approach to pricing that balances revenue growth with customer satisfaction.

### Solution Approach

Step 1: Data Preparation
- Addressed missing values using mean imputation for numerical features.
- Removed outliers in pricing and demand using interquartile ranges.
- Normalized features to ensure comparability across variables.

Step 2: Exploratory Data Analysis (EDA)

Key Insights:
- Competitor pricing heavily influenced demand, with a strong inverse correlation.
- Seasonal demand spikes presented opportunities for targeted price adjustments.

Visualizations:
- Scatter plots to visualize price-demand relationships.
- Heatmaps to identify feature correlations.

Step 3: Implementing Fuzzy Logic
- Define Demand Levels:
  - Categorized sales data into three demand levels:
      - Low Demand: Below 25th percentile.
      - Moderate Demand: 25th–75th percentile.
      - High Demand: Above 75th percentile.

- Create Fuzzy Rules:
      - High Demand → Increase Price by 10%.
      - Moderate Demand → Maintain Price.
      - Low Demand → Decrease Price by 10%.

- Dynamic Pricing Adjustments:
      - Calculated revenue across various price points using machine learning models.
      - Applied fuzzy logic to identify optimal prices dynamically.

Step 4: Model Building
- Predictive Models:
      - Random Forest Regressor to predict revenue under different pricing scenarios.
      - Fuzzy logic-based pricing adjustments implemented using Python's skfuzzy library.
- Evaluation Metrics:
      - RMSE and R² scores to evaluate model accuracy in predicting revenue.

Step 5: Testing and Evaluation
- Simulated three pricing scenarios:
      - Low Demand: Price reduction increased sales but marginally improved revenue.
      - Moderate Demand: Price stability maintained consistent revenue and customer trust.
      - High Demand: Price increase resulted in a 15% revenue boost during peak seasons.

### Key Findings

1. Revenue Optimization:
- Dynamic pricing strategies outperformed static models in all demand scenarios.

2. High Demand Capitalization:
- 15% revenue growth achieved by increasing prices during high-demand periods.

3. Inventory Management:
- Price reductions for low-demand products cleared inventory effectively, minimizing holding costs.

### Visualizations

- Revenue vs. Price Adjustments: A line chart illustrating how revenue changes with price adjustments, highlighting the efficacy of fuzzy logic.
- Demand Thresholds: A histogram showing categorized demand levels and corresponding price adjustments.
- Before and After Price Adjustments: A scatter plot comparing original and adjusted prices, emphasizing the impact of fuzzy logic.

### Future Directions

1. Real-Time Implementation: Test the fuzzy logic pricing model in a live environment.
2. Incorporate Additional Features: Include customer segmentation, seasonal trends, and economic indicators.
3. Expand Fuzzy Rules: Introduce granular demand levels for more nuanced adjustments.

### Source

https://www.kaggle.com/datasets/suddharshan/retail-price-optimization/data
