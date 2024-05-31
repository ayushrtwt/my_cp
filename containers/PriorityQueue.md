Data stored inside is not linear, a **TREE** is maintained

**Largest num, string** stays at the top (top depends on priority)

Here **push and pop is log(n)**

**top is O(1)**

```cpp
// Declare a priority queue of integers (default max-heap)
    priority_queue<int> pq;

    // Pushing elements into the priority queue
    pq.push(5);     // Priority Queue: [5]
    pq.push(2);     // Priority Queue: [5, 2]
    pq.push(8);     // Priority Queue: [8, 5, 2] (max-heap order)
    pq.emplace(10); // Priority Queue: [10, 8, 5, 2] (max-heap order)

    // Accessing and printing the top element (max element)
    cout << pq.top(); // Output: 10 (max element)

    // Removing the top element (max element)
    pq.pop(); // Priority Queue: [8, 5, 2]

    // Accessing and printing the new top element (max element)
    cout << pq.top(); // Output: 8 (new max element)

    // Declare a priority queue of integers using min-heap order
    priority_queue<int, vector<int>, greater<int>> pq_min;

    // Pushing elements into the min-heap priority queue
    pq_min.push(5);     // Priority Queue (Min-Heap): [5]
    pq_min.push(2);     // Priority Queue (Min-Heap): [2, 5] (min-heap order)
    pq_min.push(8);     // Priority Queue (Min-Heap): [2, 5, 8] (min-heap order)
    pq_min.emplace(10); // Priority Queue (Min-Heap): [2, 5, 8, 10] (min-heap order)

    // Accessing and printing the top element (min element)
    cout << pq_min.top(); // Output: 2 (min element)
```
