# 🚌 School Trip Bus Optimization

This project solves a **linear programming optimization problem** using Python's **PuLP** library and visualizes the feasible region and optimal solution using **matplotlib**.

## 📌 Problem Statement

A school is planning a trip for **400 students** and has access to:

- 10 large buses (50 seats each, ₹800 per bus)
- 8 small buses (40 seats each, ₹600 per bus)
- Only **9 drivers** are available

### Objective

Determine the **number of large and small buses** to minimize the **total transportation cost**, subject to:

- All students must be transported (≥ 400 seats total)
- No more than 10 large buses and 8 small buses
- No more than 9 drivers (i.e., buses used ≤ 9)

---

## ✅ Constraints

Let `x` = number of large buses  
Let `y` = number of small buses

### Constraints:

- `50x + 40y ≥ 400` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(seat requirement)
- `x + y ≤ 9` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(max drivers)
- `x ≤ 10`, `y ≤ 8` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(bus availability)
- `x, y` are non-negative integers

### Objective Function:

Minimize:  
**`Total_Cost = 800x + 600y`**

---

## 🧠 Solution Approach

We used the following tools:

- [PuLP](https://github.com/coin-or/pulp) for formulating and solving the LP problem
- [matplotlib](https://matplotlib.org/) to visualize constraints and feasible region

---

## 📊 Output

- Optimal number of large buses: **4**
- Optimal number of small buses: **5**
- Minimum cost: **₹6200**

![Graph Output](graph_output.png)

---

## 🛠 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/animesharyan07/task4.git
   cd task4

2. Install Dependencies:
   ```bash
   pip install pulp matplotlib numpy
   
4. Run the Script:
  ```bash
  python BusProblem.py
