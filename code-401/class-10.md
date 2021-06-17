# What is a Stack

- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.
## stacks follow these concepts:

- FILO First In Last Out : This means that the first item added in the stack will be the last item popped out of the stack.

- LIFO This means that the last item added to the stack will be the first item popped out of the stack.

visiual


# What is a Queue

# Queues follow these concepts:

- FIFO (First In First Out): This means that the first item in the queue will be the first item out of the queue.

- LILO (Last In Last Out): This means that the last item in the queue will be the last item out of the queue.


# Common terminology for a queue is

- Enqueue - Nodes or items that are added to the queue.
- Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- Front - This is the front/first Node of the queue.
- Rear - This is the rear/last Node of the queue.
- Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- IsEmpty - returns true when queue is empty otherwise returns false.
- FIFO (First In First Out) : This means that the first item in the queue will be the first item out of the queue.
- LILO : Last In Last Out

## Push O(1)

- Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

- When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

## Pop O(1)

- steps :

    - create a reference named temp that points to the same Node that top points to.
    - re-assign top
    - clear out the next property in your current temp reference
    - return the value of the temp Node that was just popped off.

- pseudocode for a pop
- ALGORITHM pop() // INPUT <-- No input // OUTPUT <-- value of top Node in stack // EXCEPTION if stack is empty Node temp <-- top top <-- top.next temp.next <-- null return temp.value
## Peek O(1)

- must be check if empty pseudocode for a peek
- ALGORITHM peek() // INPUT <-- none // OUTPUT <-- value of top Node in stack // EXCEPTION if stack is empty return top.value
