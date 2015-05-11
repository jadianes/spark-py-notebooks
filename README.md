# Spark IPython Notebooks  

This is a collection of IPython notebooks intended to train the reader
in different Spark concepts, from basic to advance, by using the Python
language.  

## Instructions  

A good way of using these notebooks is by first cloning the repo, and then 
starting your own [IPython notebook](http://ipython.org/notebook.html) in 
**pySpark mode**. For example, if we have a *standalone* Spark installation
running in our `localhost` with a maximum of 6Gb per node assigned to IPython:  

    MASTER="spark://127.0.0.1:7077" SPARK_EXECUTOR_MEMORY="6G" IPYTHON_OPTS="notebook --pylab inline" ~/spark-1.2.1-bin-hadoop2.4/bin/pyspark

Notice that the path to the `pyspark` command will depend on your specific 
installation. So as requirement, you need to have
[Spark installed](https://spark.apache.org/docs/latest/index.html) in 
the same machine you are going to start the `IPython notebook` server.     

For more Spark options see [here](https://spark.apache.org/docs/latest/spark-standalone.html). In general it works the rule of passign options 
described in the form `spark.executor.memory` as `SPARK_EXECUTOR_MEMORY` when
calling IPython/pySpark.   
 
## Datasets  

We will be using datasets from the [KDD Cup 1999](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html).

## Notebooks  

The following notebooks can be examined individually, although there is a more
or less linear 'story' when followed in sequence. By using the same dataset
they try to solve a related set of tasks with it.  
 
### [RDD creation](nb1-rdd-creation/nb1-rdd-creation.ipynb)  

About reading files and parallelize.  
  
### [RDDs basics](nb2-rdd-basics/nb2-rdd-basics.ipynb)

A look at `map`, `filter`, and `collect`.  
  
### More on RDDs  

The rest of transformations and actions.  
  
### Working with key-value pairs  
  
### MLlib I  

Data types and basic statistics.  
  
### MLlib II   

Classification.  

### MLlib III   

Clustering and PCA.  


