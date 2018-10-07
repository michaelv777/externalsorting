Externalsorting
==========================================================
External-Memory Sorting in Java: 
Sort very large files using an external-memory algorithm.

Require at least Java 8. 


How to build [optional - all the jars and compiled classes have been provided - see How to run description]
-----------------

- get the java jdk
- Install Maven 2
- mvn install - builds jar
- mvn test - runs tests

How to run
-----------------
STEP 1 - download the project from the Hithub
https://github.com/michaelv777/externalsorting.git

STEP 2 - run the main class or jar file
 
Run Option 1:
1. CD to target/classes folder
2. Run: java com/externalsorting/FileSort FileSortInput.txt FileSortOutput.txt -d

Run Option 2:
1. CD to target folder
2. Rename externalsorting.jar.tmp to externalsorting.jar
3. CD to target/lib foler
4. Rename *.jar.tmp to *.jar
3. Run: java -jar externalsorting.jar FileSortInput.txt FileSortOutput.txt -d   

All the run flags:
java com.externalsorting.FileSort inputfile outputfile [flags]
Flags are:
-v or --verbose: verbose output
-d or --distinct: prune duplicate lines
-t or --maxtmpfiles (followed by an integer): specify an upper bound on the number of temporary files
-c or --charset (followed by a charset code): specify the character set to use (for sorting)
-z or --gzip: use compression for the temporary files
-H or --header (followed by an integer): ignore the first few lines
-s or --store (following by a path): where to store the temporary files
-h or --help: display this message