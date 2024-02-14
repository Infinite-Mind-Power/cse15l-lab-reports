#### 4. -l (Files with matches)
The -l option lists the names of files with matching lines, rather than the matching lines themselves. It's useful for identifying files that contain certain 
patterns without displaying the content.

 Example 1: List files that contain "API" in the ./technical directory.

 `grep -l "API" ./technical/*.txt`

 output:
 ![image 6](lastone.png)

 Example 2: Find configuration files containing "timeout"

 `grep -l "timeout" ./technical/plos/*`

 output: none. There was no match.

This searches through all files in the ./technical/configs directory for the term "timeout" and lists files where the term is found, aiding in identifying which configuration files might need adjustments for timeout settings.

### These examples demonstrate the power of `grep` for searching through text files for specific patterns, with options to customize the search according to case sensitivity, recursion, exclusion of matches, and listing file names with matches.


###### Cite:
*** Sources I have used are:
Google,
https://www.geeksforgeeks.org/grep-command-in-unixlinux/,
Wikipedia
