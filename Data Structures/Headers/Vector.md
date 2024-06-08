**Definition**
It is a header file which is available to us in the Standard Template Library ( STL ) which is a dynamic array that can grow or shrink in size, making it a versatile and efficient data structure for storing and manipulating sequences of elements.

**Declaration**
`vector<dataType> variableName`;

**Initialisation**
`vector<int> arr(5,0);` 
This will create a vector of 5 elements with all initialised to zeroes.

`vector<int>arr{1, 2, 3, 4, 5}` This will create those 5 elements but this is a new way so might not work in some of the compilers as it came after C++11.

`vector<int> arr = {1, 2, 3, 4, 5}` This will work in all compilers.

>[!important] Capacity Vs Size 
> `Capacity` is the current amount of values the current vector can hold when the current size limit will be reached it will double the capacity so that more values can be added automatically.
> 
> `Size` is the current amount of values the current vector is holding.  

**Features**
`vector.push_back(item)` will push an item in the vector.

`vector.size()` will return the current size of the vector. It follows 1 based indexing so whenever want to get the size need to use it as `vector[vector.size()-1]`

`vector.front()` will return the front element of the vector.

`vector.back()` will return the last element of the vector.

`vector.at(index)` will return the value at that particular index.

`vector.clear()` will clear all of the vector and hence size will become zero 
but capacity will still be there only the size will be cleared.

**For Each Loop**
```cpp
for(auto it: v) {
	cout << v[it];
}
```
