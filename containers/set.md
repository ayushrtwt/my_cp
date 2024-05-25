Store everything in **sorted order and unique**

Inside a **Tree** is maintained, not linear.

In set everything happens at **log(n).**

**Using st.find().** If element is not in the set it will always return st.end() (an iterator which points to right after end)

```cpp
// Declare a set of integers
    set<int> st;

    // Inserting elements into the set
    st.insert(1);     // Set: {1}
    st.emplace(2);    // Set: {1, 2}
    st.insert(2);     // Duplicate element, no change (Set: {1, 2})
    st.insert(4);     // Set: {1, 2, 4}
    st.insert(3);     // Set: {1, 2, 3, 4}

    // Finding elements in the set
    auto it = st.find(3);   // Find element 3 in the set
    // it points to the position of 3 in the set, or st.end() if not found

    auto it_not_found = st.find(6); // Find element 6 in the set
    // it_not_found equals st.end() since 6 is not present in the set

    // Erasing elements from the set
    st.erase(5);  // No effect since 5 is not in the set (logarithmic time)

    int cnt = st.count(1); // Count occurrences of element 1 in the set (returns 1)

    auto it_to_erase = st.find(3);  // Find element 3 again
    st.erase(it_to_erase);  // Erase the element pointed by 'it_to_erase' (constant time)

    auto it1 = st.find(2);   // Find element 2
    auto it2 = st.find(4);   // Find element 4
    st.erase(it1, it2);      // Erase elements in the range [it1, it2) (exclusive of it2)

    // Finding lower and upper bounds
    auto lower_bound_it = st.lower_bound(2);  // Iterator to the first element not less than 2
    auto upper_bound_it = st.upper_bound(3);  // Iterator to the first element greater than 3

```
