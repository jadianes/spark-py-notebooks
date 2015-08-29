# Spark Python Notebooks  

This is a collection of [IPython notebook](http://ipython.org/notebook.html)/[Jupyter](https://jupyter.org/) 
notebooks intended to train the reader on different [Apache Spark](http://spark.apache.org/) concepts, from 
basic to advanced, by using the **Python** language.  

If your are interested in being introduce to some basic Data Science
Engineering, you might find [these series of tutorials](https://github.com/jadianes/data-science-your-way)
interesting. There we explain different concepts and applications 
using Python and R.  

## Instructions  

A good way of using these notebooks is by first cloning the repo, and then 
starting your own [IPython notebook](http://ipython.org/notebook.html)/[Jupyter](https://jupyter.org/) in 
**pySpark mode**. For example, if we have a *standalone* Spark installation
running in our `localhost` with a maximum of 6Gb per node assigned to IPython:  

    MASTER="spark://127.0.0.1:7077" SPARK_EXECUTOR_MEMORY="6G" IPYTHON_OPTS="notebook --pylab inline" ~/spark-1.3.1-bin-hadoop2.6/bin/pyspark

Notice that the path to the `pyspark` command will depend on your specific 
installation. So as requirement, you need to have
[Spark installed](https://spark.apache.org/docs/latest/index.html) in 
the same machine you are going to start the `IPython notebook` server.     

For more Spark options see [here](https://spark.apache.org/docs/latest/spark-standalone.html). In general it works the rule of passign options 
described in the form `spark.executor.memory` as `SPARK_EXECUTOR_MEMORY` when
calling IPython/pySpark.   
 
## Datasets  

We will be using datasets from the [KDD Cup 1999](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html). The results 
of this competition can be found [here](http://cseweb.ucsd.edu/~elkan/clresults.html).  

## References

The reference book for these and other Spark related topics is:  

- *Learning Spark* by Holden Karau, Andy Konwinski, Patrick Wendell, and Matei Zaharia.  

## Notebooks  

The following notebooks can be examined individually, although there is a more
or less linear 'story' when followed in sequence. By using the same dataset
they try to solve a related set of tasks with it.  
 
### [RDD creation](https://github.com/jadianes/spark-py-notebooks/blob/master/nb1-rdd-creation/nb1-rdd-creation.ipynb)  

About reading files and parallelize.  
  
### [RDDs basics](https://github.com/jadianes/spark-py-notebooks/blob/master/nb2-rdd-basics/nb2-rdd-basics.ipynb)

A look at `map`, `filter`, and `collect`.  
  
### [Sampling RDDs](https://github.com/jadianes/spark-py-notebooks/blob/master/nb3-rdd-sampling/nb3-rdd-sampling.ipynb)  

RDD sampling methods explained.    
  
### [RDD set operations](https://github.com/jadianes/spark-py-notebooks/blob/master/nb4-rdd-set/nb4-rdd-set.ipynb)    

Brief introduction to some of the RDD pseudo-set operations.  

### [Data aggregations on RDDs](https://github.com/jadianes/spark-py-notebooks/blob/master/nb5-rdd-aggregations/nb5-rdd-aggregations.ipynb)  

RDD actions `reduce`, `fold`, and `aggregate`.   

### [Working with key/value pair RDDs](https://github.com/jadianes/spark-py-notebooks/blob/master/nb6-rdd-key-value/nb6-rdd-key-value.ipynb)    

How to deal with key/value pairs in order to aggregate and explore data.  
  
### [MLlib: Basic Statistics and Exploratory Data Analysis](https://github.com/jadianes/spark-py-notebooks/blob/master/nb7-mllib-statistics/nb7-mllib-statistics.ipynb)    

A notebook introducing Local Vector types, basic statistics 
in MLlib for Exploratory Data Analysis and model selection.  
  
### [MLlib: Logistic Regression](https://github.com/jadianes/spark-py-notebooks/blob/master/nb8-mllib-logit/nb8-mllib-logit.ipynb)     

Labeled points and Logistic Regression classification of network attacks in MLlib.
Application of model selection techniques using correlation matrix and Hypothesis Testing.    

### [MLlib: Decision Trees](https://github.com/jadianes/spark-py-notebooks/blob/master/nb9-mllib-trees/nb9-mllib-trees.ipynb)  

Use of tree-based methods and how they help explaining models and
 feature selection.  

### [Spark SQL: structured processing for Data Analysis](https://github.com/jadianes/spark-py-notebooks/blob/master/nb10-sql-dataframes/nb10-sql-dataframes.ipynb)  

In this notebook a schema is inferred for our network interactions dataset. Based on that, we use
Spark's SQL `DataFrame` abstraction to perform a more structured exploratory data analysis.  


## Applications  

Beyond the basics. Close to real-world applications using Spark and other technologies.  

### [An on-line movie recommendation service using Spark & Flask](https://github.com/jadianes/spark-movie-lens)  

A two part tutorial + Python scripts to run your own scalable movie recommendation service using Spark and Flask.  

### [Olssen: On-line Spectral Search ENgine for proteomics](http://olssen.github.io/)  

Same tech stack this time with an AngularJS client app.  

### [KDD Cup 1999](https://github.com/jadianes/kdd-cup-99-spark)  

My try using Spark with this classic dataset and Knowledge Discovery competition.  



