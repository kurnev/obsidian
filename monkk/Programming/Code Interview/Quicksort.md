average is O(n * log n) A fast sorting algorithm

but in worst case scenarion is O (n ^ 2)

Uses [[Divide and conquer]]

1. Pick pivot number (it is copmliacated but first element can be chosen, or better random)
2. Compare all numbers with pivot number and place them to the left array and to the right
3. Do the same for left and right part
4. Return when empty array or array of one element or two elements (they are ez to sort)

it is similar to  [[Inductive proofs]]