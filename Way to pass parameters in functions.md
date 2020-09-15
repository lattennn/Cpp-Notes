
## Definition of Pointers and References

- Pointers: a variable that saves a memory address that points to a data storage unit.

- Reference: a synonym of a varible, they are the same thing cause they point to the same data storage unit.

```c++
int a=10;
int *p = &a; // p is a pointer, p's value is the memory address of the contents of variable a

int a=10;
int &b=a; //b is the reference, b = a actually because they have the same memory address
```

## Difference of Pointers and References

- Pointer can be a **const** value

  + it points to a fixed address -> while the contents in that address can be changes, this **Const Pointer's value** cannot be changed.

- Reference **NO NEED** to be a **const** reference

  + because it's always **const**, once set it as an object's reference, cannot reset it as another object's reference.

- **Pointers** can be chained while **Reference** cannot

```c++
int *p;
int **p = &p;

int a;
int &b=a;
int &&c=b; //NO

```

- **Pointers'** values can be NULL (pointing to nowhere) while **Reference** should be initialized when it's defined

- **Pointers**(not const) can be changed later (point to another location) while **Reference** cannot be changed after it's set initially

- sizeof() **a Pointer** is the size of the pointer variable itself but sizeof() **a Reference** is the size of the object/variable it points to

- **Pointers++** is different with **Reference++**

## How many ways to pass parameters into a function?

1. Passing values

Copy the value from the **actual arguments** to the **formal parameters** of the function.

2. Passing pointers

Copy the value of **pointer variable (as an actual arguments)** to the **formal parameters** of the function so that they get the same memory location (the same data storage unit).

3. Passing 
