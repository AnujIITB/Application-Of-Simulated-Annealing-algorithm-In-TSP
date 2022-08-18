# Application-Of-Simulated-Annealing-algorithm-In-TSP
TSP is a NP hard problem.
Finding optimal solutions are computationally expensive as problem size becomes bigger.
Simulated annealing is a heuristic method to find near optimal solution.
This code is written in python to use Simulated Annealing to solve TSP problems with bigger sizes.
This algorithm uses the nearest neighbor search algorithm to find an initial solution.
The initial solution is improved by using simulated annealing for a predefined number of iterations.
In Simulated Annealing, if we keep waiting for better solution, the algorithm may stuck in a local minima.
To get over local minima and locate global minima, bad solutions are also accepted in a conditional basis. 
Condition used is a probability (normal distribution with mean = 50% and s.d = 5%) of finding better solutions in future.

In this project i compair optimal solution from metaheuristic Simulated-Annealing algorithm with the  solution of Mixed integer linear programming 
the dataset is TSP-11 and TSP-48 , got  4.3% error in solution of simulated annealing algorithm as compared to MILP.

