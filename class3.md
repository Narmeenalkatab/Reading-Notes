# <span style="color:red">File Input/Output and Exceptions</span>



## <span style="color:blue">File Input/Output</span>

•	File:
          a file is a contiguous set of bytes used to store data.

            contiguous set of bytes:

         e.g.: ('Hello, world!\n')
              48 65 6c 6c 6f 2c 20 77 6f 72 6c 64 21 0a

           Each pair of hexadecimal digits represents a single byte of data.
<span style="color:orange">
             1- (48) represents the ASCII code for the letter "H".
             </span>

<span style="color:orange">
              2- (65) represents the ASCII code for the letter "e", and so on.
             </span>





•<span style="color:orange">**File path**:</span>
         file path is a string that represents the location of a file on a computer's file system
           and is made up of the folder path, file name, and extension.



•	<span style="color:orange">**Line Endings**:</span>
related to how new lines or line breaks are represented in a file.

Ex:

<span style="color:green">text on a Windows system:</span>

This is the first line\r\n

This is the second line\r\n

<span style="color:green">Unix system:</span>

with open("example.txt", "r") as file:

content = file.read()

print(content)



•	<span style="color:orange">**Opening and Closing a File in Python**:</span>


To work with files in Python, we first need to open them. With a built-in function called <span style="color:red">open()</span>.

Ex:

file_object = open(file_path, mode)

file_path: the path to the file we want to open.

mode is how you want to open the file. The mode can be one of the following:

<span style="color:red">'r': </span> Open for reading (default)

<span style="color:red">'w':</span>   Open for writing, truncating (overwriting) the file first

<span style="color:red">'rb' or 'wb'</span>: Open in binary mode (read/write using byte data)








## <span style="color:blue"> **Exceptions** </span>


Errors types:

1-**syntax error**: it stopes the program (the error message will appears in error place).

2-**exceptions**:

is an event that occurs during the execution of a program , we use it to handle errors.

We handle it using <span style="color:green">(try-expect block)</span> also we can use <span style="color:green">(finally-block)</span>.

<span style="color:orange">(try-expect block)</span>:

try : code that may raise an exception

expect :code that handles the exception

<span style="color:orange">(finally-block)</span>:

finally: code that is executed all always.



3-**logical errors**: it is the worst error types because the program will not stop but it will not give the right output. It calls bugs ,hackers do hacking throw these bugs .To solve this errors we need to read the code more than one time and make it logical.






# <span style="color:green">**Reading Questions**</span>
1.	What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

<span style="color:green">The 'with' statement is used in Python  to open file (with open('filename', 'mode'))</span>




2.	Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

<span style="color:green">The **'read()'** method reads the entire contents of the file and returns them as a string. The **'readline()'** method reads one line at a time from the file and returns it as a string. The key difference between the two methods is that **'read()'** reads the entire contents of the file at once, while **'readline()'** reads one line at a time.</span>






3.	Briefly describe the concept of exception handling in Python.how the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.


<span style="color:green">
<span style="color:orange">(try-expect block)</span>:

try : code that may raise an exception

expect :code that handles the exception

<span style="color:orange">(finally-block)</span>:

finally: code that is executed all always.
</span>





## <span style="color:red">Things I want to know more about</span>

I want to have deep understanding .
