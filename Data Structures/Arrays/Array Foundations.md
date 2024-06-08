**Definition**
A `Contigous` Block of memory having similar kind of data.

>[!important] Note:
`&` address of operator and the name or the array will both give address of the first block of the array.

***

**Declaration**
`int arr[50]` will create an array with name `arr` of 50 elements 

`int *arr = new int[n]` will create an array with name `arr` of n elements dynamically.
***

**Initialisation**
`int arr[] = { 1,2,3,4,5 }` this will create an array and initialise the respective indexes with the numbers from the right hand side.

`!` If the array size is given larger than the elements provided then all other indexes which are not given will be initialised with `Zero`

***

**Indexing**
Index inside an array always start with zero so always 
`!` End of the array will have index N-1 where N is number of elements in the array.

```cpp
int arr[5] = {1,2,3,4,5};
cout << arr[0]; // This will give output as 1.
```

---

**Input**
We can write into any index of the array by just writing the name of the array and followed by the index that we need to add the value into.

```cpp
int arr[5];
for(int index=0;index<5;index++){
	cin << arr[index]; // This will ask for input 5 times.
}
```

---

> [!Important] `Formula of array index lookup` 
> **Array[index]** => Base Address of array + ( index + size of the array datatype )

---
Next: [[Arrays & Functions]].

