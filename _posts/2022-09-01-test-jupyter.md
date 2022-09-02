---
title: "Test Jupyter"
last_modified_at: 2022-03-09T16:20:02-05:00
categories:
  - Blog
tags:
  - Post Formats
  - readability
  - standard
---

```python
import pyspark
import os
import boto3
```


```python
s3 = boto3.resource('s3')
```


```python
for bucket in s3.buckets.all():
    print(bucket.name)
```

imgentrybucket
    

```python
from pyspark.sql import SparkSession
from pyspark import SparkContext
```


```python
SparkContext() 
```





<div>
    <p><b>SparkContext</b></p>

    <p><a href="http://DESKTOP-G0D1OGF:4040">Spark UI</a></p>

    <dl>
      <dt>Version</dt>
        <dd><code>v3.2.0</code></dd>
      <dt>Master</dt>
        <dd><code>local[*]</code></dd>
      <dt>AppName</dt>
        <dd><code>pyspark-shell</code></dd>
    </dl>
</div>





```python
spark = SparkSession.builder.appName("Imgpreprocess").getOrCreate()
```


```python
os.getcwd()
```



'c:\\Users\\Guillaume\\Documents\\Projet 8'




```python
os.listdir(os.getcwd())
```




    ['fruits-360-original-size',
     'fruits-360-original-size.zip',
     'pyspark_preprocess.ipynb',
     'test_vs.py']




```python
os.listdir(os.path.join(os.getcwd(),"fruits-360-original-size"))
```




    ['Meta', 'Papers', 'readme.md', 'Test', 'Training', 'Validation']




```python
directory = "C:/Users/Guillaume/Documents/Projet 8/fruits-360-original-size/Training/eggplant_violet_1"
```


```python
spark.read.format("image").load(os.path.join(directory,"r0_0.jpg"))
```




    DataFrame[image: struct<origin:string,height:int,width:int,nChannels:int,mode:int,data:binary>]




```python

```
