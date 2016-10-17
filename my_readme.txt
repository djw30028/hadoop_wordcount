mvn clean package

== Install Hadoop
brew install hadoop
/usr/local/Cellar/hadoop/2.7.3/libexec/etc/hadoop/hadoop-env.sh,

alias hstart="/usr/local/Cellar/hadoop/2.7.3/sbin/start-dfs.sh;/usr/local/Cellar/hadoop/2.7.3/sbin/start-yarn.sh"
alias hstop="/usr/local/Cellar/hadoop/2.7.3/sbin/stop-yarn.sh;/usr/local/Cellar/hadoop/2.7.3/sbin/stop-dfs.sh"

source ~/.profile

Resource Manager: http://localhost:50070
JobTracker: http://localhost:8088
Specific Node Information: http://localhost:8042

============================
https://examples.javacodegeeks.com/enterprise-java/apache-hadoop/hadoop-hello-world-example/

Apache Hadoop consists of two core components, they are:
-- Distributed File System called Hadoop Distributed File System or HDFS for short.
-- Framework and API for MapReduce jobs.

============================
== Execute, not working
WOrdCount.
java -cp target/wordcount-0.0.1-SNAPSHOT.jar com.javacodegeeks.examples.wordcount.WordCount Input.txt output.txt