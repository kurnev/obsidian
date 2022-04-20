**In browser**
![](https://miro.medium.com/max/529/0*R5ERVqo86TC5cDkt.png)
The call stack is a place in memory that keeps track of the function executing at that time, and the functions that are going to be executed after that.

The web API is not part of the core JS, instead, it provides various methods that can be used by a Javascript program, like `setTimeout()` or `alert()`.

The message queue is a list of messages, waiting to be executed by their associated functions. A new message is added to the list, each time an event, that has been watched by an event listener, occures.

The event loop is a process that keeps running and checks whether the call stack is empty or not. If the call stack is empty, it pushes the first item of the message queue into the call stack for execution.

**In Node.js**