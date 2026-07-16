
📌 What is Time Complexity?

Imagine two students solving the same math problem.

👨 Student A takes 5 seconds

👨 Student B takes 30 seconds

Both give the correct answer.

Which one is better?

Obviously,
Student A, because he solved it faster.

Exactly the same thing happens in programming.

Sometimes,
many programs give the correct answer.

But the program that takes less time is considered the better algorithm.

This is called Time Complexity.

📖 Definition

Time Complexity tells us how the running time of an algorithm increases as the input size increases.

Example 1

.Suppose you have

10 numbers

Searching one by one takes

10 operations

.Now imagine

100 numbers

Searching one by one may take

100 operations

.Now

1000 numbers

Searching may take

1000 operations

.As the input increases,

operations also increase.

This growth is called Time Complexity.



.What is Big O Notation?

Big O is simply a way to write Time Complexity.
{
O(1)

O(log n)

O(n)

O(n log n)

O(n²)

O(2ⁿ)

O(n!)
}

Here n is the size of the input. 

1. O(1) — Constant Time ⭐⭐⭐⭐⭐
 This is the fastest.

No matter how big the input becomes,

the work remains the same.

  Example: 
  
```java
int[] arr = {5,8,2,9};

System.out.println(arr[2]);
```

Whether the array has   

4 elements

400 elements

400000 elements

Finding

arr[2]

always takes one direct access.
hence O(1)

Real-life example

You know your friend's phone number is saved at position 25 in your contacts. You open it directly instead of checking every contact one by one.




2. O(n) — Linear Time ⭐⭐⭐⭐⭐

Suppose you want to find

50 inside an array.
```java
for(int i=0;i<n;i++)
{
    if(arr[i]==50)
        break;
}
```

Worst case
You check every element. If n=10 -> 10 opt
if n=100 then 100 opt
hence o(n)

Real-life example
Finding your name in an attendance sheet by checking one name after another.


3. O(n²) — Quadratic Time

This usually happens when one loop is inside another.

Example
```java
for(int i=0;i<n;i++)
{
    for(int j=0;j<n;j++)
    {
        System.out.println(i+" "+j);
    }
}
```
Real-life example

Every student shakes hands with every other student.
If there are more students, the number of handshakes increases much faster.

4. O(log n) — Logarithmic Time

This is one of the best complexities.
Instead of checking one by one,
it cuts the search space into half every time.

Example

Binary Search
100 elements
↓
50
↓
25
↓
12
↓
6
↓
3
↓
1

Real-life example

Looking for a word in a dictionary. You don't start from page 1—you open near the middle and keep narrowing down.


5. O(n log n)

Algorithms like

Merge Sort
Heap Sort
Quick Sort (average case)
have this complexity.
This is considered very efficient for sorting large datasets.



| Time Complexity | Name              |   Performance  |            Growth Rate           | Common Example                                    | Interview Rating |
| :-------------: | :---------------- | :------------: | :------------------------------: | :------------------------------------------------ | :--------------: |
|     **O(1)**    | Constant Time     |  ⭐⭐⭐⭐⭐ Fastest | Doesn't increase with input size | Array Indexing (`arr[i]`), Stack `push()`/`pop()` |       ⭐⭐⭐⭐⭐      |
|   **O(log n)**  | Logarithmic Time  | ⭐⭐⭐⭐ Very Fast | Input is divided by 2 repeatedly | Binary Search                                     |       ⭐⭐⭐⭐⭐      |
|     **O(n)**    | Linear Time       |    ⭐⭐⭐ Good    |  Grows directly with input size  | Linear Search, Single Loop                        |       ⭐⭐⭐⭐       |
|  **O(n log n)** | Linearithmic Time |  ⭐⭐ Efficient  |     Slightly more than Linear    | Merge Sort, Heap Sort, Average Quick Sort         |       ⭐⭐⭐⭐⭐      |
|    **O(n²)**    | Quadratic Time    |     ⭐ Slow     |           Nested loops           | Bubble Sort, Selection Sort                       |        ⭐⭐⭐       |
|    **O(2ⁿ)**    | Exponential Time  |   ❌ Very Slow  |   Doubles with every new input   | Naive Fibonacci Recursion                         |         ⭐        |
|    **O(n!)**    | Factorial Time    |     ❌ Worst    |      Explodes extremely fast     | Generating All Permutations, Brute Force TSP      |         ⭐        |


> **Rule to Remember**
>
> The smaller the Time Complexity, the faster and more scalable the algorithm.
>
> O(1) > O(log n) > O(n) > O(n log n) > O(n²) > O(2ⁿ) > O(n!)






