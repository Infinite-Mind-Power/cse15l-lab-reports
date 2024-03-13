# Lab Report 5 - Debugging an Array Reversal Program in Java



### Trouble with Array Reversal Java Program


Hello everyone,

I'm having trouble with a Java program designed to reverse an array of integers inputted via command-line arguments. The program is supposed to split the input string into an array, reverse the array, and print the result. However, the output doesn't seem to reflect a correctly reversed array. Here's the Java code I'm using:

#### The code:
![Screenshot 1](originalcode.png)

#### The output:
![Screenshot 2](output.png)


## Response from a TA:

It looks like you're on the right track suspecting the loop. When swapping elements, you should consider how you're accessing the indices of the array. Remember, arrays in Java are zero-based. Can you try adjusting the indices during the swap and see if that fixes your issue? Please share your findings after you make the adjustment.
### The bug is here:
![Screenshot 3](buggy.png)

### This might fix the code:
![Screenshot 4](fixed.png)

#### In the reverseArray method, adjust the indices used during the swap to correctly access the mirrored element in the array. Specifically, change:


## Follow-up Post by the Student:
Thank you for the quick response! Here's the Bash script I use to compile and run my Java program:

Bash Script (compileAndRunReverseArray.sh):

### This is the bash code I used:

![Screenshot 5](bashcode.png)

![Screenshot 6](reverarraybash.png)


Thank you for the hint! I adjusted the indices in the swapping logic, and now the program works perfectly. Here's the corrected part of the code and the new output.

