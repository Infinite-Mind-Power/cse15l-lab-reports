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
