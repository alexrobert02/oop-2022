# LAB-4 (CLASSES)

Write a class in C++ that has the following definition:
```
class Sort
{
    // add data members
public:
    // add constuctors
    void InsertSort(bool ascendent=false);
    void QuickSort(bool ascendent=false);
    void BubbleSort(bool ascendent=false);
    void Print();
    int GetElementsCount();
    int GetElementFromIndex(int index);
}
```
Organize the code in the following way:
* a header file called **Sort.h**
* a .cpp file called **Sort.cpp** that contains the source code for class **Sort**
* a main file called **main.cpp** that contains the main function and has an example on how to use **Sort**. The example must include using all methods from the class.
* add several constructors that will allow the following:
  1. create the list that needs to be sorted out of random values within a specific interval (min, max). The constructor will receive 3 parameters (the number of elements in the list, minimum value, maximum value).
  2. create the list that needs to be sorted from an initialization list
  3. create the list that needs to be sorted from an existing vector (the constructor will have two parameters - one being the vector, the other one being the number of elements from the vector)
  4. create the list that needs to be sorted using variadic parameters (use va_args for this)
  5. create the list that needs to be sorted from a string (e.g. "10,40,100,5,70" -> each number is separated from the rest of the number with a comma). It is assumed that the string is correctly written (no space, only numerical characters and commas)


OBS: By "list" in this context we refer to a vector or any form of container that stores elements (it could be a double-linked-list, a heap vector or an array).