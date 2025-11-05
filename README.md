# 🕸️ Influence Maximization on Social Networks

**Python Project - Hill Climbing with Budget Constraint**

## 💡 Overview
This project solves the **Influence Maximization** problem under the Independent Cascade (IC) Model. The goal is to select an optimal seed set of users within a **fixed budget** to maximize influence spread across the social network.

## 🎯 Core Implementation

The solution implements a **Greedy Hill Climbing** algorithm, featuring two main optimizations:

1.  **Selection Metric:** Nodes are selected based on the highest **Marginal Gain per Unit Cost** ratio (Influence Gain / Node Cost).
2.  **Filtering:** Nodes identified as "haters" are pre-filtered to ensure a focus on positive influence spread.

## 📄 Full Methodology

**The complete technical analysis, mathematical justification, and full results are documented in the PDF report below.**

| File Name | Description |
| :--- | :--- |
| **`Influence Maximization Model.pdf`** | **FULL METHODOLOGY REPORT.** Detailed analysis of the greedy approach and filtering methods. |
| **`Influence Maximization Model.py`** | **The main implementation.** Contains the modified `hill_climbing` algorithm and filtering logic. |
| **Data Files** | **`NoseBook_friendships.csv`**, **`costs.csv`**, **`haters.csv`** | Input files defining the network structure, costs, and negative influence nodes. |
