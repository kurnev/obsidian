A linked list is a data structure that represents a sequence of nodes. In a singly linked list, each node points to the next node in the linked list. A doubly linked list gives each node pointers to both the next younode and the previous node.

[[Big O]]

**Access**: avg O(n) worst O(n)
**Search**: avg O(n) worst O(n)
**Insertion**: avg O(n) worst O(1)
**Deletion**: avg O(n) worst O(1)

More generally - the cost to do an insertion or deletion in a singly-linked list is O(1), assuming you have a pointer to the node right before the one you want to insert or delete. However, you might have to do extra work (up to Θ(n)) to find that node.

The "runner" (or second pointer) technique is used in many linked list problems. The runner technique  
means that you iterate through the linked list with two pointers simultaneously, with one ahead of the  
other. The "fast" node might be ahead by a fixed amount, or it might be hopping multiple nodes for each  
one node that the "slow" node iterates through.


```ts

class ListNode {
    constructor(data) {
        this.data = data
        this.next = null                
    }
}

class LinkedList {
    constructor(head = null) {
        this.head = head
    }
}

size() {
    let count = 0; 
    let node = this.head;
    while (node) {
        count++;
        node = node.next
    }
    return count;
}

clear() {
    this.head = null;
}

getLast() {
    let lastNode = this.head;
    if (lastNode) {
        while (lastNode.next) {
            lastNode = lastNode.next
        }
    }
    return lastNode
}

getFirst() {
    return this.head;
}```