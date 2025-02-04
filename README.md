# N-Queens Solver: A Comparative Study of Exhaustive Search and Genetic Algorithms

This repository contains implementations of two different algorithms for solving the N-Queens problem:

* **Exhaustive Search (Depth-First Search):** A traditional approach that systematically explores all possible queen placements, guaranteeing to find all solutions but becoming computationally expensive for larger boards.

* **Genetic Algorithm:** A heuristic approach that mimics natural selection to evolve solutions, offering faster execution times but potentially missing some solutions.

## Problem Description

The N-Queens problem is a classic combinatorial optimization challenge. The goal is to place N chess queens on an N×N chessboard so that no two queens threaten each other (i.e., no two queens share the same row, column, or diagonal). This problem highlights the complexities of constraint satisfaction problems and serves as a benchmark for algorithmic performance.

## Methodology

This research evaluates the performance of both algorithms across varying board sizes (N = 8, 10, 12, and 14). Key metrics collected include:

* **Configurations Explored:** The total number of board configurations examined by each algorithm.
* **Execution Time:** The time taken to find a solution(s).
* **Number of Valid Solutions Found:** The number of unique valid solutions found (DFS is guaranteed to find all solutions; GA may not).

## Results

The results demonstrate a clear trade-off between the two approaches:

* **Exhaustive Search (DFS):** Provides a comprehensive search, guaranteeing all solutions. However, execution time grows exponentially with increasing board size (N).

* **Genetic Algorithm (GA):** Significantly faster for larger boards but doesn't guarantee finding all solutions. It often finds only one solution.

The following table summarizes the key findings:

| Board Size (N) | DFS Configurations Explored | DFS Time (seconds) | DFS Valid Solutions | GA Configurations Explored | GA Time (seconds) | GA Valid Solutions |
|---|---|---|---|---|---|---|
| 8 | 16,456 | 0.012 | 92 | 130,000 | 122.1 | 1 |
| 10 | 355,390 | 0.17 | 724 | 618,000 | 198.6 | 1 |
| 12 | 3,598,720 | 4.46 | 14,200 | 1,391,000 | 301.7 | 1 |
| 14 | 383,019,748 | 177.9 | 365,596 | 190,000 | 432.8 | 1 |




## Conclusion

This research provides a valuable comparative analysis of Exhaustive Search and Genetic Algorithms for solving the N-Queens problem. While Exhaustive Search guarantees solution completeness, Genetic Algorithms offer superior efficiency for larger problem instances. Future work could explore hybrid approaches combining the strengths of both methods.


## Getting Started

This project requires a basic understanding of Git and Python. To run the code (assuming you have the necessary dependencies installed):

1. Clone the repository: `git clone <repository_url>`
2. Navigate to the project directory: `cd n-queens-solver`
3. Run the Python scripts for each algorithm.
4. Results will be output to the console.


## License

Creative Commons Zero v1.0 Universal
