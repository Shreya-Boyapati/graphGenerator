graphGenerator
=======================
#### The purpose of this project is to act as an extension to NetGameSim that outputs .txt files in addition to .ngs

Overview
---
* [NetGameSim](https://github.com/0x1DOCD00D/NetGameSim) is a graph generating platform that outputs in the .ngs format
* graphGenerator adds to NetGameSim in order to produce two additional .txt files containing graph information
* The first file /{path}/input.txt contains five semi-colon separated strings:
    * nodes of the original graph
    * nodes of the perturbed graph
    * edges of the original graph
    * edges of the perturbed graph
    * nodes that contain valuable data
* The second file /{path}/input2.txt is written in UTF_8 encoding and contains rows of "node node" pairs

Installing, Compiling and Running NetGameSim 
---
* graphGenerator has the same prerequisites as NetGameSim. Once all prerequisites are met, clone [graphGenerator](https://github.com/Shreya-Boyapati/graphGenerator/tree/main) using the command ```git clone```;
* Once the repository is cloned, assuming its local path is the root directory ```/path/to/the/cloned/graphGenerator``` open a terminal window and switch to the directory ```cd /path/to/the/cloned/graphGenerator```;
* Build and run the project using the command ```sbt clean compile run```
* Alternatively, you can load the project into IntelliJ and compile and run it using the main entry point in [Main.scala](src/main/scala/Main.scala);
* You should make sure that the Java version that is used to compile this project matches the JVM version that is used to run the generated program jar from the command line, otherwise you may receive an error.

Running graphGenerator results in many log messages, the last log entries can look like this:
```
Loading the NetGraph from /Users/shreyaboyapati/Downloads/graphGenerator-mainNetGraph_02-11-23-15-21-30.ngs.perturbed
15:21:32.364 [main] INFO  - Deserialized the object List(NodeObject(1,5,13,1,36,4,2,10,0.6326104150056775,false), NodeObject(2,4,7,1,50,2,6,8,0.9790725510773015,false), NodeObject(3,5,7,1,35,2,6,6,0.7933514825145984,false)...NodeObject(397,4,7,1,41,3,0,11,0.6950922868607358,false),0,32,Some(1),0.794390188624053))
15:21:32.368 [main] INFO  - Deserialized 493 nodes and 918 edges
15:21:32.411 [main] INFO  - Graph info found at /Users/shreyaboyapati/Downloads/randomWalker-main/input02-11-23-15-21-32/input.txt
```

Maintenance notes
---
This program is written by [Dr. Mark Grechanik](https://www.cs.uic.edu/~drmark/) and appended to by Shreya Boyapati







