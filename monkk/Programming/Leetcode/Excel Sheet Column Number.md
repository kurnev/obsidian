Given a string `columnTitle` that represents the column title as appear in an Excel sheet, return _its corresponding column number_.

For example:

A -> 1
B -> 2
C -> 3
...
Z -> 26
AA -> 27
AB -> 28


---

Solution 1: 

Create a mapping to alphabet using ascii code (65 is A)
Formula is :
	*weight* 26  ^ (position of char in given string)
	
for examlpe for AAA = 1 * 26^2 + 1 * 26^1 + 1 * 26^0