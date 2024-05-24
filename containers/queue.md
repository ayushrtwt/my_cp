**FIFO,** all operations are in **big O(1)**

```cpp
// Declare a queue of integers
    queue<int> q;

    // Pushing elements onto the queue
    q.push(1);     // Queue: [1]
    q.push(2);     // Queue: [1, 2]
    q.emplace(4);  // Queue: [1, 2, 4]

    // Modifying and accessing the back element
    q.back() += 5;      // Increment the last element (4) by 5
    cout << q.back();   // Output: 9 (modified last element)

    // Accessing the front element
    cout << q.front();  // Output: 1 (first element)

    // Removing and accessing the new front element
    q.pop();            // Remove the first element (1)
    cout << q.front();  // Output: 2 (new first element)
```
