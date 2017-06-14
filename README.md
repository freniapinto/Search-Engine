# Information Retrieval FinalProject
- Please extract the files from the folder "Search-Engine"
- Please install the following libraries so that the code doesn't throw error execute the following in terminal
"pip install BeautifulSoup4"
"pip install stemmer"

The files present are:
all_runs: text files and spreadsheets of all the runs mentioned in the requirement of the project
cacm : The cacm documents
clean_cacm : cleaned documents(all terms are converted to lower case and stripped of punctuations) of cacm
evaluation_phase2 : this file consists of the text files contining MAP, MRR, P@K, precision and recall for the retrieval models involved in this project
stopped_cacm : the corpus with no stop words present in it
task1 : this file contains the text files for the 4 retrieval models
task2 : the text files in this folder are the clean queries and the results for rocchios pseudo relevance
task3a : this contains two text files, one containing the queries without stopowords and the other file containing the results of pseudo relevance model on stopped queries
task3b : this contains two text files, one containing the stemmed queries and the other file containing the results of pseudo relevance model on stemmed queries
taskphase2 : a text file with stopped and expanded queries and the output of the expansion technique on these queries
graph_imgs: this folder contains the graph plotted against precision and recall for each run and the 64 queries and the code file to generate the graph


- The source code for this project is named "project.py"
- Please install python 2.7 in the system.
- You can run the code by executing the command "python project.py" in terminal.
- Open the file "project.py" and run it. the initial run gives the output for task1
- To get the results for the remaining tasks, please uncomment the function names according to the requirement.
- The snippet generator file "SnippetGen.py" requires users input. Upon the request please enter a query ID  

- To run the lucene java file
--------------------------------------------------------------------------------------------------------------

HOW TO INSTALL LIBRARIES TO RUN THE CODE ON WINDOWS:

Import the following JARS:
1) lucene-core-VERSION.jar
2) lucene-queryparser-VERSION.jar
3) lucene-analyzers-common-VERSION.jar.

Create two directories: 
1) Index - to store indexes created by Java code
2) Documents - to store the cleaned corpus from the previous homework

Also, added a hashmap function for retrieving doc_id from the index file created from the last homework

---------------------------------------------------------------------------------------------------------------

HOW TO RUN THE PROGRAM:

Run the Java code on Netbeans/Eclipse. 

--------------------------------------------------------------------------------------------------------------

PROGRAM RESULTS:

The code generates a ranked list of top 100 documents depending on the similarity scores generated by Lucene library and retrieval models for each query. And hence, there are 6400 rows formatted in TREC

-------------------------------------------------------------------------------------------------------------

FORMAT OF THE FILES:
The precision and recall files contain three extra columns apart from the TREC format namely 'relevance', 'precision' and 'recall'
The MAP and MRR files are a single value average over 64 queries
The P@K is the value at K=5 and K=20 for each query

* We have attached the excel files in the documentation PDF, in case they don’t open please refer to the .docx file attached.




