BACKGROUND INFORMATION FOR INSTALL SCRIPT:
	PRE-REQUISITES:
		Java (openjdk: openjdk/11.0.8_10-ge7nviu)
		GCC (gcc/10.2.0-sbrvuly)
		Python3 (Version 3.6.8)
		Spark Standalone (https://spark.apache.org/downloads.html) 


	PYTHON: PRE-REQUISITES
		pip install --upgrade pip (may need sudo for this)
		pip3 install pandas
		pip3 install pyspark
		pip3 install findspark
		pip3 install numpy
		pip3 install petastorm (NEEDS GCC and UPGRADED PIP)
		pip3 install jupyter
		pip3 install tensorflow
		pip3 install keras
		pip3 install matplotlib
		pip3 install seaborn
		
If you wish to install the above manually, you can skip step one

STEP 1: RUNNING THE PRE-REQ SCRIPT

*NOTE* you can only provide one argument at a time. (Meaning you may have to call this script multiple times)
This is because certain arguments require sudo to run properly while others do not
	Arguments:
	   	-p: install pre-requisites, NEEDS TO BE RUN WITH SUDO"
	   	-b: pip install on base machine instead of a virtual enviornment"
	   	-v: pip install on a virtual enviornment called env "
		
STEP 2: UNTAR SPARK STANDALONE TO WHERE ALL NODES CAN ACCESS IT (EITHER ON A NFS OR UNTAR ON EACH NODE )
	
	NOTE: Make sure you remember where you put spark standalone, you have to reference the path when you run the start/stop scripts

STEP 3: RUN START/STOP SCRIPTS in spark-standalone-scripts ( readme in there as well )


