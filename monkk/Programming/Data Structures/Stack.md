Only has two actions:

push to the top
pop (remove the topmost and read it)

(Lets say we have Box which contains a lot of boxes (Box A, Box B, Box C) which might contain another boxes)
Using call stack is convenient when you do a recursive search, stack saves info about Box A in the stack itself. You don't have to keep track of a pile of boxes.

But saving all that info may take A LOT of memoty.