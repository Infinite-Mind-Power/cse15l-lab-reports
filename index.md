
### Lab Report 1: Remote Access and FileSystem
Intro:

In this lab report, we explored the basic filesystem commands: `cd`, `ls`, and `cat`. 
These commands are fundamental for navigating and managing files using terminal. 
I will provide example for each command and their outputs that we used during the lab.

## `cd` command examples:
  
  ##### No Argument:
  
     [user@sahara ~]$ cd
     
     Working directory: changed to /home.
  
     [user@sahara ~]$ pwd
     /home
     
  Explanation: `cd` with no argument did not have any output, but changed my directory to /home. 
  
  Error: None. 
  
  ##### With Path as an Argument:
  
     [user@sahara /]$ cd /home/lecture1/messages
     [user@sahara ~/lecture1/messages]$ (THERE WAS NO OUTPUT.)

     Working directory: changed to /home/lecture1/messages
   
     [user@sahara ~/lecture1/messages]$ pwd
     /home/lecture1/messages
     
   Explanation: `cd` with the path to the messages as an argument changed the working 
   directory from `/home` to `/home/lecture1/messages`.
   
   Error: None.
   
  ##### With File Path as an Argument:
   
     [user@sahara ~]$ cd /lecture1/messages/Hello.java
     bash: cd: /lecture1/messages/Hello.java: No such file or directory

     Working directory: remains unchanged.
   
     [user@sahara ~]$ pwd
     /home

   Explanation: `cd` with the file path to `/lecture1/messages/Hello.java` prints an error, becuase
   it is not a directory.
   
   Error: No such file or directory
   
-------------------------------------------------------------

## `ls` Command Example:


  ##### No Argument:
  
     [user@sahara ~]$ ls
     lecture1
     
     Working directory: /home
  
     [user@sahara ~]$ pwd
     /home
     
  Explanation: `ls` Lists the content of the directory with no change to working directory. 
  
  Error: None. 
  
  ##### With Path as an Argument:
  
     [user@sahara ~]$ ls /home/lecture1/messages
     en-us.txt  es-mx.txt  tr-tr.txt  zh-cn.txt

     Working directory: Remains unchanged.
   
     [user@sahara ~/lecture1/messages]$ pwd
     /home
     
   Explanation: `ls /home/lecture1/messages` lists the content of the given directory.
   
   Error: None.
   
  ##### With File Path as an Argument:
   
     [user@sahara ~]$ ls /lecture1/messages/Hello.java
     ls: cannot access '/lecture1/messages/Hello.java': No such file or directory

     Working directory: remains unchanged.
   
     [user@sahara ~]$ pwd
     /home

   Explanation: `ls /lecture1/messages/Hello.java` does not perform any action with 
   the given directory.
   
   Error: Cannot access. No such file or directory


------------------------------------------------------------------------------

## `cat` Command Example:


  ##### No Argument:
  
     [user@sahara ~]$ cat

     
     Working directory: /home
  
     [user@sahara ~]$ pwd
     /home
  
  Explanation: `cat` command ran and a black space with blinking pointer. The user info
  vanished and had to press `ctrl+C` to exit exit.
  ![Terminal](/terminal.png)
  
  Error: None but File path is requried to perform an action.

  
  
  ##### With Path as an Argument:
  
     [user@sahara ~]$ cat /home/lecture1/messages
     cat: /home/lecture1/messages: Is a directory  

     Working directory: Remains unchanged.
   
     [user@sahara ~/lecture1/messages]$ pwd
     /home
     
   Explanation: `cat` command read Files path not a directory.
   
   Error: cat: /home/lecture1/messages: Is a directory
   
  ##### With File Path as an Argument:
   
      [user@sahara /]$ cat /home/lecture1/messages/tr-tr.txt
      Merhaba Dünya!

      Working directory: remains unchanged.
   
     [user@sahara ~]$ pwd
     /home

   Explanation: `cat /home/lecture1/messages/tr-tr.txt` command directly reads the 
   file that the path has been given to it.
   
   Error: none.


## Conclusion:

This lab report covers the basic commands `cd` `ls` `cat` to navigate through system,
using terminal and understanding this is very important for efficient work.

     


    

    
    
