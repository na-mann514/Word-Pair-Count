# Word-Pair-Count
Map Reduce Job to count frequency of all pairs of words in a file

# Description
This is a MapReduce Job written in Java-1.7 to output the frequency of all the possible pair of "valid words" in a text file. Conditions:
1.  Valid words contains [a-z A-Z 0-9] only
2.  Code ignores all the punctuation marks and special characters other than valid characters listed in point 1
3.  Examples of valid word: Hello-World will be considered as a pair (Hello , World), (1992) will be considered as 1992 etc.
4.  Example Input: a cat is really a cat!
    Example Output: a cat 2
                    cat is 1
                    is really 1
                    really a 1
                    
# How to run?
1.  Set up a Hadoop environment.
2.  Download the java file: WordPairCount.java, add it to your Java Project using your favorite IDE
3.  Using your favorite Build tool resolve all the dependencies - For this code, all you need is Apache Hadoop Client
    Maven repo link: https://mvnrepository.com/artifact/org.apache.hadoop/hadoop-client/2.6.0
4.  Create a Jar File and run using the following command on Hadoop Bash:
    hadoop jar <Jar-File-Name>.jar <HDFS-PATH-TO-YOUR-INPUT-TEXT-FILE>.txt <OUTPUT-FILE-NAME-WILL-BE-CREATED-BY-HADOOP>
    

