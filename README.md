# Arrays

## What are arrays?

Arrays a kind of data structure that can store a fixed-size sequential collection of elements of the same type. An array is used to store a collection of data, but it is often more useful to think of an array as a collection of variables of the same type.

Instead of declaring individual variables, such as number0, number1, ..., and number99, you declare one array variable such as numbers and use numbers[0], numbers[1], and ..., numbers[99] to represent individual variables. A specific element in an array is accessed by an index.

All arrays consist of contiguous memory locations. The lowest address corresponds to the first element and the highest address to the last element.

![Screenshot 2023-04-10 at 9 03 47 PM](https://user-images.githubusercontent.com/91966167/230933934-5e1c8116-27a2-4c69-bb62-0e2457367f77.png)

## C Array Initialization

Initialization in C is the process to assign some initial value to the variable. When the array is declared or allocated memory, the elements of the array contain some garbage value. So, we need to initialize the array to some meaningful value. There are multiple ways in which we can initialize an array in C.

**1. Array Initialization with Declaration-**
In this method, we initialize the array along with its declaration. We use an initializer list to initialize multiple elements of the array. An initializer list is the list of values enclosed within braces { } separated b a comma.

```
data_type array_name [size] = {value1, value2, ... valueN};
```
c array initialization
 

**2. Array Initialization with Declaration without Size-**
If we initialize an array using an initializer list, we can skip declaring the size of the array as the compiler can automatically deduce the size of the array in these cases. The size of the array in these cases is equal to the number of elements present in the initializer list as the compiler can automatically deduce the size of the array.

```
data_type array_name[] = {1,2,3,4,5};
```
The size of the above arrays is 5 which is automatically deduced by the compiler.

![Screenshot 2023-04-10 at 9 13 34 PM](https://user-images.githubusercontent.com/91966167/230937502-8be17ae6-ec4b-4631-9441-7a7049b40b31.png)


**3. Array Initialization after Declaration (Using Loops)-**
We initialize the array after the declaration by assigning the initial value to each element individually. We can use for loop, while loop, or do-while loop to assign the value to each element of the array.

```
for (int i = 0; i < N; i++) {
    array_name[i] = valuei;
}
```
**Output-**

![Screenshot 2023-04-10 at 9 05 17 PM](https://user-images.githubusercontent.com/91966167/230935628-d4a3027b-bf52-4b52-a3f2-b366b4c1ac88.png)
