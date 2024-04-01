knapsack_value Function:
Computes the total value of items in the knapsack based on the current solution.
It checks if the total weight of the items in the solution exceeds the maximum weight allowed. If so, it
returns 0, otherwise, it returns the total value.
generate_initial_solution Function:
Generates a random initial solution where each item is either included (1) or not included (0) in the
knapsack.
generate_neighbors Function:
Generates neighboring solutions by flipping a single bit in the current solution. This means it toggles the
inclusion status of one item at a time.
hill_climbing_knapsack Function:
Performs the hill climbing algorithm to find the best solution for the knapsack problem.
It starts with a random initial solution and iteratively explores neighboring solutions, moving towards
solutions with higher values.
If a neighbor has a higher value, it moves to that neighbor. If not, it stays at the current solution.
It keeps track of the global maximum value and solution encountered during the search process.
It also records local maxima and minima encountered during the search.
Main function:
Defines a set of items with their weights and values.
Specifies the maximum weight allowed in the knapsack and the maximum number of iterations for the
hill climbing algorithm.
Calls the hill_climbing_knapsack function with these parameters and prints out the best solution found,
its value, and lists of local maxima and minima encountered during the search.
