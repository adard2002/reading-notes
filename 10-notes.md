# Reading 10 Notes

[Home](README.md)

# Stacks and Queues

## What is a stack?
Datastructure which contains Nodes. Each node is a reference the next Node in the sequence or stack. Does not refer to the previous one. 

## Terminology for a Stack:
1. Push - Nodes or items being put into the stack (being pushed into the stack)
2. Pop - Means to remove a Node or item from a stack. If you attempt to pop an empty stack an error will be seen
3. Top - Top of the stack
4. Peek - Will view the value of the top Node in the stack. If you try to peek an empty stack an error will also be seen
5. IsEmpty - Returns true when a stack is empty. But if it's not empty it will return false

## Concepts of Stacks

### FILO
First In Last Out
Meaning: First item added in the stack will be the last item popped or taken out of the stack.

### LIFO
Last In First Out
Meaning: Last item added to the stack will be the first item popped or taken out of the stack.

### Push O(1)
Pushing a Node onto a stack will always be an O(1) operation. This is because it will always take the same amount no matter how many Nodes or (n) you have in a stack

### Pop O(1)
This is the action of removing a Node from the top. Which will result in the top Node being reassigned to the Node below it. Normally you would check isEmpty before doing a pop. 

### Peek O(1)
This is used if you want view only the top Node of the stack. You would also check isEmpty before conducting this action.

## What is a Queue
Similar to a Stack
Terminology for Queue:
1. Enqueue - Nodes or items being added to the queue
2. Dequeue - Nodes or items being removed from the queue. An error will be raised if this is used on an empty queue
3. Front - Front or first Node of the queue
4. Rear - Rear or last Node of the queue
5. Peek - This is used if you want to view the first or front Node in the queue. An error will be raised if this used on an empty queue
6. IsEmpty - Returns true when queue is empty otherwise returns false.

## Concepts of Queues
### FIFO
First In First Out
Meaning: First Item in the queue will be the First item out of the queue

### LILO
Last In Last Out
Meaning: Last item in the queue will be the last item out of the queue

### Enqueue O(1)
Adding an item to a queue is dnoe with an O(1) operation in time because it doesn't matter how many other items live in the queue or (n). It takes the same amount of time to perform the operation.

### Dequeue O(1)
Removing an item from a queue is done with an O(1) operation because it doesn't matter how many other items are in the queue, it jusst removes the front or first Node of the queue.

### Peek O(1)
Viewing the front Node of the queue. Before using the Peek action you want to check IsEmpty. This is being it will make sure an error isn't thrown. You can avoid this using a try/catch block.