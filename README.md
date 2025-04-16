# Custom-Four-Step-Demand-Model-From-Scratch
Manual implementation of the classic Four-Step Travel Demand Model using Python, applied to a synthetic 5-zone city. Built entirely from scratch without simulation software for hands-on understanding and practice.


# Four-Step Urban Travel Demand Model – Synthetic 5-Zone City

This project demonstrates a full implementation of the classic four-step travel demand model, using synthetic data for a five-zone city. All code was written in Python and executed in Google Colab.

## Author
Md. Muhtashim Shahrier  
March 2025

---

## Overview

The four modeling steps included are:

1. **Trip Generation**  
   Estimated productions and attractions using regression-style equations and synthetic socioeconomic data.

2. **Trip Distribution**  
   Implemented a doubly-constrained gravity model with impedance function f(c_ij) = 1 / (t_ij)^2

3. **Mode Choice**  
   Split total trips between Auto and Transit using a utility-based logit model.

4. **Traffic Assignment**  
   Performed all-or-nothing assignment for Auto trips using NetworkX with Dijkstra's shortest-path.

---

## Repository Structure

four-step-demand-model/
│
├── README.md                         # Project overview, instructions, and summary
├── Demand_Modelling.ipynb           # Main notebook with all modeling steps
│
├── images/                           # Visualizations generated from the model
│   ├── network.png                   # Synthetic network (nodes, edges, travel time)
│   └── assignment_flows.png         # All-or-nothing assignment edge flows
│
├── data/                             # Input datasets (Excel format)
│   ├── socioeconomic_data.xlsx
│   ├── travel_time_matrix.xlsx
│   ├── Cost_auto.xlsx
│   ├── Cost_transit.xlsx
│   ├── Travel_time_auto.xlsx
│   └── Travel_time_transit.xlsx


---

## Libraries Used

- `pandas`, `numpy` – Data manipulation  
- `matplotlib` – Visualization  
- `networkx` – Network modeling and path assignment

---

## Sample Output

Visualizations include:

- Zone-level O-D matrices for both Auto and Transit
- Network graph with edge labels for travel time and capacity
- All-or-nothing assigned flows visualized using edge width

---

## Notes

- All data are synthetic and meant for demonstration.
- Inspired by a term final question of the course CE 457: Urban Transportation Planning and Management at BUET.




