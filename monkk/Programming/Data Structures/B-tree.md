*B-tree** is a self-balancing [tree data structure] that maintains sorted data and allows searches, sequential access, insertions, and deletions in [logarithmic time]



It should have following properties: 

1.  Every node has at most _m_ children.
2.  Every non-leaf node (except root) has at least ⌈_m_/2⌉ child nodes.
3.  The root has at least two children if it is not a leaf node.
4.  A non-leaf node with _k_ children contains _k_ − 1 keys.
5.  All leaves appear in the same level and carry no information.