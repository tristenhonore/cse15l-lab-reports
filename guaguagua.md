# Lab Report 1 - Remote Access and FileSystem
this page shows the results of giving a terminal different commands with different circumstances. In these cases a directory named "Lecture1" exists with multiple directories and files within these directories. 
# Command cd (change directory):
## Example with no arguments: 
```
[user@sahara ~]$ cd
[user@sahara ~]$ []
```
With no arguments the cd command will set your terminal to not be inside of any directory.
This is because the cd command requires a directory to open, otherwise it defaults back to the beggining with no directory open.
This output is NOT an error.

## Example with a path to a directory as an argument:
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ []
```
With a directory as an argument the cd command will visibily change the field with the name of the directory you are now looking in. 
This change shows that you are now accessing the lecture1 directory. 
This output is NOT an error. 

## Example with a path to a file as an argument:
```
[user@sahara ~/lecture1]$ cd README
bash: cd: README: Not a directory
[user@sahara ~/lecture1]$ []
```
With a file as an argument the cd command will tell you that the file is not a directory. 
This is because the cd command only changes directories, it does not open files.
this output is NOT an error.
