
# Operator ::

## Scope Resolution Operator ::

- Global scope --> `::name`

- Class scope --> `class::name`

- namespace scope --> `namespace::name`

### For what

- Call the correct variables Explicitly!

  - call global variable or function **x** in the code -->`::x`

  - call the member function or member varible **x** of class **X** --> `X::x` 
  
  (when a function is declared but not specified yet in the class, **must** use **::** to define it outside of the class)
  
  - call the object **cout** in the standard library **std** --> std::cout (相当于 using namespace std; 后直接用cout)
  
