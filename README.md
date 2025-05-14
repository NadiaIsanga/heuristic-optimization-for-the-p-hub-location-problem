# heuristic-optimization-for-the-p-hub-location-problem
# Heuristic Optimization of the Single Allocation p-Hub Location Problem (SApHLP)

This project implements and compares two powerful metaheuristic algorithms — **Simulated Annealing (SA)** and **Tabu Search (TS)** — to solve the SApHLP, a logistics network design challenge. The goal is to minimize total network cost by optimally placing hubs and allocating nodes through a single hub.



##  Summary

Solved the SApHLP for datasets with 10 to 100 nodes using Simulated Annealing and Tabu Search.  
Explored the effect of hub count and discount factors on cost using CAB, TR, and RGP datasets.  
Found that **lower discount factors (α = 0.3)** and **fewer hubs** consistently reduced Total Network Cost (TNC).  
Tabu Search performed better on smaller problems; Simulated Annealing offered more stable exploration.



##  Skills Used

- **Python (NumPy, Pandas, Matplotlib)**
- **Heuristic Optimization**
- **Simulated Annealing**
- **Tabu Search**
- **Logistics Network Modeling**
- **Performance Evaluation (TNC, Iteration Analysis)**
- **Parameter Tuning (Cooling schedules, hub count, α)**



##  Key Experiments

- **Datasets**: CAB10, CAB20, TR40, RGP100  
- **Hub Counts (p)**: 3, 5, 7, 10  
- **Discount Factors (α)**: 0.3, 0.7  
- **Cooling Schedules (SA)**: Geometric, Linear, Exponential  
- **Performance Metric**: Total Network Cost (TNC)


##  How to Run

1. Clone the repo  
   `git clone https://github.com/NadiaIsanga/heuristic-p-hub-optimization.git`

2. Open the notebook  
   `cd heuristic-p-hub-optimization/code`  
   `jupyter notebook hub_location_optimization.ipynb`

3. Run configurations for different datasets, hub counts, and discount factors



## Results Overview

- **Best Configurations**: CAB10 with p=3 and α=0.3 yielded lowest costs.
- **SA vs TS**:  
  - SA performed consistently across all problems, especially with geometric cooling.  
  - TS showed efficiency on smaller networks but needed tuning for large-scale problems (RGP100).  
- **Scalability**: Both algorithms face challenges on large networks; hybrid models are recommended.


![image](https://github.com/user-attachments/assets/e1bfc516-f8db-415b-a1e6-615140b9db7d)






