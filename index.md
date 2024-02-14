Example 1: Search for the word "configuration" in a specific document, ignoring case
 
 `grep -i "configuration" ./technical/plos/*.txt`
 
 output:
 
 ![image2](grepplos2.png)

 This command searches for the term "network" in all .txt files within the ./technical directory, ignoring case. It's useful when the 
 casing of the search term is unknown or mixed.

#### 2. -r or -R (Recursive search)
The -r (or -R, which is equivalent) option enables recursive search, allowing grep to search through directories and their subdirectories for the pattern.

 Example 1:
   
 `grep -r "error" ./technical/plos/*.txt`

  output:

  ![iamge3](greprtech.png)
   

 Example 2: Recursively search for "error" in all files within the ./technical/ directory without the specific folder name.
 
 `grep -ri --include="*.md" "todo" ./technical/

 output:

 ![image4](grepri.png)
