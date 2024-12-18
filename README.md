# Dynamic Multidimensional Knapsack Optimization Problem
|![image](https://github.com/user-attachments/assets/18bd87d1-7a03-4d58-ab35-4181f409f766)|
|--|
|Example of a one-dimensional (constraint) knapsack problem: which books should be chosen to maximize the amount of money while still keeping the overall weight under or equal to 15 kg? A multiple-constrained problem could consider both the weight and volume of the books. (Solution: if any number of each book is available, then three yellow books and three grey books; if only the shown books are available, then all except for the green book.) [^1]|

[^1]: The image and its description are from [Knapsack problem](https://en.wikipedia.org/wiki/Knapsack_problem) Wikipedia page.

  The knapsack problem, in its simplest form, has only one constraint and is easily solvable. However, for an extension of it, with more than one constraint $` m \geq 2 `$, it is called a **multidimensional knapsack problem (MKP)** and is NP-complete. [^2] The MKP is a static problem, meaning all the decisions are made simultaneously; however, as in real life, the **dynamic multidimensional knapsack problem (DMKP)** is about making decisions over time. Pieces of information like the item expiration date, changes in budget, and volume are all time-dependent.
  Commercial solvers, such as CPLEX or Gurobi Optimizer, can be used to find a solution. However, the free version of these solvers has some limitations regarding the number of variables and constraints. Therefore, this project's purpose is to exceed commercial solvers' limitations. The static multidimensional knapsack problem is as follows:

$$
\max 𝐜^T 𝐱 \quad \Bigg| \quad \sum_{i=1}^{n} a_i x_i \leq b_j, \quad  \text{for all} \quad 1 \leq j \leq m, \quad 𝐱 \in \\{0,1\\}^n 
$$


## Objective
To design a predictor for solving the following class of knapsack optimization problems, Dynamic Multidimensional Knapsack Problem (DMKP), using methods other than commercial solvers:

$$
\max 𝐜^T 𝐱 \quad \Bigg| \quad \sum_{t=1}^{T} \sum_{i=1}^{n} a_it x_it \leq b_jt, \quad  \text{for all} \quad 1 \leq j \leq m, \quad 1 \leq t \leq T, \quad \text{and} \quad 𝐱 \in \\{0,1\\}^n 
$$


## Technologies
Python, Random Forest (RF), XGBoost, Neural Network (NN), Naive Bayesian (NB), and Support Vector Machine (SVM)

## Table of Contents
- [Dataset](Datasets)
- Feature Selection
- ML Algorithms
- Performance Comparison

## Datasets:
I used the following datasets in training the model 


The 

## Creating a Dummy Dataset 
The dummy dataset is for 10,000 problems, where the size of each problem (number of variables) is from $$1$$ to $$30$$. The following algorithm can create
