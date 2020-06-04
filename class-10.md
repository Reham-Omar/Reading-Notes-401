# Stacks and Queues

## What is a Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

**Common terminology for a stack is**

1. Push - Nodes or items that are put into the stack are pushed /`Push O(1)`
2. Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised /`Pop O(1)`
3. Top - This is the top of the stack.
4. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised /`Peek O(1)`
5. IsEmpty - returns true when stack is empty otherwise returns false/`IsEmpty O(1)`

**Stacks follow these concepts:**

`FILO`
First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

`LIFO`
Last In First Out

## Stack Visualization

![Image](img/stack1.png)

## What is a Queue

### Common terminology for a queue is

- Enqueue - Nodes or items that are added to the queue.
- Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- Front - This is the front/first Node of the queue.
- Rear - This is the rear/last Node of the queue.
- Peek - When you `peek` you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- IsEmpty - returns true when queue is empty otherwise returns false.

## Queue Visualization
![Image](img/Queue.png)
