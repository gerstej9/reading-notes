# Code 401 Class 08 Reading Notes

## Teaching instructions for using Pop() to remove a node from a stack
* To remove a node from a stack one must first assign the top node value to a temporary variable
* Once this is done the next node in the stack, node.next, must be assigned to the top
* Lastly the value of the old top should be returned
* Code for this operation looks like the following
* ```let temp = this.top; let this.top = temp.next; return temp.value```

## Stacks
* A stack is a data structure composed of nodes which refer to the next node in the stack
* Nodes are pushed onto the stack and popped off, the top is the most recently added and you can peek at the value of the top
* The function isEmpty() returns a boolean based on whether or not the stack is empty
* Stacks operate LIFO so the last added node is the first to be removed and FILO so the first node added is the last out
* Pushing a node onto a stack is a O(1) operation
* Popping a node off the stack is also O(1)
* As are Peek and isEmpty

## Queue
* A queue is similar to a stack but operates on FIFO and LILO principals meaning first in first out and last in last out
* Enqueue is the addition of nodes to the queue
* Dequeue is the removal of nodes to the queue
* Front refers to the oldest node in the stack and one to be dequeued
* Rear fers to the newest node in the stack and one that was most recently enqueued
* Peek is looking and the front and isEmpty serves the same purpose as it does in stacks
* Like stacks, the queue operations mentioned above are all O(1) operations.

[Source for all notes comes from Code Fellows](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)


[Table of Contents](README.md)