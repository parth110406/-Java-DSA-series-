💾 Space Complexity
📌 What is Space Complexity?
Space Complexity tells us how much extra memory (RAM) an algorithm needs to solve a problem.

Simple Definition:
Space Complexity is the amount of memory used by an algorithm as the input size (n) increases.


🤔 Why is Space Complexity Important?

A fast algorithm is good, but if it uses too much memory, it may not work efficiently on large datasets.

Companies like Google, Amazon, Microsoft, and Meta care about both:

⚡ Time (How fast?)
💾 Space (How much memory?)

An ideal algorithm uses less time and less memory

📌 Example 1 – O(1) Space (Constant Space)
```java
int sum = 0;

for(int i = 0; i < n; i++){
    sum += arr[i];
}
```

Explanation

Only two variables are used:

.sum
.i
Whether the array has:

.10 elements
.100 elements
.1,000,000 elements

The number of extra variables remains the same.
Space Complexity => O(1)

🏠 Real-Life Example
You have one notebook.
Whether you solve 10 questions or 1000 questions, you still use the same notebook.


📌 Example 3 – O(n²) Space
```java
int[][] matrix = new int[n][n];
```
Explanation

A 2D array of size n × n is created.
If:
n = 5 → 25 cells
n = 100 → 10,000 cells
Memory grows much faster.

Space Complexity=>O(n²)

🏠 Real-Life Example
A classroom where every student gets an entire row and column of seats.
