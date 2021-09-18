Find a fastest path for weighted [[graphs]] and directed acylic graphs

Uses [[Hash table]]s

You CAN NOT use Dijkstra algo if nodes have negative weight! [[Bellman-Ford algo]] can be used with negative weights

1. Find the “cheapest” node. This is the node you can get to in the least  
amount of time.
2. Update the costs of the neighbors of this node. I’ll explain what I mean by this shortly.
3.  Repeat until you’ve done this for every node in the graph
4.  Calculate the final path.

First important step is to find really cheapest node. 

It uses three [[Hash table]]: graph, cost, parent