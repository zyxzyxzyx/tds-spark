# Top-Down Specialization on Apache Spark&trade;

Proposed top-down specialization algorithm on Apache Spark for COMP 5704

# Build

Run `build.sbt`

# Package

Run `sbt package` task

# Run

## Spark submit

`spark-submit --class TopDownSpecialization --master local target/scala-2.12/code_2.12-0.1.jar <pathToInputDataset> <pathToTaxonomyTree> <k>`

## Performance

|Records|k|Nodes|Partitions|Time (in ms)|
|---|---|---|---|---|
|32562|100|8|1|119371|
|32562|100|8|8|73119|
|32562|100|1|1|391149|


# Useful documentation

[Submitting Applications](https://spark.apache.org/docs/latest/submitting-applications.html)  
[Set up Apache Spark on a Multi-Node Cluster](https://medium.com/ymedialabs-innovation/apache-spark-on-a-multi-node-cluster-b75967c8cb2b)  
[Installing Spark Standalone to a Cluster](https://spark.apache.org/docs/latest/spark-standalone.html)