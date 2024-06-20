Element stored are sorted and **(not unique)**

```cpp
// Declare a multiset of integers
    multiset<int> ms;

    // Inserting elements into the multiset
    ms.insert(1);   // Multiset: {1}
    ms.insert(1);   // Multiset: {1, 1}
    ms.insert(1);   // Multiset: {1, 1, 1}

    // Erasing all occurrences of a specific value
    ms.erase(1);    // Erase all occurrences of value 1 from the multiset

    // Counting occurrences of a specific value
    int cnt = ms.count(1); // Count occurrences of value 1 in the multiset (returns 0)

    // Erasing a single occurrence of a specific value
    ms.erase(ms.find(1)); // Erase a single occurrence of value 1 from the multiset

    // Erasing a range of occurrences based on iterators
    auto start = ms.find(1);          // Iterator pointing to the first occurrence of value 1
    auto end = ms.find(1) + 2;        // Iterator pointing to the position after the second occurrence of value 1
    ms.erase(start, end);             // Erase elements in the range [start, end), excluding end

```
