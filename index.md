#### 3. -v (Invert match)
The -v option inverts the match, showing lines that do not match the given pattern. It's useful for excluding specific patterns from the search results.

 Example 1: Show lines that do not contain "success" in a txt files
 
 `grep -v "success" ./technical/plos/*.txt`

 output:

 ![image5](grepv1.png)
 
 Example 2: Exclude lines with "deprecated" from source code files in the ./technical/
 
 `grep -v "deprecated" ./technical/*.java`


 output: none. There were no code files.

This command filters out lines containing "success" from all of the txt files in the directory, which can be helpful for focusing on lines that indicate warnings, 
errors, or other statuses.
