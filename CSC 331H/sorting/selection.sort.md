## Sorting

1. Selection Sort

- work on unsorted part

```cpp
void selectionSort(int A[], int length)
{
    int smallest;
    for(int i = 0; i < length - 1; i++)
    {
        // find smallest element
        smallest = i;
        //check i element with the element next to i, so j = i + 1
        for(int j = i + 1; j < length; j++){
            if(A[j] < A[smalllest])
                smallest = j;
        }
        //no need to add the condition, if smallest is the element itself, it stays the same
        swap(A[smallest], A[i]);
    }
}
```

2. Insertion Sort

- work on the sorted part
- inserts the unsorted elements to the sorted
- **continue swap with the element before after true comparison**

```cpp
void insertionSort(int A[], int length)
{
    // int smaller;
    // for(int i = 1; i < length - 1; i++)
    // {
    //     smaller = A[i-1];
    //     //compare the element after with the element, if smaller, swap
    //     while(A[i] < A[i-1]){
    //         smaller = A[i]
    //         swap(A[smaller], A[i]);
    //     }
    //     //should have another loop to check with the element
    // }

    //above is an infinite loop, needs increment/decrement in the while loop
}
```
