
# Python Scope:

The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code. The scope of a name or variable depends on the place in your code where you create that variable. The Python scope concept is generally presented using a rule known as the LEGB rule.

A variable is only available from inside the region it is created. This is called scope.


Local Scope:
A variable created inside a function belongs to the local scope of that function, and can only be used inside that function.

Example:

```
def myfunc():
  x = 300
  print(x)

myfunc()
```

Global Scope:
A variable created in the main body of the Python code is a global variable and belongs to the global scope.

Global variables are available from within any scope, global and local.

Example:
```
x = 300

def myfunc():
  print(x)

myfunc()

print(x)
```
## Global Keyword:

If you need to create a global variable, but are stuck in the local scope, you can use the global keyword.

The global keyword makes the variable global.

Example:
```
def myfunc():
  global x
  x = 300

myfunc()

print(x)
```

## nonlocal keyword:


The nonlocal keyword is used to work with variables inside nested functions, where the variable should not belong to the inner function.

Use the keyword nonlocal to declare that the variable is not local.

example:
```
def myfunc1():
  x = "John"
  def myfunc2():
    x = "hello"
  myfunc2()
  return x

print(myfunc1())
```




#####  by OBADA ALHAWJREH.*

My name is obada jaber, I’m 27 years old, I studied Mechanical engineering and i graduated from al balqa applied university, i am now a software student. [OBADA ALHAWJREH](https://github.com/Obada-gh).

##### *Support or Contact:*

Having trouble with Pages? Check out our : [email](obada7jaber7@gmail.com) or phone number : 0781912474 or [contact support for gethub](https://support.github.com/contact) and we’ll help you sort it out. &#x1F691; &#x1F691; &#x1F691;
