# Monte Carlo Simulation for Supply Chain Management

This repository demonstrates my approach to solving a supply chain management problem using Monte Carlo simulation in Python. The simulation models the impact of demand variability, transportation delays, and supply disruptions on inventory levels, allowing for effective supply chain optimisation and risk mitigation.

## Problem Statement and Objective
**Company A** is experiencing significant uncertainties due to fluctuating product demand, transportation delays, and supply disruptions. The objective is to use probability models to simulate inventory levels over a 252-day business period and determine optimal inventory levels to meet daily demands for the next year.

The key challenge is to balance inventory to avoid surplus, which leads to increased storage costs, or deficits, resulting in lost sales and decreased revenue. The Monte Carlo simulation helps to forecast these risks and guide the company's supply chain strategy.

## Statistical Techniques and Libraries
The simulation uses the following statistical techniques and Python libraries:

- **Statistical Techniques**:
  - Monte Carlo simulation to model the randomness in supply chain operations.
  - Histogram analysis for visualising the frequency of stockouts.
  
- **Python Libraries**:
  - `numpy` for random number generation and mathematical operations.
  - `pandas` for data manipulation and analysis.
  - `matplotlib.pyplot` for data visualisation and plotting.

## Key Variables and Assumptions
To build the Monte Carlo simulation, I defined key variables and assumptions:

- **Key Variables**:
  - Quantity in Stock
  - Reorder Level
  - Unit Price
  - Shipping Lead Time (days)
  - Demand Forecast (Next Month)

- **Assumptions**:
  - Data is assumed to be normally distributed.
  - A business year consists of 252 working days.
  - Demand forecasts increase by 1% monthly, with a 5% variance.
  - Unit prices increase by 2% monthly, with a 5% variance.
  - Lead time has a standard deviation of 1 day.
  - A reorder buffer of 1.5 is used for safety stock.

## Simulation and Results
The Monte Carlo simulation runs over a 252-business-day period, with 200 iterations to assess inventory levels, demand, unit price changes, and shipping lead time. Reorders are placed when inventory drops below the reorder level, with lead time uncertainty accounted for in the simulation.

The results from 200 simulations are:

- **Stockout Frequency**:
  - The simulation calculates the average stockout frequency for each product. Most products have close to zero stockouts, indicating effective inventory control or overstocking. However, some outliers with higher stockouts suggest specific issues.
- **Total Order Cost**:
  - The simulation calculates the total order cost for each product over the period.

## Suggested Implementations
Based on the simulation results, I identified recommendations for improving supply chain management:

- **Low-Stockout Products**:
  - Consider reducing safety stock levels to free up capital without significantly increasing stockout risk.
  
- **High-Stockout Products**:
  - Investigate the reasons behind frequent stockouts, including demand forecasting, supplier performance, or reorder levels.
  
- **Cost Reduction**:
  - Review procurement and logistics strategies to reduce the total order cost, especially for high-cost products.
  
- **Overall Strategy**:
  - Consider segmenting products based on their stockout profile and adjusting inventory strategies accordingly.

## Summary
The Monte Carlo simulation proved valuable for modelling supply chain variability and identifying areas for improvement. This repository demonstrates my ability to create and analyse complex simulations, providing actionable insights for supply chain optimisation.

Feel free to explore the code and simulation results to understand my approach. If you have any questions or would like to discuss job opportunities, please contact me.
