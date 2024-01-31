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
