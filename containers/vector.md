```cpp
vector<int> v;
    v.push_back(1); //
    v.emplace_back(2); //emplace back is faster then push back

    vector<pair<int,int>> vec;
    v.push_back({1,2}); //here use curly brackets to push back pairs
    v.emplace_back(1,2); //no need for curly here, already assume pair

    vector<int> v1(5,100); // {100,100,100,100,100}

    vector<int> v2(5); //{0,0,0,0,0}

    vector<int> v3(5,20);
    vector<int> v4(v3);  // copy of v3(above vector)
```
