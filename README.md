# Datenanalyse mit Apache Spark

Dieses Modul erstellt ein Spark-Cluster zur Analyse von Daten.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/b-oern/daw-spark)

Lokal ausführen:
```
docker-compose up
```

## Beispiele in Python

```
from pyspark.sql import SparkSession
spark = SparkSession.Builder().master('spark://172.18.0.3:7077').appName("SparkByExamples.com").getOrCreate()
data_list = ["a", "b", "c", "d", "e", "f", "g", "h"]
list_rdd = spark.sparkContext.parallelize(data_list)
list_rdd.first()
```

## Forken

Die GitPod-URL muss in der README.md angepasst werden.
