# Dynamic Multidimensional Knapsack Knapsack Optimization Problem
|![image](https://github.com/user-attachments/assets/18bd87d1-7a03-4d58-ab35-4181f409f766)|
|--|
|Example of a one-dimensional (constraint) knapsack problem: which books should be chosen to maximize the amount of money while still keeping the overall weight under or equal to 15 kg? A multiple-constrained problem could consider both the weight and volume of the books. (Solution: if any number of each book is available, then three yellow books and three grey books; if only the shown books are available, then all except for the green book.) [^1]|

[^1]: The image and its description are from [Knapsack problem](https://en.wikipedia.org/wiki/Knapsack_problem) Wikipedia page.

The knapsack problem, in its simplest form, has only one constraint and is easily solvable. However, this problem is NP-complete for any problem with more than one constraint $` m \geq 2 `$). [^2] One can use commercial solvers such as CPLEX or Gurobi Optimizer to find a solution. However, the free version of these solvers has some limitations regarding the number of variables and constraints. Therefore, the purpose of this project is to go beyond the limitations of commercial solvers.


## Objective
To design a predictor for solving the following class of knapsack optimization problems, Dynamic Multidimensional Knapsack Problem (DMKP), using methods other than commercial solvers:

$$
\max 𝐜^T 𝐱 \quad \Bigg| \quad \sum_{i=1}^{n} a_i x_i \leq b_j, \quad  \text{for all} \quad 1 \leq j \leq m, \quad 𝐱 \in \\{0,1\\}^n 
$$

The simplest version of this problem is as follows:

$$
\max 𝐜^T 𝐱 \quad \Bigg| \quad \sum_{i=1}^{n} a_i x_i \leq b, \quad 𝐱 \in \\{0,1\\}^n
$$


## Technologies
Python, Random Forest (RF), XGBoost, Neural Network (NN), Naive Bayesian (NB), and Support Vector Machine (SVM)

## Table of Contents
- [Dataset](Datasets)
- Feature Selection
- ML Algorithms
- Performance Comparison
- 

## Datasets 
The 

## Creating a Dummy Dataset 
The dummy dataset is for 10,000 problems, where the size of each problem (number of variables) is from $$1$$ to $$30$$. The following algorithm can create
