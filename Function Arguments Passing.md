
## How many ways to pass arguments into a function?

**1. Passing values**

Copy the value from the **actual arguments** to the **formal parameters** of the function.

**2. Passing pointers**

Copy the value of **pointer variable (as an actual arguments)** to the **formal parameters** of the function so that they get the same memory location (the same data storage unit).

**3. Passing reference**

Pass the address of the **actual arguments** to the **formal parameters** so they are synonym and pointing to the same storage data unit.

**4. Globle variable**

No need to be the exactly globle variables, the variables just need to be inside the scope of the working function, e.g. two different member functions can share one member variable, or use static keyword to define, or use *namespace* to limit it, so in these kinds of cases, the variables are kinda "globle".
