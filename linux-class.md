# Basic Linux Introduction

**What is Linux**
Linux is a family of open-source Unix-like operating systems based on the Linux kernel. [more](https://en.wikipedia.org/wiki/Linux)

**What is Command Line**

The command line, also known as the command-line interface (CLI) or terminal, is a text-based interface in which the user interacts with a computer by typing commands. It allows users to perform various tasks and operations on a computer without using a graphical user interface (GUI)



**Linux File Hierarchy Structure**

![image](https://linuxhandbook.com/content/images/2020/06/linux-directory-structure.png)

The Linux File Hierarchy Structure (FHS) is a system that organizes the files and directories on a Linux system. It provides a standard and consistent way of organizing the file system, ensuring that different programs and services can find the files and resources they need
```
Link 1: https://help.ubuntu.com/community/LinuxFilesystemTreeOverview
Link 2: https://www.geeksforgeeks.org/linux-file-hierarchy-structure/

```
# Basic Linux Commands
`ls`

List the files and directories in the current directory.

```shell
 Additional options:
-l: Long format, showing detailed information about files.
-a: Include hidden files starting with a dot (.).
```

`cd` (Change Directory)

```shell
Change the current working directory. Replace [directory] with the desired directory name.

Additional tips:

cd .. : Move to the parent directory.
cd ~ : Move to the home directory.
```

`pwd`

The pwd command in Linux stands for "Print Working Directory.

```shell
$ pwd
/home/user/documents
In this example, the output /home/user/documents indicates that the current working directory is documents, which is located inside the user directory, which, in turn, is inside the home directory.

Purpose:

It helps you understand your current location within the file system.
Useful when you need to reference the full path of the current directory or provide the path for other commands.
```

`mkdir` (Make Directory)

The mkdir command in Linux is used to create new directories (folders).

```shell
Create a new directory:

mkdir my_directory
This creates a directory named my_directory in the current working directory.

Create a nested directory:

mkdir -p my_parent_directory/my_child_directory
The -p option creates parent directories as needed. In this example, it creates both my_parent_directory and my_child_directory.

Purpose:
To create new directories in the file system.
```

`touch` 


The touch command in Linux is used to create empty files or update the access and modification times of existing files.

```shell
Command : touch [options] [filename]
Create an empty file:

touch myfile.txt

This command creates a new empty file named myfile.txt in the current working directory.

Update access and modification times of a file (if the file exists):

touch existing_file.txt

If existing_file.txt already exists, the touch command updates its access and modification times to the current time.

Purpose:

To create empty files.
To update the timestamp (access and modification times) of a file.

```

`cat` (Concatenate and Display)

The cat command in Linux is used to concatenate and display the content of files. It is a versatile command that can be used for various purposes related to working with text files. 

```shell
Command: cat [filename]
Ex: cat myfile.txt


Purpose:

To display the content of one or more files.
To concatenate and display the content of multiple files.
```

`grep`

The **grep** command in Linux is used to search for specific patterns or regular expressions in files or streams of text. The name "grep" stands for "Global Regular Expression Print." It is a powerful tool for text searching and manipulation.

```shell
Command: grep [options] pattern [file(s)]

Example: grep -i "pattern" filename.txt

pattern: The text or regular expression you want to search for.
[file(s)]: Optional. If provided, grep will search for the pattern in the specified file(s). If not provided, grep reads from the standard input (e.g., output from another command or from a pipeline).
```
