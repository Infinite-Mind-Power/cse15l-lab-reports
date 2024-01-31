-------------------------------------------------------

## `cat` Command Example:


  ##### No Argument:
  
     [user@sahara ~]$ cat

     
     Working directory: /home
  
     [user@sahara ~]$ pwd
     /home
  
  Explanation: `cat` command ran and a black space with blinking pointer. The user info
  vanished and had to press `ctrl+C` to exit.
  
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

     
