***************README file for MPI Page Rank*******************

9/24/2012

CONTENTS OF PACKAGE 1_Project1P2:

The package contains five files,
-Mpi_Pagerank.java : The source code for the project
-Mpi_Pagerank.class : The executable class file built from the same code
-README.txt : The README file to describe how to run mpi_pagerank.class
-Group01_Project1P2_Report.docx: The technical report for the project
-Group1_pagerank_output.txt : The output file that contains the top 10 ranking url numbers with input file pagerank.input.1000.1





TO RUN THE PROGRAM:

When running the program on Eclipse IDE, following settings have to be made.

1.Create a Java project and under libraries tab click on Add External Jars. Browse and select mpj.jar file and click on add.
2.Place the mpi_pagerank.java file under src folder of the project.
3.To run this project, go to Run Configurations uder Run tab.
4.Go to Environment tab and select New. Give name as 'MPJ_HOME'.
5.If the variable does not exist, then set the value by clicking on Variables -> Edit Variables -> Browse and select the path where 'mpj-v0_38' is stored.

Now, under Arguments tab, following command line arguments have to be given.
1. Type '-jar', then click on Variables and select the MPJ_HOME variable. Once selected, it appears as: -jar ${MPJ_HOME}
2. Complete the argument list as: -jar ${MPJ_HOME}/lib/starter.jar
3. In the program arguments section, enter the arguments as follows:
   -np [number of processes] [input file name] [output file name] mpi_[number of iterations] [threshold]
4. To enable the debug mode enter "-d" in the command line arguments. Ex: 
   -np [number of processes] [input file name] [output file name] mpi_[number of iterations] [threshold] -d
5. To check the usage/help enter "-help" as follows:
   -np [number of processes] -help
6. Click on Apply and Run.


NOTE: 
-Ensure that the number of iterations and number of processes given is a positive integer greater than 0. 
-The threshold value should be greater than 0.0



***************** END of FILE *******************