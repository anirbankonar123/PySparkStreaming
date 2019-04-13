# PySparkStreaming <br>
Reads streaming data from twitter and displays aggregated bar plots based on hashtags <br>

Set up an account at developer.twitter.com, accept the agreement and click defaults, provide reason for your account etc<br>
Then create an app, and setup the credentials for a twitter app at https://developer.twitter.com/en/apps, ex: https://anirbank.twitter.com<br>


<b>Following libraries are to be installed:</b><br>

sudo apt-get install default-jre (this is linux default jre, make sure version 1.8.x is installed)<br>
sudo apt-get install scala (check for version 2.11.6-6)<br>
sudo pip3 install py4j<br>
Download spark (version 2.1, with Hadoop 2.7 works best) and extract the tar file<br>
wget -q https://archive.apache.org/dist/spark/spark-2.1.1/spark-2.1.1-bin-hadoop2.7.tgz<br>
pip install pyspark<br>
pip install findspark<br>
pip install python-twitter - a python library to connect your Python to the twitter dev account.<br>
pip install tweepy<br>

Setup following env vars:<br>
export SPARK_HOME=.... (path where the spark-2.1.1-bin-hadoop2.7 is extracted)<br>
export PATH = $SPARK_HOME:$PATH<br>
export PYTHONPATH=$SPARK_HOME/python:$PYTHONPATH<br>
export PYSPARK_DRIVER_PYTHON="jupyter"<br>
export PYSPARK_DRIVER_PYTHON=OPTS="notebook"<br>

In addition you might have to setup JAVA_HOME (since I am using default jre in Linux, I am not setting it)<br>
    
