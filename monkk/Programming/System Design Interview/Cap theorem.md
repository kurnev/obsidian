Also  **Brewer's Theorem**
A distributed system can deliver only two of three characteristics:
_**consistency**, **availability**,_ and _**partition tolerance**_

### Consistency

Consistency means that all clients see the same data at the same time, no matter which node they connect to.

### Availability

Availability means that that any client making a request for data gets a response, even if one or more nodes are down.

### Partition tolerance

A _partition_ is a communications break within a distributed system—a lost or temporarily delayed connection between two nodes. Partition tolerance means that the cluster must continue to work despite any number of communication breakdowns between nodes in the system.

https://www.ibm.com/cloud/learn/cap-theorem