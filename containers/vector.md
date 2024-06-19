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
```cpp
//iterator
    vector<int>::iterator it =v.begin(); //v.begin points to the memory
    it++;
    cout<< *(it)<<" "; //using * to access value of the memory
    
    //different types of iterators
    vector<int>::iterator it =v.end(); //points to the memory location right after the last element
    vector<int>::iterator it =v.rend(); //reverse it then points to end
    vector<int>::iterator it=v.rbegin(); //reverse it then points to begin
    cout<<v.back(); //prints the last element
```

```cpp
//Traversing vector(using iterator):
for(vector<int>::iterator it= v.begin(); it!=v.end(); it++) {
        cout<< *it<<" ";
    }
    for(auto it = v.begin(); it!=v.end();it++){
        cout<<*it<< " ";
    }
    for(auto it:v){
        cout<<it<<" ";
    }
```
```cpp
//Erase function in vector
v.erase(v.begin()+1); //giving the address to delete {1,3,4,5}
v.erase(v.begin()+1,v.begin()+3); // {1,5}
```
```cpp
//insert function
vector<int> v(2,100); //{100,100}
v.insert(v.begin(),300); //{300,100,100}
v.insert(v.begin()+1,2,10); //{300,10,10,100,100}
```
```cpp
//other useful functions:
    cout<<v.size(); //print number of element in vector
    v.pop_back(); //{10,20}->{10}
    v1.swap(v2); //swap both vectors
    v.clear(); // erase the entire vector
    v.empty(); // tell vector empty of not
```
