# Spark SQL

Spark SQL允许Spark执行用SQL, HiveQL或者Scala表示的关系查询。这个模块的核心是一个新类型的RDD-[SchemaRDD](http://spark.apache.org/docs/latest/api/scala/index.html#org.apache.spark.sql.SchemaRDD)。
SchemaRDDs由[行](http://spark.apache.org/docs/latest/api/scala/index.html#org.apache.spark.sql.package@Row:org.apache.spark.sql.catalyst.expressions.Row.type)对象组成，行对象拥有一个模式（scheme）
来描述行中每一列的数据类型。SchemaRDD与关系型数据库中的表很相似。可以通过存在的RDD、一个[Parquet](http://parquet.io/)文件、一个JSON数据库或者对存储在[Apache Hive](http://hive.apache.org/)中的数据执行HiveSQL查询中创建。

本章的所有例子都利用了Spark分布式系统中的样本数据，可以在`spark-shell`中运行它们。

* [开始](getting-started.md)