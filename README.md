Queue Implementation in C

This is a simple implementation of a queue data structure in C. The queue is implemented using an array with dynamic memory allocation and supports basic queue operations such as enqueue (push), dequeue (pop), peek, checking if the queue is empty or full, and printing the elements of the queue.

Features
Dynamic memory allocation for the queue array.
Enqueue (Push): Add an element to the rear of the queue.
Dequeue (Pop): Remove an element from the front of the queue.
Peek: View the element at the front of the queue without removing it.
Size: Get the current number of elements in the queue.
Is Empty: Check if the queue is empty.
Is Full: Check if the queue is full.
Print Elements: Display all the elements in the queue.

How to Use
Clone or download this repository to your local machine.

Compile the program using a C compiler, for example:

bash
gcc -o queue queue.c
Run the program:

bash
./queue
The program will prompt you to input the capacity of the queue. You can then interact with the queue using the menu options.

Functions
void initQueue(struct Queue* queue, int capacity)
Initializes the queue with a given capacity.
int isFull(struct Queue* queue)
Checks if the queue is full.
Returns 1 if full, otherwise returns 0.
int isEmpty(struct Queue* queue)
Checks if the queue is empty.
Returns 1 if empty, otherwise returns 0.
void push(struct Queue* queue, int value)
Enqueues a new value at the rear of the queue.
Prints an error message if the queue is full.
int pop(struct Queue* queue)
Dequeues the front element of the queue.
Returns the dequeued value, or -1 if the queue is empty.
int peek(struct Queue* queue)
Returns the front element of the queue without removing it.
Returns -1 if the queue is empty.
int size(struct Queue* queue)
Returns the number of elements currently in the queue.
void printElements(struct Queue* queue)
Prints all the elements in the queue.
Prints a message if the queue is empty.

Example
markdown
Enter the capacity of the queue: 5

Menu:
1. Enqueue (Push)
2. Dequeue (Pop)
3. Peek
4. Size
5. Is Empty
6. Is Full
7. Print Elements
8. Exit
Enter your choice: 1
Enter value to enqueue: 10
Enqueued element: 10

Menu:
1. Enqueue (Push)
2. Dequeue (Pop)
3. Peek
4. Size
5. Is Empty
6. Is Full
7. Print Elements
8. Exit
Enter your choice: 7
Queue elements: 10

Requirements
C Compiler (e.g., GCC)
Standard C library functions

License
This project is open-source and available under the MIT License.

