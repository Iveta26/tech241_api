# Intro to Scripting

<br />

### What is scripting?
A scripting language or script language is a programming language that is used to manipulate, customize, and automate the facilities of an existing system. Scripting languages are usually interpreted at runtime rather than compiled.

<br />

### Why is it important in DevOps?

Shell scripting for DevOps enables automation of deployment, configuration management, CI/CD pipelines, monitoring, logging, and performance optimization tasks. Shell scripting languages, such as Bash, are used for automating tasks in DevOps workflows.

<br />

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