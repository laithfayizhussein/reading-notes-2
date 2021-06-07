# Reading and Writing Files in Python
- What Is a File? Before we can go into how to work with files in Python, it’s important to understand what exactly a file is and how modern operating systems handle some of their aspects.

- At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

- Files on most modern file systems are composed of three main parts:

- Header: metadata about the contents of the file (file name, size, type, and so on) Data: contents of the file as written by the creator or editor End of file (EOF): special character that indicates the end of the file
-
## Line Endings
- Windows uses the CR+LF characters to indicate a new line, while Unix and the newer Mac versions use just the LF character.

- unix :
```
 German Shepherd\r \n

Opening and Closing a File in Python let`s explain it by code example :

    open

file = open('dog_breeds.txt') do any coding between finally: file.close()

or
with open('dog_breeds.txt') as reader: # Further file processing goes here
```

- The with statement automatically takes care of closing the file once it leaves the with block,

    - Warning: You should always make sure that an open file is properly closed.

- what we want from file , r-read ,wirte ... etc we can add as argument
- with open('dog_breeds.txt', 'r') as reader: # Further file processing goes here

## Character Encodings
- Another common problem that you may face is the encoding of the byte data. An encoding is a translation from byte data to human readable characters. This is typically done by assigning a numerical value to represent a character. The two most common encodings are the ASCII and UNICODE Formats. ASCII can only store 128 characters, while Unicode can contain up to 1,114,112 characters.

- ASCII is actually a subset of Unicode (UTF-8), meaning that ASCII and Unicode share the same numerical to character values. It’s important to note that parsing a file with the incorrect character encoding can lead to failures or misrepresentation of the character. For example, if a file was created using the UTF-8 encoding, and you try to parse it using the ASCII encoding, if there is a character that is outside of those 128 values, then an error will be thrown.

# Python Exceptions
- A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception. In this article, you will see what an exception is and how it differs from a syntax error. After that, you will learn about raising exceptions and making assertions. Then, you’ll finish with a demonstration of the try and except block.
- Syntax errors occur when the parser detects an incorrect statement. Observe the following example:

```
 print( 0 / 0 ))
  File "<stdin>", line 1
    print( 0 / 0 ))
```
SyntaxError: invalid syntax

The arrow indicates where the parser ran into the syntax error. In this example, there was one bracket too many. Remove it and run your code again:

```
print( 0 / 0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  ``` 
  
ZeroDivisionError: integer division or modulo by zero

This time, you ran into an exception error. This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.

Instead of showing the message exception error, Python details what type of exception error was encountered. In this case, it was a ZeroDivisionError. Python comes with various built-in exceptions as well as the possibility to create self-defined exceptions.