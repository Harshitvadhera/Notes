>[!important] limits.h

This header file has `INT_MIN` & `INT_MAX`.

---
**INT_MIN**

```cpp
#include<limits.h>
using namespace std;
int main() {
 cout >> INT_MIN >> endl; 
 /** This will output -2147483648
	 which is -2^31 the least possible value of integer
 **/
}
```

---
**INT_MAX**

```cpp
#include<limits.h>
using namespace std;
int main() {
 cout >> INT_MAX >> endl; 
 /** This will output 2147483648
	 which is 2^31 the max possible value of integer
 **/
}
```
