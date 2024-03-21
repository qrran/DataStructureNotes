### 1. Special case:

- any # less than the first number(info) is considered special case, b/c need to modify first
  ```cpp
  item<first>info
  ```

### 2. Empty

- if empty: no any loop/local pointer

```cpp
//need to have a pointer that walks
// can be solved by using 2 pointers that walk different pace
p->next = q;
trail->next = p;

```

### 3. Between 2 nodes

### 4. At the end

_In any case, we can create a node once we found the place_

- crash: a particular case didn't happen

  **code need to work with all cases**

1. ```cpp
   node<T> * p = new ndoe<T>;
   p->info = item;
   ```

### Copy Algorithm

### Insert Algorithm

```cpp
void LList<T> :: insertItem(T item)
{
  length++;
// temp is a local pointer, only used to walk or create nodes
// all local values are gone at the end of the program
// only first exists by the end
  node<T> *temp = new node<T>;
  temp->info = item;

  if(first == NULL || item < first->info)
  {
    temp-next = first; // temp->next means the space nest to the temp variable
    fist = temp;
  }
  else
  {
    node<T> *trail = NULL;
    node<T> *q = first;

    while(q != NULL && q->info < item)
    {
      trail = q;
      q = q->next;
    }
    temp->next = q;
    trail-> next = temp;
  }
}
```

### Delete Algorithm

```cpp
void LList<T> :: deleteItem(T item)
{
  // info, trail
  // check if the item is in the list
  // special case:

  // S.C. 1. If empty print error

  // 2. modify the first item in the list, if item equal to first info
  // local pointer equal to the first, first equals to the next, then delte first
  // if item = first->info

  // 3. delete the item that is not in the list

  // 4. delete the item at the end

  // in order to delete a pointer you need to add a node (pointing to the pointer)
  // do something to first->next, need to have a node that points to the first

  // trail pointer = NULL

  // as long as p is not equal to NULL
  // if equal, then delete

  //////////////////////////////////////////////
  // 1, set p = p->next
  // 2. compare p with node, p > item, then set trail into
  // 3. trail->next = p->next, delete p
  // 4. delete the equal item
  // end loop if(p == NULL || p > item) keep walking; else(delete_)

  // do something in the beginning and do something in the end
}


```
