Given an integer array `nums` which is sorted in **ascending order** and all of its elements are **unique** and given also an integer `k`, return the `kth` missing number starting from the leftmost number of the array.


difficult, ideally solved with [[Binary search]] beacuse there is a sorted array and binary search is only works with it

Mainly you have to write a function that can determine how many numbers are missing before the current in an array, this way you juts find k that sits between `missing(idx - 1) < k <= missing(idx)`

difficult