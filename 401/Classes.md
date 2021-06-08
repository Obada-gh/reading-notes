
## Classes and Objects:

Python is an object oriented programming language.

Almost everything in Python is an object, with its properties and methods.

A Class is like an object constructor, or a "blueprint" for creating objects.
```
Create a class named MyClass, with a property named x:
class MyClass:
  x = 5

Now we can use the class named MyClass to create objects:

p1 = MyClass()
print(p1.x)


```
The `__init__()` Function
The examples above are classes and objects in their simplest form, and are not really useful in real life applications.

To understand the meaning of classes we have to understand the built-in `__init__()` function.

All classes have a function called `__init__()`, which is always executed when the class is being initiated.

Use the `__init__()` function to assign values to object properties, or other operations that are necessary to do when the object is being created:

```
Create a class named Person, use the `__init__()` function to assign values for name and age:

class Person:
  def `__init__`(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)
```

[object_methods](https://www.w3schools.com/python/gloss_python_object_methods.asp)

## Thinking Recursively in Python:
Along the way on your programming journey, there are a few milestones that you need to conquer to advance ahead. For example, getting comfortable with classes, understanding pointers, master the art of functionalizing your code, and so on. One of the trickest programming concepts to learn for newcomers and master for those who have been programming for a while is recursion.

Steps to train your mind to think recursively:
1. Use the iterable-approach first.
2. Extract the parameters of your function.
3. Deduct minimal problem instance.
4. Add the solution to the minimal problem instance.
5. Expand your function.

### Naive Recursion is Naive
Thus, we avoid recomputation by explicitly checking for the value before trying to compute it.




## Python Testing with pytest: Fixtures and Coverage:

What Does Fixtures Mean?
Fixtures, in the context of insurance, are movable or personal property attached to an immovable property that they become a part of the immovable or real property and are covered under a real estate insurance policy.

Insuranceopedia Explains Fixtures
Fixtures are said to form part of the immovable when they are attached or affixed permanently, such as when they are embedded, rooted, or permanently attached with cement, glue, nails, screws, bolts, or plaster. There are four types of fixtures, namely:

Agricultural fixtures, or those attached for the purpose of farming;
Domestic fixtures, or those attached to a home in order to make it more livable;
Ornamental fixtures, or those attached to a property in order to make it more attractive; and
Trade fixtures, or those necessary in the conduct of business in the real property.
To determine whether a personal property is a fixture or not, the following shall be considered:

Method of attachment;
Adaptability of use;
Intent of the buyer and the seller in a contract of sale;
Agreement of the parties; and
Relationship of the parties.

examples:
```
>>> while True print('Hello world')
  File "<stdin>", line 1
    while True print('Hello world')
                   ^
SyntaxError: invalid syntax
```
Exceptions:

```
>>> 10 * (1/0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: division by zero
>>> 4 + spam*3
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'spam' is not defined
>>> '2' + 2
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: Can't convert 'int' object to str implicitly
```

shell:
```
$ pytest
================== test session starts =============================
platform darwin -- Python 3.7.3, pytest-5.3.0, py-1.8.0, pluggy-0.13.0
rootdir: /.../effective-python-testing-with-pytest
collected 2 items

test_with_pytest.py .F                                          [100%]

======================== FAILURES ==================================
___________________ test_always_fails ______________________________

    def test_always_fails():
>       assert False
E       assert False

test_with_pytest.py:5: AssertionError
============== 1 failed, 1 passed in 0.07s =========================
```

##### *writen by OBADA ALHAWJREH.*

My name is obada jaber, I’m 27 years old, I studied Mechanical engineering and i graduated from al balqa applied university, i am now a software student. [OBADA ALHAWJREH](https://github.com/Obada-gh).

##### *Support or Contact:*

Having trouble with Pages? Check out our : [email](obada7jaber7@gmail.com) or phone number : 0781912474 or [contact support for gethub](https://support.github.com/contact) and we’ll help you sort it out. &#x1F691; &#x1F691; &#x1F691;
