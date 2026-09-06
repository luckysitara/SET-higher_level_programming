# SET-higher_level_programming



SE 300: High Level Programming II Average: 0.0%
Welcome to Week 1
Introduction to JavaScript and Your Development Environment
Variables, Constants, and Data Types
Control Flow and Loops
Functions and Error Handling
Working with Arrays and Objects
W1 | GRADED | 10.0% | JavaScript - Warm up Part 1
W1 | GRADED | 10.0% | JavaScript - Warm up Part 1

    Weight: 100
    Project will start Aug 30, 2026 5:00 PM, must end by Sep 8, 2026 4:59 PM


Copyright - Plagiarism

    You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
    You will not be able to meet the objectives of this or any following project by copying and pasting someone else's work.
    You are not allowed to publish any content of this project.
    Any form of plagiarism is strictly forbidden and will result in removal from the program.

Requirements
General

    Allowed editors: vi, vim, emacs
    All your files will be interpreted on Ubuntu 20.04 LTS using node (version 14.x)
    All your files should end with a new line
    The first line of all your files should be exactly #!/usr/bin/node
    A README.md file, at the root of the folder of the project, is mandatory
    Your code should be semistandard compliant (version 16.x.x). Rules of Standard + semicolons on top. Also as reference: AirBnB style
    All your files must be executable
    The length of your files will be tested using wc

More Info
Install Node 14

$ curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
$ sudo apt-get install -y nodejs

Install semi-standard



Documentation

$ sudo npm install semistandard --global


Tasks
0. First constant, first print
mandatory

Write a script that prints "JavaScript is amazing":

    You must create a constant variable called myVar with the value "JavaScript is amazing"
    You must use console.log(...) to print all output
    You are not allowed to use var

guillaume@ubuntu:~/0x12$ ./0-javascript_is_amazing.js 
JavaScript is amazing
guillaume@ubuntu:~/0x12$ 
guillaume@ubuntu:~/0x12$ semistandard ./0-javascript_is_amazing.js 
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 0-javascript_is_amazing.js

1. 3 languages
mandatory

Write a script that prints 3 lines:

    The first line: "C is fun"
    The second line: "Python is cool"
    The third line: "JavaScript is amazing"
    You must use console.log(...) to print all output
    You are not allowed to use var

guillaume@ubuntu:~/0x12$ ./1-multi_languages.js 
C is fun
Python is cool
JavaScript is amazing
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 1-multi_languages.js

2. Arguments
mandatory

Write a script that prints a message depending of the number of arguments passed:

    If no arguments are passed to the script, print "No argument"
    If only one argument is passed to the script, print "Argument found"
    Otherwise, print "Arguments found"
    You must use console.log(...) to print all output
    You are not allowed to use var

Reference: process.argv

guillaume@ubuntu:~/0x12$ ./2-arguments.js 
No argument
guillaume@ubuntu:~/0x12$ ./2-arguments.js Best
Argument found
guillaume@ubuntu:~/0x12$ ./2-arguments.js Best School
Arguments found
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 2-arguments.js

3. Value of my argument
mandatory

Write a script that prints the first argument passed to it:

    If no arguments are passed to the script, print "No argument"
    You must use console.log(...) to print all output
    You are not allowed to use var
    You are not allowed to use length

guillaume@ubuntu:~/0x12$ ./3-value_argument.js 
No argument
guillaume@ubuntu:~/0x12$ ./3-value_argument.js School
School
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 3-value_argument.js

4. Create a sentence
mandatory

Write a script that prints two arguments passed to it, in the following format:

<first argument> is <second argument>

    You must use console.log(...) to print all output
    You are not allowed to use var

guillaume@ubuntu:~/0x12$ ./4-concat.js c cool
c is cool
guillaume@ubuntu:~/0x12$ ./4-concat.js c 
c is undefined
guillaume@ubuntu:~/0x12$ ./4-concat.js
undefined is undefined
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 4-concat.js

5. An Integer
mandatory

Write a script that prints My number: <first argument converted in integer> if the first argument can be converted to an integer:

    If the argument can't be converted to an integer, print "Not a number"
    You must use console.log(...) to print all output
    You are not allowed to use var
    You are not allowed to use try/catch

guillaume@ubuntu:~/0x12$ ./5-to_integer.js 
Not a number
guillaume@ubuntu:~/0x12$ ./5-to_integer.js 89
My number: 89
guillaume@ubuntu:~/0x12$ ./5-to_integer.js "89"
My number: 89
guillaume@ubuntu:~/0x12$ ./5-to_integer.js 89.89
My number: 89
guillaume@ubuntu:~/0x12$ ./5-to_integer.js School
Not a number
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 5-to_integer.js

6. Loop to languages
mandatory

Write a script that prints 3 lines: (like 1-multi_languages.js) but by using an array of string and a loop

    The first line: "C is fun"
    The second line: "Python is cool"
    The third line: "JavaScript is amazing"
    You must use console.log(...) to print all output
    You are not allowed to use var
    You are not allowed to use any if/else statement
    You can use only one console.log
    You must use a loop (while, for, etc.)

guillaume@ubuntu:~/0x12$ ./6-multi_languages_loop.js 
C is fun
Python is cool
JavaScript is amazing
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 6-multi_languages_loop.js

7. I love C
mandatory

Write a script that prints x times "C is fun"

    Where x is the first argument of the script
    If the first argument can't be converted to an integer, print "Missing number of occurrences"
    If the first argument is a negative number, the loop doesn't execute and nothing is printed
    You must use console.log(...) to print all output
    You are not allowed to use var
    You can use only two console.log
    You must use a loop (while, for, etc.)

guillaume@ubuntu:~/0x12$ ./7-multi_c.js 2
C is fun
C is fun
guillaume@ubuntu:~/0x12$ ./7-multi_c.js 5
C is fun
C is fun
C is fun
C is fun
C is fun
guillaume@ubuntu:~/0x12$ ./7-multi_c.js 
Missing number of occurrences
guillaume@ubuntu:~/0x12$ ./7-multi_c.js -3
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 7-multi_c.js

8. Square
mandatory

Write a script that prints a square

    The first argument is the size of the square
    If the first argument can't be converted to an integer, print "Missing size"
    You must use the character X to print the square
    You must use console.log(...) to print all output
    You are not allowed to use var
    You must use a loop (while, for, etc.)

guillaume@ubuntu:~/0x12$ ./8-square.js
Missing size
guillaume@ubuntu:~/0x12$ ./8-square.js School
Missing size
guillaume@ubuntu:~/0x12$ ./8-square.js 2
XX
XX
guillaume@ubuntu:~/0x12$ ./8-square.js 6
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
XXXXXX
guillaume@ubuntu:~/0x12$ ./8-square.js -3
guillaume@ubuntu:~/0x12$ 


Repo:

    GitHub repository: SET-higher_level_programming
    Directory: 0x12-javascript-warm_up
    File: 8-square.js

Copyright © 2026 SET, All rights reserved.
