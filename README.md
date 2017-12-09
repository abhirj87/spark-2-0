# Spark

## Pre-requisites for Installation

Java installed on the laptop

## Download Spark 2.2.0

- Download Spark 2.2.0 from here : http://spark.apache.org/downloads.html

## Install Spark 2.2.0 on Mac

- tar -zxvf spark-2.2.0-bin-hadoop2.7.tgz

- export PATH=$PATH:/Users/path_to_downloaded_spark/spark-2.2.0-bin-hadoop2.7/bin

## Install Spark 2.2.0 on Windows

- Download Spark 2.2.0 from https://spark.apache.org/downloads.html
  - Accept default Spark release and package type - spark-2.2.0-bin-hadoop2.7.tgz file
  - If necessary download and install 7Zip program to extract .tgz files
 
- Extract spark-2.2.0-bin-hadoop2.7.tgz file
 
- Add the spark bin directory to Path : ...\spark-2.2.0-bin-hadoop2.7\bin
 
- Download/Clone WinUtils from https://github.com/steveloughran/winutils
 
- Copy all files under winutils\hadoop-2.7.1\bin from where WinUtils was extracted/cloned to the spark-2.2.0-bin-hadoop2.7\bin directory.
 
- Set the following Environment Variables (User level is fine):
  - HADOOP_HOME : to your spark-2.2.0-bin-hadoop2.7 directory
  - SPARK_HOME : to your spark-2.2.0-bin-hadoop2.7 directory
  
## Git

Nice to have

[IMPORTANT]: Downloads
Have the following downloaded before the session
* Spark binaries
* JDK installed

## Code

git clone https://github.com/jayantshekhar/spark-2-0
mvn clean package

## Execute

- hadoop fs -put README.md
- hadoop fs -put data

- spark2-submit --class org.workshop.SparkBasics --master yarn --deploy-mode client --executor-memory 1G  --num-executors 1 --executor-cores 1 target/spark-exercises-1.0-jar-with-dependencies.jar







