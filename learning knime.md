# Knime
Question:

1. where is the example server, registration
2. interface other eclipse plugins, if yes, any outsife of knime commonly used plugins
3. is there a code generation or write the python or java code that can be used in production
4. is there a standard workflow description whick allow us to leverage the development in Knime to other "analytics engine"
5. public nodes repository/hub
6. publish research results

[open source data analytics tools][9], 
[wikipedia-Knime][10],
[interface with HortonWorks][11]
[Knime product matrix][19]

## Getting Started
* [download, installation and getting started][1]
* [Knime tv channel][3]

## Overview
This is a general analytics work flow with Knime ![workflow][5]

![example-2][12]
![ml workflow][20]

## IDE/Workbench
![knime UI][7]
From: [Beginner's Luck][8]

## Nodes Respository


## Data Source
Data from the [UC Irvine Machine Learning Repository][17]:
[￼￼Adult.data][13][Iris data][14][Yellow-small.data (Balloons)][15] 
[Wine data][16]

## Exercises
[update IDE first][18], then 
IDE help > update site: http://www.knime.org/update/2.11 > select KNIME & extension

### Chapter 2
#### Exercise 1
1. under LOCAL, **workspace**, create then a new **workflow group** and call it “Chapter 2”
2. create a new **workflow**, let’s call it “my_first_workflow”, delete it and start and new `workgroup` called exercise1.
3. add `File Reader` node, `Row Filter` node, `Column Filter` node and `File Writer` node. Usually, we will add one node at time after we reviewed the result and decided  what do we need to do next.

`File Reader node`:

* Read file data1.txt (from the “Download Zone”) by indicating file URL, use "," as column delimiter, change column “ranking” as String and name “marks”;
* We found the first 5 rows are comments, we need to remove it, and we have no interest on the column <class>.

`Row Filter`:

* Remove initial comments (row 1-5) from data read from file; Use excluding row by (beginning and ending) row numbers

`Column Filter`:* Remove column “class” by adding <class> column in exluding box.
`CVS File Writer`
* Check options in setting (write column header, row number), and define delimiter (in advance tab). If you check "abort" when file exist, it will not execute until you switch to "overwrite".

`Line Chart` (optional)
![Chapter 2 - Exercise 1][21]

* just connect it to the last processing node, execute. 
Exercise 2 is similar to exercise 1 except the file output is in append mode.

### Chapter 3


### Chapter 4


### Chapter 5


### Chapter 6



## Links
[1]:https://www.knime.org/
[2]:https://tech.knime.org/screencasts
[3]:https://www.youtube.com/user/KNIMETV
[4]:https://www.knime.org/learning-hub
[5]:http://note.io/1cFBO0B 
[6]:https://tech.knime.org/installation-0
[7]:http://note.io/1DjQB6J
[8]:https://www.knime.org/files/bl_sample_s.pdf
[9]:http://butleranalytics.com/5-free-data-mining-tools/
[10]:http://en.wikipedia.org/wiki/KNIME
[11]:http://hortonworks.com/wp-content/uploads/2014/12/Knime-Hortonworks-Solutions-Brief.pdf
[12]:https://www.knime.org/files/marketingworkflow_2.10.png
[13]:http://archive.ics.uci.edu/ml/datasets/Adult[14]:http://archive.ics.uci.edu/ml/datasets/Iris[15]:http://archive.ics.uci.edu/ml/datasets/Balloons[16]:http://archive.ics.uci.edu/ml/datasets/Wine[17]:http://archive.ics.uci.edu/ml/index.html
[18]:https://www.knime.org/downloads/update
[19]:https://www.knime.org/products/product-matrix
[20]:http://note.io/1bg94Lu
[21]:http://note.io/1aIHSDO

