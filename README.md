# Missionaries and Cannibals

<img src="MC.png" alt="MC" width= “100%”/>

The missionaries and cannibals problem is usually stated as follows. Three missionaries and three cannibals are on one side of a river, along with a boat that can hold one or two people. Find a way to get everyone to the other side without ever leaving a group of missionaries in one place outnumbered by the cannibals in that place.(if they were, the cannibals would eat the missionaries). The boat cannot cross the river by itself with no people on board. This problem is famous in AI because it was the subject of the first paper that approached problem formulation from an analytical viewpoint (Amarel, 1968). *Source: “Artificial Intelligence: A Modern Approach.” Artificial Intelligence: A Modern Approach, by Stuart J. Russell and Peter Norvig, Pearson Education, Inc., 2010, pp. 115.*

## Semantic Networks Agent 

This Python project implements an agent that can solve a scaled-up version of the classic Missionaries and Cannibals problem in AI with an arbitrary number of missionaries and cannibals using breadth-first-search (BFS) algorithm.

## How to Run

python3.8 main.py

SemanticNetsAgent.py will return a list of moves that will result in the successful solving of the problem. These are only the moves that the agent ultimately selected to be performed, not the entire web of possible moves. Each item in the list should be a 2-tuple where each value is an integer representing the number of missionaries (the first integer) or cannibals (the second integer) to be moved; we assume the moves are alternating. So, if your first move is (1, 1), that means you’re moving one missionay and one cannibal to the right. If your second move is (0, 1), that means you’re moving one cannibal to the left.

For example, one possible solution to the test case of 3 missionaries and 3 cannibals would be:

[(1, 1), (1, 0), (0, 2), (0, 1), (2, 0), (1, 1), (2, 0), (0, 1), (0, 2), (0, 1), (0, 2)]

The result of running the moves in order should be (a) that all people are successfully moved from left to right, and (b) that all intermediate states along the way are valid (cannibals never outnumber missionaries in any state).
