# Search Algorithms
2024-04-04 | 15:21
{Subject}:[[]]
{Section}:[[]]
{Tags}: #
{Related}:

--- 
Depth First Search Algorithm
- The DFS is a recursive algorithm for traversing a tree or graph data structure
- The search algorithm is called DFS simply because it start from the root node and follow each path to its greatest depth node before moving to the next step path.
- The DFS algorithm uses a stack data structure for its implementation
- The process is similar to BFS algorithm

Advantages
- DFS requires very less memory as it only needs to store a stack of the node on the path from root node to the current node
- DFS takes less time to reach to the goal node than the BFS algorithm

Disadvantages
- There is the possibility that many states keep re-occurring and there is no guarantee of finding a solution
- DFS algorithm goes for the deep down searching and sometimes it may go to the infinite loop

Analysis of the DFS in terms of
Completeness: DFS is complete within finite state space, meaning for a given finite search tree, DFS will come up with a solution if it exists.

Optimality: DFS is not optimal considering the fact that it has the potential to generate large number of steps or high cost to reach the goal node.
Time complexity: $T(n)=1+n^2+n^3+\ldots+n^m$
Where $\mathrm{m}=\max$ depth of any node
Space complexity
$\mathrm{S}(\mathrm{c})$ is the order of $O(\mathrm{bm})$
Note that the DFS needs to only store single path, so it requires less memory, hence
$S(c)=O(b m)$
Where $m$ is the maximum depth of any node and $b$ stands for the level

--- 
{Efundi Lecture Notes}: [Search Algorithms]()
