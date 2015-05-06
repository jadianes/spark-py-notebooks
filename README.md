# Spark IPython Notebooks  

This is a collection of IPython notebooks intended to train the reader
in different Spark concepts, from basic to advance, by using the Python
language.  

## Instructions  

A good way of using these notebooks is by first cloning the repo, and then 
starting your own [IPython notebook](http://ipython.org/notebook.html) in 
**pySpark mode**. For example, if we have a *standalone* Spark installation
running in our `localhost`:  

    MASTER=spark://127.0.0.1:7077 IPYTHON_OPTS="notebook --pylab inline" ~/spark-1.2.1-bin-hadoop2.4/bin/pyspark

Notice that the path to the `pyspark` command will depend on your specific 
installation. So as requirement, you need to have
[Spark installed](https://spark.apache.org/docs/latest/index.html) in 
the same machine you are going to start the `IPython notebook` server.     

## Datasets  

We will be using datasets from the [KDD Cup 1999](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html).

## Notebooks  

1. [RDD creation](http://nbviewer.ipython.org/github/jadianes/spark-py-notebooks/blob/master/nb1-rdd-creation/nb1-rdd-creation.ipynb): reading files and parallelize.  
2. RDDs basics: map, filter, collect.  
3. More on RDDs: the rest.  
4. Working with key-value pairs.  


