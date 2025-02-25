# Data Engineering: Environment Setup

# Tools:

- **Programming Languages:** Python-3.10.11, Java-1.8.0_202
- **Big Data Tools:** Hadoop-3.3.6, Spark-3.5.4, PySpark-3.5.4, Delta-lake-3.3.0
- **Development Tools:** VSCode-1.97.2, Git-2.48.1
- **Data Science Platform:** Kaggle

# Download tools:(Keep in mind the compatibility of different tools)

### Programming Languages:

- Python Installation:
    - Go to: [https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe](https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe)
    - Let it download, navigate to download and double click on it.
    - in the install window,
        - Check these two options:
            - Use admin privileges when installing py.exe
            - Add python.exe to PATH
        - Click on:
            - Customize Installation
        - Click on Next:
        - Check the option:
            - Install Python 3.10 for all users
        - click on Install
- Java Installation:
    - Go to: [https://www.oracle.com/in/java/technologies/javase/javase8-archive-downloads.html#license-lightbox](https://www.oracle.com/in/java/technologies/javase/javase8-archive-downloads.html#license-lightbox)
    - Click on: [jdk-8u202-windows-x64.exe](https://www.oracle.com/in/java/technologies/javase/javase8-archive-downloads.html#license-lightbox)
    - Sign in with your oracle id and password (Please create if not already)
    - Let it download, navigate to download and double click on it.
    - follow the instructions to install both jdk and jre

### Big Data Tools

- Spark Installation:
    - Go to: [https://www.apache.org/dyn/closer.lua/spark/spark-3.5.4/spark-3.5.4-bin-hadoop3.tgz](https://www.apache.org/dyn/closer.lua/spark/spark-3.5.4/spark-3.5.4-bin-hadoop3.tgz)
    - Let it download, navigate to download and double click on it.
    - Extract the folder
    - Copy the extract inside  C:\Program Files\spark
- Hadoop Installation:
    - Go to: [cdarlint/winutils: winutils.exe hadoop.dll and hdfs.dll binaries for hadoop windows](https://github.com/cdarlint/winutils)
    - Get the winutils file for specific hadoop version you want.
    - Copy and paste it inside C:\Program Files\hadoop\bin

### Development Environment

- VSCode Installation:
    - Go to: [Download Visual Studio Code - Mac, Linux, Windows](https://code.visualstudio.com/download)
    - Click on: Windows
    - Let it download, navigate to download and double click on it.
    - Follow the instructions to install VSCode
- Git Installation:
    - Click on: https://github.com/git-for-windows/git/releases/download/v2.48.1.windows.1/Git-2.48.1-64-bit.exe
    - Let it download, navigate to download and double click on it.
    - follow instructions to install Git
    - Set up the Global variables for Git:
        - `git config --global [user.name] <user_name>`
        - `git config --global [user.email] <email>`

# Environment Variables:

- Go to Environment variables
- Under System Variables
- Java
    - Click on New…
    - Variable Name: **JAVA_HOME**
    - Variable Value: <path to java> e.g. C:\Program Files\Java\jdk1.8.0_202
- Spark
    - Click on New…
    - Variable Name: **SPARK_HOME**
    - Variable Value: <path to spark> e.g. C:\Program Files\spark\spark-3.5.4-bin-hadoop3
- Hadoop
    - Click on New…
    - Variable Name: **HADOOP_HOME**
    - Variable Value: <path to hadoop> e.g. C:\Program Files\hadoop
- PySpark
    - Click on New…
    - Variable Name: **PYSPARK_HOME**
    - Variable Value: <path to python> e.g. C:\Program Files\Python310\python.exe
    - Click on New…
    - Variable Name: **PYSPARK_DRIVER_PYTHON**
    - Variable Value: python
    - Click on New…
    - Variable Name: **PYSPARK_PYTHON**
    - Variable Value: python

## Referencing to bin folder

- Double click on Path variable under System Variables
- Click on New
- Java
    - %JAVA_HOME%\bin
- Hadoop
    - %HADOOP_HOE%\bin
- Spark
    - %SPARK_HOME%\bin

# Kaggle: Setup

- Install Kaggle for python
    - In terminal write:
    - `pip install kaggle`
- Go to your Kaggle account and create API key and place the kaggle.json file which downloaded into C:\Users\karan\.kaggle

# Delta-Lake: Setup

- Install delta-lake for python
    - in terminal write:
    - `pip install delta-spark`
- Go to : [Maven Repository: io.delta » delta-storage » 3.3.0](https://mvnrepository.com/artifact/io.delta/delta-storage/3.3.0)
- Download jar file.
- Let it download, navigate to download.
- Go to: C:\Program Files\spark\spark-3.5.4-bin-hadoop3\bin\jars and paste the jar file
- Go to: [cdarlint/winutils: winutils.exe hadoop.dll and hdfs.dll binaries for hadoop windows](https://github.com/cdarlint/winutils)
- Get the hadoop.dll file for specific hadoop version you want.
- Copy and paste it inside C:\Program Files\hadoop\bin

# Duckdb: Setup

- Install duckdb for python
    - in terminal write:
    - `pip install duckdb`
