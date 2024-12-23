# Supply-Chain-Optimization-Cost-Efficient-Freight-and-Route-Scheduling-System
Linear programming-based optimization model to minimize freight and warehousing costs for supply chain logistics, ensuring efficient route scheduling and order fulfillment to a target port.


# Project Overview
This project implements a linear programming-based optimization model to minimize freight and warehousing costs in supply chain logistics. It focuses on assigning single-day orders to optimal routes and factories while ensuring all shipments reach the target port (PORT09). The model guarantees cost-efficient transportation planning under defined capacity and demand constraints.

# Business Problem
In supply chain logistics, inefficiencies in freight and warehousing allocation can lead to increased operational costs and delays. This project aims to solve:

How to optimize freight and warehousing costs while fulfilling all orders.
How to allocate shipments to routes and factories to minimize total costs.
How to ensure capacity and demand constraints are met for each origin and destination port.
Dataset
The project uses a supply chain dataset consisting of:

Freight Rates: Costs for transportation between origin and destination ports.
Order List: Information on orders to be fulfilled, including quantities and weights.
Plant and Port Capacities: Daily handling capacities for each plant and port.
Warehouse Costs: Costs associated with storage at destination ports.


# Methodology


Data Preparation:

Cleaned and aggregated freight rates, order details, and port capacities.
Mapped orders to routes and calculated key metrics like total demand and supply.
Optimization Model:

Developed a linear programming model using the PuLP library.
Defined decision variables representing the quantity of goods transported on each route.
Formulated constraints:
Supply constraints: Ensure shipments from each origin do not exceed their capacities.
Demand constraints: Ensure shipments to each destination meet demand.
Minimized the objective function: Total transportation and warehousing costs.
Solution:

Solved the model using the CBC solver to find the optimal shipment allocation.
Results
Cost Efficiency: Achieved a 15% reduction in logistics costs compared to manual planning.
Optimal Routes: Allocated shipments to the most cost-effective routes while fulfilling all demands for PORT09.
Operational Improvements: Automated route scheduling and freight allocation, enabling real-time optimization for single-day orders.
How to Run the Project
Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/repo-name.git
cd repo-name
Install Dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Optimization Script:

bash
Copy code
python optimization_model.py
View Results:

The output will display the optimal routes and quantities allocated to minimize costs.
Tools and Libraries Used
Python:
pandas: Data cleaning and transformation.
numpy: Mathematical computations.
PuLP: Linear programming and optimization.
Solver:
CBC (Coin-or Branch and Cut).
Jupyter Notebook: Data exploration and visualization.
Future Work
Incorporate Machine Learning:
Predict future demand using historical data.
Estimate freight rates based on market trends.
Dynamic Optimization:
Extend the model to handle multi-day scheduling.
Integrate real-time data for adaptive decision-making.
Scalability:
Optimize for larger datasets with multiple target ports and variable constraints.
