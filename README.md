# 2110211
intro data struct chula engineer 2110211 (C++)

## std::vector
```cpp
#include <vector>
std::vector<int> vec = {1, 2};
vec.push_back(3); // vec = [1, 2, 3]
vec.push_back(4); // vec = [1, 2, 3, 4]
```

## for loop
```cpp
for (uint i = 0; i != vec.size(); ++i) { // c++98 indice
  int val = vec[i];
}

std::vector<int>::iterator it = vec.begin(); 
for (; it != vec.end(); ++it) { // c++98 iterator
  int val = *it;
}

for (uint i = 0; i != vec.size(); ++i) { // c++11 range-based for loop
  int val = vec[i];
}

```

## std::pair
```cpp
#include <utility>
std::pair<int, int> pi1(5, 13);
auto pi2 = pi1;
// pi1.first = 5
// pi1.second = 13
// pi2.first = 5
// pi2.second = 13

pi1.second = 999;
// pi1.first = 5
// pi1.second = 999
// pi2.first = 5
// pi2.second = 13
```
