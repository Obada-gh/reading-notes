List comprehensions are used for creating new lists from other iterables.
As list comprehensions return lists, they consist of brackets containing the expression, which is executed for each element along with the for loop to iterate over each element.
This is the basic syntax:
```
new_list = [expression for_loop_one_or_more conditions]
```

For example, find the squares of a number using the for loop:

```
numbers = [1, 2, 3, 4]
squares = []

for n in numbers:
  squares.append(n**2)

print(squares)  # Output: [1, 4, 9, 16]
```

Finding squares using list comprehensions:

```
numbers = [1, 2, 3, 4]
squares = [n**2 for n in numbers]

print(squares)  # Output: [1, 4, 9, 16]
```

more:

```

list_a = [1, 2, 3]

square_cube_list = [ [a**2, a**3] for a in list_a]

print(square_cube_list) # Output: [[1, 1], [4, 8], [9, 27]]

```