# WordCount
Class assignment to understand Hadoop by implementing simple WordCount application.

### Objectives
1. Understand the MapReduce programming model.
2. Setting up Hadoop on a single node and on a cluster of nodes.

### Requirements
    1. Hadoop >= 3.2.1 or greater
    2. Java >= 14 or greater
    3. Intellij-IDEA (IDE)

### Installation

1. It is required to install Hadoop on both single node cluster and multiple nodes cluster. Next, you will practice running few HDFS commands and executing Hadoop jobs. You can use the following command to download Hadoop on your machine:
   ```bash
   wget http://www-eu.apache.org/dist/hadoop/common/hadoop-3.2.1/hadoop-3.2.1.tar.gz
   ```

2. You can extract the downloaded file using:
    ```bash
    tar -xzvf hadoop-3.2.1.tar.gz
    ```
3. Download text files from the https://www.gutenberg.org/, in Plain Text UTF-8 format (hint: you can use wget)

4. Download the above data and store them to the **input** directory on your machine.

5. Create a new file mydata.txt in the input directory. Open the file and write to it this line:
 FirstStudentID SecondStudentID. Repeat this line four times in the file.

6. Copy the input directory from your local disk to HDFS. You can use the command:  
    ```bash
    hadoop fs -copyToLocal /home/userid/input /home/userid/input
    ```
   The first path is the source, which is on your local disk. The second path is the destination, which is on HDFS.

7. Now check that the files were already copied using this command:
     ```bash
   hadoop fs -ls /home/userid/input
     ``` 

8. Now open IDE and compile and run to see the output in the **output** folder. OR Create a **.JAR** file to execute using hadoop.

#### Running Hadoop Jobs
At this step, you run Hadoop jobs on the data loaded on HDFS.
1. You need to build the WordCount example described in this tutorial. Name the created jar file
wc.jar.

2. You are now ready to run the jar file using:
   ```bash
   hadoop jar wc.jar /home/userid/input /home/userid/output
   ```
3. Check the output files created in the /home/userid/output.

4. You're all done :)


## Contribute
Want to work on the project? Any kind of contribution is welcome!

Follow these steps:
- Fork the project.
- Create a new branch.
- Make your changes and write tests when practical.
- Commit your changes to the new branch.
- Send a pull request.

- drop a mail to me for database file at debajyotiguha11@gmail.com
## Authors

1. ***[Debjyoti Guha](https://github.com/debajyotiguha11/)***
2. **Other project files used are subjected to CopyWrite**
