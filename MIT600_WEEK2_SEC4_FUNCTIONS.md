# Funtions
## Functions and Scope

- Function Characteristics:
  - Has a __name__
  - Has __parameters__ (0 or more)
  - Has a __docstring__ (Optional but recommended)
    - docstring tells a funtion what it does
  - Has a __body__
- Funtions are not run in a program until they are "__called__" or "__invoked__" in a program


```python
def is_even( i ):
    """
    Input: i, a postive int
    Returns True if i is even, otherwise False
    """
    print("hi")
    return i%2 == 0
    
is_even(3)
```

- `def` is the keyword It says it's about to define a function.
- `is_even` is the name of the function
- `( i )`  Parameters or arguments that are goign to be fed into the function.  0 or more.
- `"""` The stuff inside the triple double quotes is the docstring or specifications of the function.  Tells what the inputs and outputs are of the function.
  - Should definitly use this as wheny ou go to call the function python will give you a popup box with this information so that you can tell the specs of the function on the fly.

- The body of the function is the `print` and `return` lines.

- `is_even(3)`  is how you would call the function.  (invoke)

```python
def my_function(argument):
   """
   Docstring goes here. Explain what type argument(s) should have, and what your function
   is going to return.
   """
   < Code for your function (the body of the function) goes here >
```

### Variable Scope

- __Formal parameter__ gets bound to the value of __actual parameter__ when function is called.
- new __scope/frame/environment__ created when enter a function
- __scope__ is mapping of names to objects

#### ONE WARNING IF NO `return` STATEMENT
```python
def is_even( i ):
  """
  Input: i, a positive int
  Does not return anything
  """
  i%2 == 0
```
- Pytho returns the value __None, if no return given__
- represents teh absense of a value


### Keyword Arguments

You can call the inputs by name and if so you can call them in any order.

Also you can have default values for fucntion inputs just assign them at the time of definition.

### Specifications
-  A __contract__ between the implementer of a function and the clients who will use it
  - __Assumptions:__ conditions that must be met by clients of the funtion; typically contraints on values of parameters
  - __Gurantees:__ conditions that must be met by the function, providing it has been called in manner consistent with assumptions.

#### Use docstring!

- Not required but good programmers __ALWAYS__ do.
- docstring should have what the inputs should be and what the return should be,
- If purpose of the function is not clear from those two then explain in more detail








