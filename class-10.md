# Stacks & Queues

## What is a Stack?

- `Stacks` are data structures made up up `Nodes`

  - Each Node has a reference to the _following_ Node in a given stack
  - Nodes do _not_ reference previous Nodes in a stack

- The `Call Stack` is perhaps the best-known example of a stack that developers use constantly

- Stacks follow `FILO/LIFO` concepts:
  - `FILO` = First In/Last Out
  - `LIFO` = Last In/First Out
  - Both of these equate to the same thing: The first item added to the stack (at the "bottom") will be the last item removed from the stack
  - New items will be added atop previous items - and lower items cannot be resolved until all items above them have been resolved first

## Stack Methods

- `push()`: This will always be an `O(1)` operation, regardless of how many Nodes are in a stack

  - Nodes are pushed into the stack and assigned as a new top
  - Nodes' `next` property are set to the original "top" Node

- `pop()`: This will always be an `O(1)` operation, regardless of how many Nodes are in a stack

  - Removes topmost Node from the stack
  - Top Node is returned to user
  - "Top" property is reassigned to the previous top's "next" Node

- `peek()`: This will always be an `O(1)` operation

  - Inspects the top Node of a stack
  - Cannot peek on an empty stack
  - Will return the value of the topmost Node in a stack

- `isEmpty()`: This will always be an `O(1)` operation
  - Only checks to see if the topmost Node in a stack is _null_
  - If null, returns a Boolean "true" to indicate the stack is empty

## What is a Queue?

- `Queues` are data structures made up up `Nodes`

  - Each Node has a reference to the _following_ Node in a given stack

- Queues follow `FIFO/LILO` concepts:
  - `FILO` = First In/First Out
  - `LIFO` = Last In/Last Out
  - Both of these equate to the same thing: The first item added to a queue will be the first item removed from a queue
  - New items will be added "behind" previous items - much like a real-life queue of people

## Queue Methods

- `enqueue()`: This will always be an `O(1)` operation, regardless of how many Nodes are in a queue

  - Nodes are pushed into the queue and assigned as a new "next" Node

- `dequeue()`: This will always be an `O(1)` operation, regardless of how many Nodes are in a queue

  - Removes Node from the front of the queue
  - Front Node is returned to user

- `peek()`: This will always be an `O(1)` operation

  - Inspects the front Node of a queue
  - Cannot peek on an empty queue
  - Will return the value of the frontmost Node in a queue

- `isEmpty()`: This will always be an `O(1)` operation
  - Only checks to see if the frontmost Node in a queue is _null_
  - If null, returns a Boolean "true" to indicate the queue is empty

