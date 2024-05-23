In stack there are mainly 3 functions: **push, pop, top** (and operations in stack are **big O(1)**)

**LIFO**

```cpp
// Declare a stack of integers
    stack<int> st;

    // Pushing elements onto the stack
    st.push(1);     // Stack: [1]
    st.push(2);     // Stack: [1, 2]
    st.push(3);     // Stack: [1, 2, 3]
    st.push(3);     // Stack: [1, 2, 3, 3] (allows duplicates)
    st.emplace(5);  // Stack: [1, 2, 3, 3, 5]

    // Accessing and removing the top element
    cout << st.top();  // Output: 5 (top element)
    st.pop();          // Remove the top element (5)

    cout << st.top();  // Output: 3 (new top element)
    cout << st.size(); // Output: 3 (number of elements in the stack)
    cout << st.empty(); // Output: 0 (stack is not empty)

    // Swapping two stacks
    stack<int> st1, st2;
    st1.swap(st2);  // Swap contents of st1 and st2
```
