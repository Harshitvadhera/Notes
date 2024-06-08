Previous <- [[Array Foundations]]

```cpp
int main() {

	int arr[5];
	int size = 5;
	solve(arr,size);

}
void solve (int arr[], int size){
	cout >> arr >> endl; // This will output first element
} 
```

---
```cpp
int main(){
	int value = 5;
	int &reference = value;
	
	//***
	int &newReference = 6; 
	//This is invalid as a reference can't store a value
	//***
	
	cout << value << reference << endl; 
	/** This will output 5 5 as reference variable 
		is also pointing to value variable only and is just a 
		reference.
	**/
	
}
```

---
**Call By Value**

In call by value a new variable will be made and increment will happen over that variable and not the actual variable so the actual variable value will not get incremented.

```cpp
int main(){
	int value = 5;
	callIncrementWithoutReference(value);
	/** This will not increment the value 
	as we need to assign the result to value
	**/
}
void callIncrementWithoutReference(int value){
	value++;
}
```

---
**Call By Reference**

In call by reference a new variable will not pass and actually the reference of the variable will be passed so the operation will not be performed onto a new locally scoped variable but actually the original variable.

```cpp
int main(){
	int value = 5;
	callIncrementWithReference(value);
	//This will increment the value even if we are not returning
}

void callIncrementWithReference(int &reference){
	reference++;
}
```

---
Next 