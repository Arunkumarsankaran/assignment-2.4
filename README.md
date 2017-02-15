1.Hadoop in layman's term: Hadoop is an open source, Java-based programming framework that supports the processing and storage of extremely large data sets in a distributed computing environment. It is part of the Apache project sponsored by the Apache Software Foundation. It is divided into two components namely: a)Storage-HDFS b)Processing-MapReduce,pig,hiv
.


HDFS (storage) and MapReduce (processing) are the two core components of Apache Hadoop. The most important aspect of Hadoop is that both HDFS and MapReduce are designed with each other in mind and each are co-deployed such that there is a single cluster and thus pro¬vides the ability to move computation to the data not the other way around. Thus, the storage system is not physically separate from a processing system
Hadoop Distributed File System (HDFS)

HDFS is a distributed file system that provides high-throughput access to data. It provides a limited interface for managing the file system to allow it to scale and provide high throughput. HDFS creates multiple replicas of each data block and distributes them on computers throughout a cluster to enable reliable and rapid access.

The main components of HDFS are as described below:

NameNode is the master of the system. It maintains the name system (directories and files) and manages the blocks which are present on the DataNodes.

DataNodes are the slaves which are deployed on each machine and provide the actual stor¬age. They are responsible for serving read and write requests for the clients.

Secondary NameNode is responsible for performing periodic checkpoints. In the event of NameNode failure, you can restart the NameNode using the checkpoint.
MapReduce

MapReduce is a framework for performing distributed data processing using the MapReduce programming paradigm. In the MapReduce paradigm, each job has a user-defined map phase (which is a parallel, share-nothing processing of input; followed by a user-defined reduce phase where the output of the map phase is aggregated). Typically, HDFS is the storage system for both input and output of the MapReduce jobs.

The main components of MapReduce are as described below:

JobTracker is the master of the system which manages the jobs and resources in the clus¬ter (TaskTrackers). The JobTracker tries to schedule each map as close to the actual data being processed i.e. on the TaskTracker which is running on the same DataNode as the underlying block.

TaskTrackers are the slaves which are deployed on each machine. They are responsible for running the map and reduce tasks as instructed by the JobTracker.

JobHistoryServer is a daemon that serves historical information about completed applications. Typically, JobHistory server can be co-deployed with Job¬Tracker, but we recommend to run it as a separate daemon.



3.Explain the reasons to learn Big data technologies

 •Build new applications: Big data might allow a company to collect billions of real-time data points on its products, resources, or customers – and then repackage that data instantaneously to optimize customer experience or resource utilization. For example, a major US city is using MongoDB to cut crime and improve municipal services by collecting and analyzing geospatial data in real-time from over 30 different departments. •Improve the effectiveness and lower the cost of existing applications: Big data technologies can replace highly-customized, expensive legacy systems with a standard solution that runs on commodity hardware. And because many big data technologies are open source, they can be implemented far more cheaply than proprietary technologies. For example, by migrating its reference data management application to MongoDB, a Tier 1 bank dramatically reduced the license and hardware costs associated with the proprietary relational database it previously ran, while also bringing its application into better compliance with regulatory requirements. •Realize new sources of competitive advantage: Big data can help businesses act more nimbly, allowing them to adapt to changes faster than their competitors. For example, MongoDB allowed one of the largest Human Capital Management (HCM) solution providers to rapidly build mobile applications that integrated data from a wide variety of disparate sources. •Increase customer loyalty: Increasing the amount of data shared within the organization – and the speed with which it is updated – allows businesses and other organizations to more rapidly and accurately respond to customer demand. For example, a top 5 global insurance provider, MetLife,used MongoDB to quickly consolidate customer information from over 70 different sources and provide it in a single, rapidly-updated view. • Demand for Big Data skills is extremely high, and being able to prove your expertise is of essence • 64% of IT hiring managers rate skilled big data knowledge as having extremely high or high value when rating expertise of candidates; this is based on a survey by CompTIA. • According to Forbes, the median advertised salary for professionals with Big Data expertise is $124,000 a year. • IBM, Cisco, and Oracle together advertised 26,488 open positions that required Big Data expertise in the last twelve months.
