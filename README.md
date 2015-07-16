This is a very basic Storm topology that randomly emits sentences, splits them into individual words, and keeps a count of how many times each word has occurred.

See [Develop a Java topology for Storm on HDInsight](https://azure.microsoft.com/en-us/documentation/articles/hdinsight-storm-develop-java-topology) for a walkthrough of the code.

##To run

1. Fork/Clone the repository to your development environment.

2. Install Java JDK 7 or higher. This was tested with Oracle Java 7 and 8, but should work under things like OpenJDK as well.

3. Install [Maven](http://maven.apache.org/)

4. Assuming Java and Maven are in the path, and everything is configured fine for JAVA_HOME, use the following to build and run the topology on the development environment:

        mvn compile exec:java -Dstorm.topology=com.microsoft.example.WordCountTopology
