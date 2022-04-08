## Sort array
```cpp
sort(g.begin(), g.end());
```
    
## Customized sort
```cpp
sort(people.begin(), people.end(), [](const vector<int> &a, const vector<int> &b) {
            if(a[0] == b[0])
                return a[1] < b[1];
                return a[0] > b[0];
            });
```
    
## Sum array
```cpp
std::accumulate(num.begin(), num.end(), 0);
```
    
## Dictionary
```cpp
std::unordered_map<int, int> seen; //建立dict
seen.find(nums[i]) != seen.end() //没有这个key
seen.insert({target-nums[i], i}) //加入元素
seen[nums[i]] //拿到key对应的元素
```
    
## Loop string/array
```cpp
for (char const &c: s) {
    std::cout << c << std::endl;
}
for(auto item:array){
    std::cout << item << std::endl;
}
```
    
## Initialize 2D array
```cpp
vector<vector<int>> result(people.size(),vector<int>(2,-1));
```

## Pointer & const
```cpp
int x;
int * p1 = &x;//指针可以被修改，值也可以被修改
const int * p2 = &x;//指针可以被修改，值不可以被修改（const int）
int * const p3 = &x;//指针不可以被修改（*const），值可以被修改
const int * const p4 = &x;//指针不可以被修改，值也不可以被修改
```
    
## Set
```cpp
set<int> s;
s.insert(c - i*i);
if (s.count(i*i))
```
    
## Array tricK
```cpp
array.empty() 
return vector<int>{a,b};
```
    
## Max/Min array
```cpp
maximum = *max_element(elements.begin(), elements.end());
maximum_index = max_element(elements.begin(), elements.end()) - elements.begin();
```