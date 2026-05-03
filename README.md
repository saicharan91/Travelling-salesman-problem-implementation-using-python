# Travelling Salesman Problem (TSP) Implementation in Python

## 📌 Project Overview

This project demonstrates the implementation of the **Travelling Salesman Problem (TSP)** using Python. The goal of TSP is to determine the shortest possible route that visits each city exactly once and returns to the starting city.

In this project, we solve TSP for five cities:

* Ludhiana
* Jalandhar
* Amritsar
* Chandigarh
* Patiala

Two approaches are implemented:

* Brute Force Method
* Permutation-Based Optimization

---

## 🧠 Problem Description

A salesman must travel through all given cities exactly once and return to the starting city while minimizing the total distance traveled.

The distance matrix used:

| City       | Ludhiana | Jalandhar | Amritsar | Chandigarh | Patiala |
| ---------- | -------- | --------- | -------- | ---------- | ------- |
| Ludhiana   | 0        | 61        | 140      | 106        | 93      |
| Jalandhar  | 61       | 0         | 80       | 149        | 154     |
| Amritsar   | 140      | 80        | 0        | 229        | 235     |
| Chandigarh | 106      | 149       | 229      | 0          | 75      |
| Patiala    | 93       | 154       | 235      | 75         | 0       |

---

## ⚙️ Features

* Calculates the shortest path using brute force
* Uses permutation logic for path optimization
* Generates random cities for testing
* Visualizes TSP routes using matplotlib
* Modular and reusable code structure

---

## 📂 Project Structure

```
├── tsp.py              # Core TSP implementation using permutations
├── brute_force.py      # Brute force approach using itertools
├── util.py             # Utility functions (City class, distance, visualization)
├── test_data/          # Generated or stored city datasets
└── README.md           # Project documentation
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repo-link>
cd tsp-project
```

### 2. Install dependencies

```bash
pip install matplotlib
```

### 3. Run TSP using predefined graph

```bash
python tsp.py
```

### 4. Run brute force visualization

```bash
python brute_force.py
```

---

## 📊 Output

* Displays the minimum travel cost in the console
* Shows a graphical representation of the optimal route

---

## 🧮 Algorithm Used

### 1. Brute Force Approach

* Generates all possible permutations of cities
* Computes total distance for each route
* Selects the minimum cost path

**Time Complexity:** O(n!)

---

### 2. Permutation-Based TSP

* Iteratively computes next lexicographical permutation
* Tracks minimum path cost

---

## 📷 Visualization

The project uses `matplotlib` to visualize:

* Cities as points
* Travel path as connected lines

---

## ⚠️ Limitations

* Not suitable for large datasets due to factorial time complexity
* Performance decreases rapidly as number of cities increases

---

## 🔮 Future Improvements

* Implement dynamic programming (Held-Karp algorithm)
* Add Genetic Algorithm approach
* Optimize using heuristics (Nearest Neighbor, Simulated Annealing)

---

## 👨‍💻 Author

Vuribindi Sai Charan Reddy

---

## 📜 License

This project is open-source and available under the MIT License.

