
### Lab Report 1: Remote Access and FileSystem
Intro:

In this lab report, we explored the basic filesystem commands: `cd`, `ls`, and `cat`. 
These commands are fundamental for navigating and managing files using terminal. 
I will provide example for each command and their outputs that we used during the lab.

## `cd` command examples:
  
  Working directory: /home
  
  ##### No Argument:
  
     [user@sahara ~]$ cd

  Explanation: `cd` with no argument did not have any output, but changed my directory to /home. 
  
  Error: None. 
  
  ##### With Path as an Argument:
  
     [user@sahara /]$ cd /home/lecture1/messages
     [user@sahara ~/lecture1/messages]$ (THERE WAS NO OUTPUT.)
     
  Explanation: `cd` with the path to the messages as an argument changed the working 
   directory from `/home` to `/home/lecture1/messages`.
   
  Error: None.
   
  ##### With File Path as an Argument:
   
   `cd` with the file path to `/lecture1/messages/Hello.java` 
    gave an error as an output.
   
      [user@sahara ~]$ cd /lecture1/messages/Hello.java
      bash: cd: /lecture1/messages/Hello.java: No such file or directory

   
     
     
     [user@sahara ~]$ pwd
     /home
    
     [user@sahara ~]$ ls
     lecture1
     
  `ls` with no argument listed the directo
      
     [user@sahara ~]$ cat
      (THERE WAS NO OUTPUT.)
     

Explanation: The cd command with no arguments takes the user to their home directory. pwd show the current directory
             that the user is working inside.
Error Output: No error, but when I run the `cat` command there was no output.


### Directory Path as an Argument:
  Argument: /home/lecture1/messages
  


    [user@sahara ~]$ ls /home/lecture1/messages
    Output: en-us.txt  es-mx.txt  tr-tr.txt  zh-cn.txt

    [user@sahara ~]$ pwd /home/lecture1/messages
    Ouput: /home

    [user@sahara ~]$ cat /home/lecture1/messages
    Output: cat: /home/lecture1/messages: Is a directory

Explanation: This command changes the current working directory to the specified path.
Error output: While ran command `cat` the output was an error that said "cat: /home/lecture1/messages: Is a directory".




    

    

    
    
