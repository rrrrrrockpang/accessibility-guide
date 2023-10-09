---
title: Instructions and Loggings
layout: default
parent: Computational Notebook Accessibility
nav_order: 3
permalink: /docs/notebook/instruction
---

# Instructions and Loggings
{: .fs-9 }

This section will show you how to add instructions and loggings to your computational notebooks.

## 1. Add Instructions.

When we create many Python scripts, the data folder, and the log folder, we add more complexity to the folder structure. Have a .md file that tells students what these scripts are doing as well as clear expectations (i.e., the Colab coding questions) of the activity. You can find the question.md file in my [GitHub screenshot]({{site.baseurl}}/docs/notebook/organize#2-divide-the-colab-document-into-separate-python-scripts).

We usually have the students submit the homework Colab assignment on canvas or Gradescope. It is much easier for BVI students to submit their answers on the .md file, instead of having to navigate multiple web platforms. 

## 2. Add Loggings.

We also recommend adding loggings to your computational notebooks and the Python scripts. This will be helpful for students to debug their code. 

When you have a `print` statement, you should also `log` these statements to a log folder. This is important for students with visual impairment to debug their code. When you print a lot of statements in the terminal, you cannot easily scroll up or copy-and-paste the terminal output for screen reader users. 

{: .note }
To log your output, please use the [logging package](https://docs.python.org/3/library/logging.html) and refer to this [blog post](https://towardsdatascience.com/stop-using-print-and-start-using-logging-a3f50bc8ab0). 


## 3. Below is an example of logging in Python. 

{: .note }
Note that we use `logger.info` to log the output. We include clear documentation of the question, housekeeping information, and step 1. The output is logged to `./log/section_1.log`. 

{: .note }
We also include an estimated running time for the key step. This is important for students with visual impairment to understand how long it takes to run the code, or they simply run into glitch in the server.


```python
# Question 1: How many titles of each type are in the IMDB dataset?
# Keywords: Dataframe API, SQL, group by, sort
# check ./log/section_1.log for the output

# Load libraries
import pyspark, logging
from pyspark.sql import *
from pyspark.sql.functions import *

## Housekeeping: setup code to read intermediate datasets
def script_filter(record):
    if record.name != __name__:
        return False
    return True
    
handler = logging.StreamHandler()
handler.filters = [script_filter]
logger = logging.getLogger(__name__)
logger.addHandler(handler)
fh = logging.FileHandler('./log/section_1.log', "w+")  # write to file
logger.setLevel(logging.INFO)
logger.addHandler(fh)

# Create a SparkSession
spark = SparkSession.builder.config("spark.driver.memory", "4g").getOrCreate()

# Load the datasets
Titles = spark.read.csv("data/title.basics.tsv", sep='\t', header=True)
Principals = spark.read.csv("data/title.principals.tsv", sep='\t', header=True)
## End of Housekeeping.

# This is the description in Google Colab as well.
# Step 1: IMDB lists many different kinds of media -- movies, video games, TV episodes, etc. Let's group the IMDB titles by titleType and count how many records exist belonging to each title type:
# The estimated running time is < 1 sec.
title_type_counts = Titles.groupBy("titleType") \
    .agg(count("*").alias("numTitles")) \
    .sort(desc("numTitles"))

# Log the output
logger.info("Step 1: {}".format(title_type_counts))
```
