# Stacks and Queues

## [stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)


Let's tackle the topic of stacks and queues using the different approaches you've mentioned. We'll start with an analogy.

## Analogy:
Imagine you're in a cafeteria line waiting to get your food. You stand behind others who arrived before you, forming a queue. As the person at the front of the line receives their food, they leave, and everyone else moves forward one spot. This is similar to a queue in computer science. The first person in the line gets served first, and the last person in the line has to wait the longest.

On the other hand, imagine you have a stack of plates on a table. You can only add or remove plates from the top of the stack. This is similar to a stack in computer science. The last plate you put on the stack is the first one you can take off.

Now, let's explore stacks and queues in more detail using the WHY, WHAT, HOW structure.

## Stacks:
WHY: Stacks are useful when you need to keep track of elements in a last-in, first-out (LIFO) manner. They are commonly used in programming for tasks like function calls, storing undo operations, and expression evaluation.

WHAT: A stack is a data structure that follows the LIFO principle. It consists of elements arranged in a linear order, where insertion and deletion of elements occur only at one end called the top. The element at the top is the one accessible for retrieval or removal.

HOW: You can implement a stack using an array or a linked list. When adding elements, it's called "push," and it adds an element to the top of the stack. When removing elements, it's called "pop," and it removes the element from the top of the stack. Additionally, you can "peek" at the top element without removing it.

### **Example**:
Let's say we have a stack of integers: [1, 2, 3]. If we push the number 4 onto the stack, it becomes [1, 2, 3, 4]. If we then pop an element from the stack, we remove 4, and the stack becomes [1, 2, 3] again.

Next, let's move on to queues.

## Queues:
**WHY**: Queues are useful when you need to manage elements in a first-in, first-out (FIFO) manner. They are commonly used for tasks like scheduling processes, handling requests, and managing printer jobs.

**WHAT**: A queue is a data structure that follows the FIFO principle. It represents a collection of elements in a linear order, where insertion happens at one end (rear), and deletion occurs at the other end (front). The element at the front is the one accessible for retrieval or removal.

**HOW**: Similar to stacks, you can implement queues using an array or a linked list. When adding elements, it's called "enqueue," and it adds an element to the rear of the queue. When removing elements, it's called "dequeue," and it removes the element from the front of the queue. You can also "peek" at the front element without removing it.

### **Example**:
Let's say we have a queue of characters: [A, B, C]. If we enqueue the character D, it becomes [A, B, C, D]. If we then dequeue an element from the queue, we remove A, and the queue becomes [B, C, D].

Now, let's move on to a quiz to test your understanding.

Quiz:
1. Which data structure follows the LIFO principle?
   1. Queue
   1. Stack
   1. Array
   1. Linked list

2. Which data structure follows the FIFO principle?
   1. Queue
   1. Stack
   1. Array