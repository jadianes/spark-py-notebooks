# A scalable on-line movie recommender using Spark and Flask  

###### This tutorial-application has now [its own repository](https://github.com/jadianes/spark-movie-lens), where its evolution should continue.  

This Apache Spark tutorial will guide you step-by-step into how to use the [MovieLens dataset](http://grouplens.org/datasets/movielens/) to build a movie recommender using [collaborative filtering](https://en.wikipedia.org/wiki/Recommender_system#Collaborative_filtering) with [Spark's Alternating Least Saqures](https://spark.apache.org/docs/latest/mllib-collaborative-filtering.html) implementation. It is organised in two parts. The first one is about getting and parsing movies and ratings data into Spark RDDs. The second is about building and using the recommender and persisting it for later use in our on-line recommender system.    

This tutorial can be used independently to build a movie recommender model based on the MovieLens dataset. Neither the use of this dataset nor the use of this algorithm are new (I recommend you for example this [EdX course](https://www.edx.org/course/introduction-big-data-apache-spark-uc-berkeleyx-cs100-1x) or [Google](https://www.google.co.uk/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=movielens%20dataset%20collaborative%20filtering)), and this is because we put the emphasis on ending up with a usable model in an on-line environment, and how to use it in different situations. The second part of the tutorial explains how to use Python/Flask for building a web-service on top of Spark models. By doing so, you will be able to develop a complete **on-line movie recommendation service**.  

## Part I: [Building the recommender](https://github.com/jadianes/spark-py-notebooks/blob/master/movie-lens-recommender/notebooks/building-recommender.ipynb)  

## Part II: [Building and running the web service](https://github.com/jadianes/spark-py-notebooks/blob/master/movie-lens-recommender/notebooks/online-recommendations.ipynb)  

## Quick start  

The file `server/server.py` starts a [CherryPy](http://www.cherrypy.org/) server running a 
[Flask](http://flask.pocoo.org/) `app.py` to start a RESTful
web server wrapping a Spark-based `engine.py` context. Through its API we can 
perform on-line movie recommendations.  

Please, refer the the [second notebook](https://github.com/jadianes/spark-py-notebooks/blob/master/movie-lens-recommender/notebooks/online-recommendations.ipynb) for detailed instructions on how to run and use the service.  


