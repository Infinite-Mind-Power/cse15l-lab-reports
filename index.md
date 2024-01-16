
---
layout: normal post
title: "Lab Report 1 - Remote Access and FileSystem (Week 1)"
Name: Elyas Emami
---

# Lab 1 - Remote Access and FileSystem

Below is the things that I learned in this very first lab.

## `cd` (Change Directory)

| Command                                 | Directory | Explanation                                       |
|-----------------------------------------|-------------------|---------------------------------------------------|
| `cd`                                    | Home Directory    | Navigate users home directory.           |
| `cd`  `lecture1/`                        | Change Directory to lecture1 | Change to a specific directory.                  |
| `cd`  `cd /home/lecture1/`               | - lectuer1   | Navigates to lecture1               |

![Lab Image1](main/Screenshot 2024-01-15 at 23.43.49.png)

<img src="main/Screenshot 2024-01-15 at 23.43.49.png" width="24"/>





## `ls` (List Directory Contents)

| Command                                 | Working Directory | Explanation                                       |
|-----------------------------------------|-------------------|---------------------------------------------------|
| `ls`                                    | Current Directory | List contents of the current directory.          |
| `ls /path/to/directory`                 | Current Directory | List contents of a specific directory.           |
| `ls /path/to/file.txt` (Error)         | - /home/lecture1   | Error: Cannot list contents of a file.          |

## `cat` (Concatenate and Display File Content)

| Command                                 | Working Directory | Explanation                                       |
|-----------------------------------------|-------------------|---------------------------------------------------|
| `cat` (Error)                          | -                 | Error: Missing file argument.                   |
| `cat /path/to/file.txt`                | Current Directory | Display the content of a text file.              |
| `cat /path/to/directory` (Error)       | -                 | Error: Cannot display contents of a directory.   |
