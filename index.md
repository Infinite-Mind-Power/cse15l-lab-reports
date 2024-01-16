
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

#### Code Blocks:
     [user@sahara ~]$ cd
     [user@sahara ~]$
      
     [user@sahara ~]$ cd lecture1/
     [user@sahara ~/lecture1]$ 

     [user@sahara ~]$ cd /home/lecture1
     [user@sahara ~/lecture1]$ 


## `ls` (List Directory Contents)

| Command                                 | Directory | Explanation                                       |
|-----------------------------------------|-------------------|---------------------------------------------------|
| `ls`                                    | Current Directory    | List contents of the current directory.           |
| `ls lecture1/`  | lecture1 | List contents of the "lecture1" directory.                  |
| `ls /home/lecture1/`  | `/home/lecture1`   | List contents of the "/home/lecture1" directory.               |

##### Code Blocks:
    [user@sahara ~]$ ls lecture1/
    [user@sahara ~]$ ls
    
    lecture1
    [user@sahara ~]$ cd lecture1/
    
    [user@sahara ~/lecture1]$ ls
    Hello.class  Hello.java  messages  README


## `cat` (Concatenate and Display File Content)

| Command                                 | Working Directory | Explanation                                       |
|-----------------------------------------|-------------------|---------------------------------------------------|
| `cat`                                  | -                 | Error: Missing file argument.                   |
| `cat /lecture1/messages/en-us.txt      | Current Directory | Display the content of a text file.              |
| `cat /lecture1/messages/en-us.txt      | Destination path  | prints Hello World!                               |

#### Code Blocks:
    [user@sahara ~/lecture1]$ ls
    Hello.class  Hello.java  messages  README
  
    [user@sahara ~/lecture1]$ cd messages
    [user@sahara ~/lecture1/messages]$ ls
  
    en-us.txt  es-mx.txt  tr-tr.txt  zh-cn.txt
    [user@sahara ~/lecture1/messages]$ cat en-us.txt
    Hello World!




