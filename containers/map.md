stores everything in respect of keys and values **{keys, value}**

key and values can be anything like int, strings, char

Map store **Unique keys in sorted order**

works for **log(n);**

```cpp
//traversing on mp
    for(auto it: mp){
        cout<< it.first <<"-->" << it.second<< endl;
    }

// Declare a map with integer keys and integer values
    map<int, int> mp;

    // Declare a map with integer keys and pair of integers as values
    map<int, pair<int, int>> mpp;

    // Declare a map with pair of integers as keys and integer values
    map<pair<int, int>, int> mppi;

    // Inserting elements into the map 'mp'
    mp[1] = 2;                  // Insert key-value pair {1, 2} into 'mp'
    mp.emplace(3, 1);           // Insert key-value pair {3, 1} into 'mp' using emplace
    mp.insert({2, 4});          // Insert key-value pair {2, 4} into 'mp' using insert
    mpi[{2, 3}] = 10;            // Insert key-value pair {{2, 3}, 10} into 'mpi'

    // Inserting elements into the map 'mpp'
    mpi[{2, 3}] = 10;           // Insert key-value pair {{2, 3}, 10} into 'mpi'

    // Iterating through map 'mpp' and printing key-value pairs
    for (auto it : mpp) {
        cout << it.first.first << ", " << it.first.second << ": " << it.second << endl;
    }

    // Accessing elements using non-existent keys
    cout << mpp[1];             // Accessing 'mpp' with key 1 (returns default value, which is 0)
    cout << mpp[5];             // Accessing 'mpp' with key 5 (returns default value, which is 0)

    // Finding and accessing elements using iterators
    auto it = mpp.find(3);      // Find element in 'mpp' with key 3
    if (it != mpp.end()) {
        cout << it->second;     // Output the value associated with key 3 (if found)
    }

    auto it_not_found = mpp.find(5);  // Find element in 'mpp' with key 5

    // Finding lower and upper bounds using keys
    auto lower_bound_it = mpp.lower_bound(2);  // Iterator to the first element with key not less than 2
    auto upper_bound_it = mpp.upper_bound(3);  // Iterator to the first element with key greater than 3

```
