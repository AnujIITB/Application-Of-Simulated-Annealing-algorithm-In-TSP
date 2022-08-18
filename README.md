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

# TSP: Traveling Salesman Problem By MILP



Luego, el problema a optimizar es el siguiente:
$$\begin{align}
\min \quad & \sum_{e\in E} d_e x_e \\
\text{s.t.} \quad & \sum_{e=(i,j)\in E} x_e = 1  &&\forall i \in C \\
 & \sum_{e=(i,j)\in E} x_e = 1 && \forall j \in C  \\
 & u_i + 1 \leq u_j + M(1-x_{ij})&& \forall (i,j)\in E : j\neq 0 \\
 & x_e \in \{0,1\} && \forall (i,j)\in E\\
 & u_i \geq 0 && \forall i \in C
\end{align}$$
