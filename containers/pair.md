It is inside utility library.

Pairs are not mutable. This means that once a **`pair`** object is created, you cannot modify it.

```cpp
pair<int,int> p = {1,2};
    cout<<p.first<<" "<<p.second;

    pair<int,pair<int,int>> pr = {1,{2,3}}; //nested property of pair
    cout<<pr.first<<" "<<pr.second.second<<" "<<pr.second.first;

    pair<int,int> arr[] = {{1,2},{2,3},{5,1}};
    cout<<arr[1].second;
```