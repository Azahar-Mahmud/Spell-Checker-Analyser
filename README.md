# Spell-Checker-Analyser
This program is a robust spell checker and analyzer designed to identify misspelled words, suggest corrections, and track performance metrics. It leverages efficient algorithms such as hash tables for dictionary management, string matching for word validation, and dynamic programming (Knapsack and LCS) to optimize suggestion selection based on similarity scores. The tool processes input files, evaluates spelling accuracy and provides relevant corrections while logging execution times for analysis.

Dynamic Programming Explained Through the Code:
Dynamic Programming (DP) is a problem-solving technique that breaks complex problems into smaller, overlapping subproblems, solves each subproblem only once, and stores their solutions to avoid redundant calculations. Let's analyze how it works in your code using the Knapsack algorithm as an example.


Key Concepts of Dynamic Programming in This Code:
1. State Representation: The state is represented by a 2D array dp[k][j], which represents the number of items considered (up to a maximum number of items).
2. Recurrence Relation: The recurrence relation is based on whether to include an item or not: If an item can be included (i.e., its weight is less than or equal to the current capacity), we check if including it yields a higher profit than excluding it.
3. Initialization: The DP table is initialized with -1 to indicate uncomputed states, except for dp, which is set to 0 (no items and no capacity yields zero profit).
4. Backtracking: After filling the DP table, we backtracked to determine which items were included to achieve the maximum profit.
