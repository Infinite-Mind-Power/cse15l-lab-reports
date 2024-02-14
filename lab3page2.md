## Part 2
### My favorite command is `grep`. The reasone I chose it is becasue it is a powerfull 
### tool which can: 

- Searching text: grep can search one or more files for lines that contain a match to
a specified pattern.
- Filtering log files: It's commonly used to filter interesting entries from log files.
- Code analysis: Programmers use grep to find occurrences of a term in source codes.
- Data analysis: It can be used for quick-and-dirty data analysis, filtering lines in
data files that match a certain criterion.
- Combining with other commands: In shell scripts or command pipelines, grep is used
in conjunction with other commands to process text.

(source: Wikipedia)


#### 1. -i (Ignore case)
The -i option makes grep perform case-insensitive searching. This means grep will match lines regardless of whether the characters are 
upper or lower case.

Example 1: Search for the word "Elyas" in all text files, ignoring case

 Bash:
 
 `grep -i "states" ./plos/*.txt`

 This command searches for the term "network" in all .txt files within the ./technical directory, ignoring case. It's useful when the 
 casing of the search term is unknown or mixed.

 #### 2. 
  


