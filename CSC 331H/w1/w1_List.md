Overview: Pointers

1. List

2. Operation

3. File

```
#ifndef
#define
```

4. Template

5. Data type
   `const AList<T> & operator=`

- assign and return the result

6. Search

## Notice

`#include "AList.cpp"` the generic list in order to use it

### 2.1.2024

````cpp
template<class T>
struct node
{
   T info;
   node *next;
}```

## Vocab:
- hap

```cpp
node<T> *p = new node<T>
```

```
(*var).a = 20; //the same as
var->a = 20; //let the complier dereference the variable first then assign the value
```
````
