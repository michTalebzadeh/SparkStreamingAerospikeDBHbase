# SparkStreamingAerospikeDBHbase

With better and improving performance, organisations are looking at using data warehouses in real time. The idea of periodic load of data into data warehouses has given rise to continuous load of data in real time. This has been made possible through new capability additions to Big Data artefacts, resulting in enhanced capabilities and better throughput.
The notion of what is real time does play a role here. The engineering definition of real time is roughly fast enough to be interactive. However, I put a stronger definition.
In real time application or data, there is no such thing as an answer which is supposed to be late and correct. The timeliness is part of the application.
If we get the right answer too slowly it becomes useless or wrong. We also need to be aware of latency trades off with throughput.

Within a larger architecture, often latency is dictated by the lowest denominator which often does not adhere to our definition of low latency. For example, Kafka as widely deployed today in Big Data Architecture is micro-batch. A moderate-latency message queue that is Kafka plus low latency processor equals a moderate-latency architecture. Hence, the low latency architecture must be treated within that context. 

The challenge in such an architecture is that everything must not only work, but it must work seamlessly. The more links in the chain from source to the engagement of data, the more points of vulnerability.
That is the reason that redundancy and fault tolerance need to be part of solution design and built-in from start

Technology Stack Used
 Kafka Cluster 2.12-1.1.0
Apache Flume Cluster 1.8.0
Spark Streaming 2.3, Spark SQL 2.3
Hadoop 3.1.0
Apache Hbase 1.2.6
Aerospike Server Enterprise-4.5.2.1-el7
Scala 2.11.8 Functional Programming
