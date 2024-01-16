# Lab Report 1 - Remote Access and FileSystem
this page shows the results of giving a terminal different commands with different circumstances. In these cases a directory named "Lecture1" exists with multiple directories and files within these directories. 
# Command cd (change directory):
## Example with no arguments: 
```
[user@sahara ~]$ cd
[user@sahara ~]$ []
```
This command was run without any working directory.
With no arguments the cd command will set your terminal to not be inside of any directory.
This is because the cd command requires a directory to open, otherwise it defaults back to the beggining with no directory open.
This output is NOT an error.

## Example with a path to a directory as an argument:
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ []
```
this command was run without any working directory
With a directory (lecture1) as an argument the cd command will visibily change the field with the name of the directory you are now looking in. 
This change shows that you are now accessing the lecture1 directory. 
This output is NOT an error. 

## Example with a path to a file as an argument:
```
[user@sahara ~/lecture1]$ cd README
bash: cd: README: Not a directory
[user@sahara ~/lecture1]$ []
```
this command was run inside of the lecture1 directory.
With a file (README) as an argument the cd command will tell you that the file is not a directory. 
This is because the cd command only changes directories, it does not open files.
This output is NOT an error.
# Command ls (list):
## Example with no arguments:
```
[user@sahara ~]$ ls
lecture1
[user@sahara ~]$
```
this command was run without any working directory
With no arguments the ls command lists the current files and directories in the current directory.
Lecture1 is the output because the ls command lists the directories/files within the currently selected directory.
This output is NOT an error.
## Example with a path to a directory as an argument:
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages
[user@sahara ~]$
```
this command was run without any working directory
With a directory (lecture1) as the argument the output shows the 3 different files and directories in the lecture1 directory.
This output is a result of listing the contents of the selected directory.
This output is NOT an error.
## Example with a path to a file as an argument:
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ ls Hello.class
Hello.class
[user@sahara ~/lecture1]$ []
```
this command was run within the lecture1 directory.
With a file (Heelo.class) as the argument the output shows the name of the file. 
This is because the ls command has nothing to list within the file and therefore only repeats the file name.
This output is NOT an error.
# Command cat (concatenate)
## Example with no arguments:
```
[user@sahara ~]$ cat
[]
```
this command was run without any working directory
With no arguments the cat command makes the terminal no longer work. 
This is because the cat command does not have anything to do and cannot output anything. 
This output is an error as the cat command is typically supposed to write out the contents of a file but does not output anything. 
## Example with a path to a directory as an argument:
```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
[user@sahara ~]$ []
```
this command was run without any working directory
With a directory (lecture1) as the argument the output labels lecture1 as a directory.
This is because the cat command only writes out the contents of files not directories. 
This output is NOT an error.
## Example with a path to a file as an argument:
```
[user@sahara ~/lecture1/messages]$ cat en-us.txt 
Hello World!
[user@sahara ~/lecture1/messages]$
```
this command was run within the messages directory which is within the lecture1 directory.
With a file (en-us.txt) as the argument the output says "Hello World!".
This is because the cat command displays the contents of files. 
This output is NOT an error.
