# Scaling Data Workloads Using the Best of Best Worlds: pandas and Spark

PyData Seattle 2023

Co-presented with [@HyukjinKwon](https://github.com/HyukjinKwon)

**Abstract**
<br>

It is indisputable that pandas is oftentimes the keystone element in any data wrangling and analysis workloads. However, the challenge is that pandas is not meant for big data processing. This presents data practitioners a dilemma: should we downsample data and lose information? Or should we explore a distributed processing framework to scale out data workloads? An example of a mainstream distributed processing tool is Apache Spark. However, this means data practitioners now have to learn a new language, PySpark. Not all is bleak though: pandas API on Spark provides pandas equivalent APIs in PySpark. It allows pandas users to transition from single-node to distributed environment, by just simply swapping the pandas package with pyspark.pandas.

On the other hand, existing PySpark users may wish to write their own custom user-defined functions (UDFs) that are not included in existing PySpark API. Pandas Function APIs, newly included in Spark 3.0+, allow users to apply arbitrary Python native functions, with pandas instances as the input and output against a PySpark dataframe. For instance, data scientists could use pandas function API to train a ML model based on each group of data using a single line of code.

Co-presented by both a top open-source Apache Spark commiter and a hands-on data science consultant, this talk equips data analysts and scientists with the knowledge of scaling their data analysis workloads with implementation details and best practice guidance. Working knowledge of pandas, basic Spark, and machine learning is helpful.
