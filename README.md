Hadoop Word Count Project
Overview
This project implements a Hadoop MapReduce application to count word occurrences in a text file stored in HDFS. It is part of the "Data Engineer Deliverables" assignment, demonstrating distributed data processing using Hadoop's MapReduce framework. The project includes a Technical Design Document (TDD), source code, and test cases, with a theoretical demo outcome due to the absence of a local Hadoop setup.
Project Structure
wordcount_project/
├── src/
│   └── WordCount.java
├── input/
│   └── sample.txt
├── Technical_Design_Document.txt
├── Code_Snippet.txt
├── Demo_Outcome.txt
├── Test_Case_Report.txt
└── README.md


src/WordCount.java: Hadoop MapReduce program (Mapper and Reducer).
input/sample.txt: Sample input file (e.g., "hello world hello hadoop").
Technical_Design_Document.txt: Design details for the project.
Code_Snippet.txt: LMS code snippet with explanation.
Demo_Outcome.txt: Theoretical demo output.
Test_Case_Report.txt: Test case definitions and results.

Tech Stack

Hadoop: 3.x (HDFS, MapReduce, theoretical setup)
Java: JDK 11
OS: Windows 10 (local machine, no Hadoop installed)
VS Code: For code editing and documentation

Setup (Theoretical)
This project assumes a Hadoop single-node cluster (e.g., Ubuntu 20.04, Hadoop 3.x). Due to the absence of a local Hadoop installation, the demo outcome is theoretical. For a real setup:

Install Hadoop 3.x and Java JDK 11.
Configure HDFS (hdfs://localhost:9000) and YARN.
Clone this repository: git clone https://github.com/username/wordcount-hadoop.

Execution (Theoretical)

Upload Input:
Place sample.txt in HDFS: hdfs dfs -put input/sample.txt /input.


Compile:
Compile WordCount.java: hadoop com.sun.tools.javac.Main WordCount.java.
Create JAR: jar cf wordcount.jar WordCount*.class.


Run Job:
Execute: hadoop jar wordcount.jar WordCount /input/sample.txt /output.


Check Output:
View: hdfs dfs -cat /output/part-r-00000.



Theoretical Output (for sample.txt: "hello world hello hadoop"):
hadoop  1
hello   2
world   1

Deliverables

Technical Design Document (TDD):
Describes project summary, data flow, structure, tech stack, environment, and test cases.
File: Technical_Design_Document.txt.


Code:
Git Link: [Insert your GitHub URL, e.g., https://github.com/username/wordcount-hadoop].
LMS Snippet: Mapper and Reducer code with explanation (Code_Snippet.txt).
Demo Outcome: Theoretical output (Demo_Outcome.txt).


Test Case Report:
Defines three test cases (valid input, empty file, large file) with theoretical results.
File: Test_Case_Report.txt.



Notes

The demo outcome is theoretical due to no local Hadoop installation (hadoop: command not found).
The project demonstrates understanding of Hadoop’s MapReduce paradigm, suitable for classroom discussion.
For engagement, review WordCount.java and be prepared to explain Mapper and Reducer logic.
