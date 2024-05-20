list similar to vector, it gives to front operations as well

insert function in vector is costly(in vector singly linked list are maintained)

list internal operation is doubly linked list (so push front is cheap)

```cpp
list<int> ls;

    ls.push_back(2);
    ls.emplace_back(4);

    ls.push_front(5);
    ls.emplace_front(1);
    
    //traversing 
    for (auto num : ls) {
        cout << num << " ";
    }
    cout << std::endl;

    //rest functions are same as vector
    //begin, end, rbegin, rend, clear, insert, size, swap
```