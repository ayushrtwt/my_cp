```cpp
// Declare a deque of integers
    deque<int> dq;

    // Adding elements to the deque
    dq.push_back(1);         // dq: {1}
    dq.emplace_back(2);      // dq: {1, 2}

    dq.push_front(4);        // dq: {4, 1, 2}
    dq.emplace_front(3);     // dq: {3, 4, 1, 2}

    // Removing elements from the deque
    dq.pop_back();           // dq: {3, 4, 1}
    dq.pop_front();          // dq: {4, 1}

    // Accessing elements in the deque
    int backElement = dq.back();   // backElement = 1 (last element in deque)
    int frontElement = dq.front();  // frontElement = 4 (first element in deque)

    // Output the elements in the deque
    cout << "Elements in deque: ";
    for (auto num : dq) {
        cout << num << " ";
    }
    cout << endl;

    // Output the back and front elements
    cout << "Back element: " << backElement << endl;
    cout << "Front element: " << frontElement << endl;
```
