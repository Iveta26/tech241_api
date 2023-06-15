# Intro to Scripting

<br />

### What is scripting?
A scripting language or script language is a programming language that is used to manipulate, customize, and automate the facilities of an existing system. Scripting languages are usually interpreted at runtime rather than compiled.

<br />

### Why is it important in DevOps?

Shell scripting for DevOps enables automation of deployment, configuration management, CI/CD pipelines, monitoring, logging, and performance optimization tasks. Shell scripting languages, such as Bash, are used for automating tasks in DevOps workflows.

<br />

### Main libraries
    
- **sys** - system specific parameters and functions. This module provides access to some variables used or maintained by the interpreter and to functions that interact strongly with the interpreter
- **os** - miscellaneous operating system interfaces. This module provides a portable way of using operating system dependent functionality. If you just want to read or write a file see **open()**, if you want to manipulate paths, see the **os.path** module, and if you want to read all the lines in all the files on the command line see the **fileinput** module. For creating temporary files and directories see the **tempfile** module, and for high-level file and directory handling see the **shutil** module.
- **subprocess** - subprocess management. The subprocess module allows you to spawn new processes, connect to their input/output/error pipes, and obtain their return codes.
- **math** - mathematical functions. This module provides access to the mathematical functions. 
- **random** - generate pseudo-random numbers. This module implements pseudo-random number generators for various distributions.
- **datetime** - basic date and time types. The datetime module supplies classes for manipulating dates and times.
- **json** - JSON encoder and decoder. JSON (JavaScript Object Notation), is a lightweight data interchange format inspired by JavaScript object literal syntax.
    
### Examples

Making a directory
```python
import os
directory = "testDir"
parentDir = "C:/Users/iveta_6esu9b1/PycharmProjects"
path = os.path.join(parentDir, directory)
os.mkdir(path) #making dir
```
<br />

Putting a file into directory
```python
fileName = "testFile.txt"
filePath = os.path.join(path, fileName)
```
<br />

Writing into directory
```python
with open(filePath, "w") as file1:
    toFile = "Contents of file are written here"
    file1.write(toFile)
```