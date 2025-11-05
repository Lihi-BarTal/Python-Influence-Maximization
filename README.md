# 🕸️ Influence Maximization on Social Networks (Hill Climbing)

**Python Project - Implementation for E-Commerce Models**

## 💡 Overview
This project solves the **Influence Maximization** problem on a large social network graph (IC Model), focusing on selecting a subset of influential users (seed set) to maximize the spread of influence within a fixed budget constraint.

## 🎯 Core Strategy: Hill Climbing with Optimizations

The solution is based on the **Hill Climbing** greedy algorithm, modified with several custom optimizations to improve efficiency and results:

1.  **Hater Filtering:** Nodes identified as "haters" are initially removed from the selection pool to prevent negative influence spread.
2.  **Marginal Gain / Cost Ratio:** The algorithm uses a greedy approach, selecting the node with the highest **Marginal Gain per Unit Cost** (the ratio of new influence gained to the node's cost).
3.  **Advanced Filtering (Tested):** The solution explored advanced node filtering based on centrality metrics (Degree, Closeness, Betweenness, etc.) to refine the available seed set, aiming to further maximize expected influence.
4.  **Influence Estimation:** The expected influence spread is estimated over thousands of simulations to ensure accuracy.

## 📄 Project Files

| File Name | Description |
| :--- | :--- |
| **`Influence Maximization Model.py`** | **The main implementation.** Contains the modified `hill_climbing_with_budget` algorithm and custom filtering logic. |
| **`Influence Maximization Model.pdf`** | **Full Methodology Report.** Detailed analysis of the approach, justification for the greedy selection criteria, and results of testing various centrality-based filtering methods. |
| **`Praducci_simulation.py`** | External file used to run and simulate the influence spread. |
| **Data Files** | **`NoseBook_friendships.csv`**, **`costs.csv`**, **`haters.csv`** | Input files defining the network structure, node costs, and users with negative influence. |
