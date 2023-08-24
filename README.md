# C - Stacks and Queues (LIFO, FIFO)

This repository provides a basic implementation of stacks and queues in C programming language. Stacks and queues are fundamental data structures used in computer science to store and manage data.

## Stack (LIFO - Last-In-First-Out)

A stack is a linear data structure that follows the Last-In-First-Out (LIFO) principle. In a stack, the most recently added element is the first one to be removed.

### Implementation

The stack implementation consists of the following files:

- `stack.c`: Contains the implementation of stack operations such as push, pop, peek, and isEmpty.
- `stack.h`: Contains the function declarations and data structure definition for the stack.

#### Functionality

The stack implementation provides the following operations:

- `void push(Stack* stack, int value)`: Pushes an element onto the top of the stack.
- `int pop(Stack* stack)`: Removes and returns the top element from the stack.
- `int peek(Stack* stack)`: Returns the value of the top element without removing it.
- `int isEmpty(Stack* stack)`: Checks if the stack is empty and returns 1 if it is, 0 otherwise.

## Queue (FIFO - First-In-First-Out)

A queue is a linear data structure that follows the First-In-First-Out (FIFO) principle. In a queue, the first element added is the first one to be removed.

### Implementation

The queue implementation consists of the following files:

- `queue.c`: Contains the implementation of queue operations such as enqueue, dequeue, peek, and isEmpty.
- `queue.h`: Contains the function declarations and data structure definition for the queue.

#### Functionality

The queue implementation provides the following operations:

- `void enqueue(Queue* queue, int value)`: Adds an element to the end of the queue.
- `int dequeue(Queue* queue)`: Removes and returns the front element from the queue.
- `int peek(Queue* queue)`: Returns the value of the front element without removing it.
- `int isEmpty(Queue* queue)`: Checks if the queue is empty and returns 1 if it is, 0 otherwise.

## Usage

To use the stack and queue implementations in your C program, follow these steps:

1. Copy the `stack.c`, `stack.h`, `queue.c`, and `queue.h` files into your project directory.
1. Include the respective headers (`stack.h` or `queue.h`) in your C source code.
1. Use the provided functions to perform stack or queue operations.

```c
#include <stdio.h>
#include "stack.h" // or include "queue.h" for queue implementation

int main() {
    Stack stack;
    stackInitialize(&stack); // Initialize the stack

    push(&stack, 10); // Push an element onto the stack
    push(&stack, 20);
    push(&stack, 30);

    printf("Stack elements: ");
    while (!isEmpty(&stack)) {
        printf("%d ", pop(&stack)); // Pop and print the stack elements
    }
    printf("\n");

    return 0;
}
```
