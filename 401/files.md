
## What Is a File?:

a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.Files on most modern file systems are composed of three main parts:Header,Data,End of file (EOF)

File Paths:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
File Name: the actual name of the file
Extension: the end of the file path pre-pended with a period (.) used to indicate the file type.

```
/
│
├── path/
|   │
│   ├── to/
│   │   └── cats.gif
│   │
│   └── dog_breeds.txt
|
└── animals.csv

```
## Opening and Closing a File in Python:

```
file = open('dog_breeds.txt')
```

```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```
## read and write :

![charrters](https://www13.0zz0.com/2021/06/08/08/547656719.png)




![read](https://www2.0zz0.com/2021/06/08/08/913333863.png)


![write](https://www5.0zz0.com/2021/06/08/08/104099364.png)


there is a lot of types of files if you want more info:
[files](https://realpython.com/read-write-files-python/)



## Python Exceptions:

In Python, exceptions can be handled using a try statement. The critical operation which can raise an exception is placed inside the try clause. The code that handles the exceptions is written in the except clause. ... If no exception occurs, the except block is skipped and normal flow continues(for last value).

Until now error messages haven’t been more than mentioned, but if you have tried out the examples you have probably seen some. There are (at least) two distinguishable kinds of errors: syntax errors and exceptions.

Syntax Errors:
Syntax errors, also known as parsing errors, are perhaps the most common kind of complaint you get while you are still learning Python:
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

## Reading and Writing Files in Python:

When you’re working with Python, you don’t need to import a library in order to read and write to files. It’s handled natively in the language, albeit in a unique manner.

The first thing you’ll need to do is use the built-in python open file function to get a file object.

[gitfile](https://github.com/Obada-gh/reading-notes)

### find more:

link for the github file : [reading-and-writing-files-in-python](https://www.pythonforbeginners.com/files/reading-and-writing-files-in-python)

##### *writen by OBADA ALHAWJREH.*

My name is obada jaber, I’m 27 years old, I studied Mechanical engineering and i graduated from al balqa applied university, i am now a software student. [OBADA ALHAWJREH](https://github.com/Obada-gh).

##### *Support or Contact:*

Having trouble with Pages? Check out our : [email](obada7jaber7@gmail.com) or phone number : 0781912474 or [contact support for gethub](https://support.github.com/contact) and we’ll help you sort it out. &#x1F691; &#x1F691; &#x1F691;
