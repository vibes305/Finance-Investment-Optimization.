# Finance-Investment-Optimization.
Financial Investment Optimization using Linear Programming and Scenario Analysis.

## 1. INTRODUCTION
<p align="justify">
In the context of financial investments, we're presented with a scenario where an investor has £20,000 and various options for allocation, including stocks, options, and bonds. The challenge is to optimize this allocation to maximize expected profit while considering different scenarios for the future stock price of XYZ. In Part IIA, we'll formulate and solve linear programs to achieve this goal, both with and without the constraint of ensuring a minimum profit of £2,000 in any scenario. These analyses aim to inform the investor's financial decisions, balancing profit objectives and risk management.
</p>

## 2. METHODOLOGY
- Scenario Analysis: Considered three future scenarios for the price of stock XYZ: no change (£20), increase (£40), and decrease (£12). Each scenario is assumed equally likely.
- Linear Programming Formulation (Problem 1):
1. Define decision variables: S (Stocks), B (Bonds), C1 (Call-options purchased), and C2 (Call-options sold).
2. Maximize profit using the linear expression 10B + 4S.
3. Subject to constraints: Budget constraint, limitations on buying and selling call options, and non-negativity constraints.
- Linear Programming Formulation (Problem 2 - With Constraint):
1. Introduce an investor's profit constraint of at least £2,000 in any scenario.
2. Formulate the LP problem with an additional constraint.
3. Maximize profit while ensuring the minimum profit requirement in each scenario.
- Linear Programming Solving: Use the SciPy library's linprog function for solving the linear programs.
- Optimal Solution Analysis: Evaluate and interpret the optimal solutions for each problem.
- Gurobi Linear Programming: Implement the linear program using Gurobi library for comparison.
- Introduction of New Variable (Problem 2): Introduce the variable K to represent the least possible revenue and maximize Z.
- Gurobi Linear Programming (Problem 2): Implement the linear program with the Gurobi library to maximize Z.
- Optimal Solution Analysis (Problem 2): Interpret and analyze the optimal solutions considering the additional constraint.
