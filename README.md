Download Link: https://assignmentchef.com/product/solved-ai-lab7-tabu-search-algorithm
<br>
<h1>Taxonomy</h1>

Tabu Search is a Global Optimization algorithm and a Metaheuristic or Meta-strategy for controlling an embedded heuristic technique. Tabu Search is a parent for a large family of derivative approaches that introduce memory structures in Metaheuristics, such as Reactive Tabu Search and Parallel Tabu Search.

<h1>Strategy</h1>

The objective for the Tabu Search algorithm is to constrain an embedded heuristic from returning to recently visited areas of the search space, referred to as cycling. The strategy of the approach is to maintain a short term memory of the specific changes of recent moves within the search space and preventing future moves from undoing those changes. Additional intermediate-term memory structures may be introduced to bias moves toward promising areas of the search space, as well as longer-term memory structures that promote a general diversity in the search across the search space.

<h1>Procedure</h1>

Algorithm (below) provides a pseudocode listing of the Tabu Search algorithm for minimizing a cost function. The listing shows the simple Tabu Search algorithm with short term memory, without intermediate and long term memory management.




<strong>Figure 1. </strong>Pseudocode for Tabu Search.

<h2>Heuristics</h2>

adapted to manage any neighborhood exploration heuristic.

crete domains

such as combinatorial optimization problems.

neighborhood or the neighborhood can be stochastically sampled to a fixed size, trading off efficiency for accuracy.

-term memory structures can be introduced (complementing the short-term

memory) to focus the search on promising areas of the search space (intensification), called aspiration criteria.

-term memory structures can be introduced (complementing the short-term memory) to encourage useful exploration of the broader search space, called diversification. Strategies may include generating solutions with rarely used components and biasing the generation away from the most commonly used solution components.










<h2>Exercise</h2>

In this week, you implement a Tabu Search algorithm to solve a scheduling problem. Table 1 and 2 describes a scheduling problem. Each entry in Table 1 represents how long it takes for switching from one job to another job. For example, the entry [1,2] ([Job1, Job2]=12) is the time for switching job 1 to job 2 in Table 1. The entries in Table 2 is the time a machine completes the corresponding job. For example, the entry [2,3] ([Machine2, Job3]=5) is the time machine 2 completes job 3.




The problem in here is to assign each of the 3 jobs to one of the machines in such a way that the total time to complete all jobs is minimized. Implement a simulated annealing algorithm for this problem.