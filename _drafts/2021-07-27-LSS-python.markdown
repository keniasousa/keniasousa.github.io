---
layout: post
title: "Lean Six Sigma with Python"
date: 2021-07-27 12:00:00 +0200
categories: lean six sigma, python 
---

T

<!-- more -->

Steps:

1. Install the Python libraries in PyCharm

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

2. Read the file

I have requested to export my running data from Strava and received a CSV file.

def read_file(df):
    df = pd.read_csv(file, index_col=0)
    return df

file = "export_45061253/activities.csv"
df = read_file(file)
print(df)

3. Understand the data
Identify the data fields available in the data set.
This data set lists the running activities logged from my Garmin watch.

What are the categorical (use for grouping) and continuous data (use to measure)? 
Categorical data:
I can group the data using the categorical data, such as activity name and activity type. I can also organize it in a timeline with activity date.
Since I only run, activity type has no use in my data set.
Continuous data:
The watch has logged Elapsed Time, distance, moving time, max speed, average speed, elevation high, elevation low, average cadence (steps per minute), and calories.

4. Identify what is your goal
It's important to be aware of your goal before you start analyzing your data and clearly define a question.
I am preparing for a half marathon and I want to understand: how is my running performance?
I've set my target as 21km and the least I should go out to train is 5km (that's the lower specification limit). The upper specification limit for training is 15km because the orientation I have is to train up to 75% of the target distance. 

5. Identify key data fields to answer your question
I'm interested in analyzing elapsed time, moving time, distance, max speed and calories. 
One important metric that is missing is pace that we can calculate with the running time  (called moving time in this data set) divided by the distance.
The pace is represented in min/km. Since the running time is logged in seconds, I divided by 60 to measure it in minutes.
Pace = (Running time (in seconds))/60 / Distance

6. Analyze what the data tells you
We can start looking at summary statistics, such as minimum value, maximum value, range, mean, median. 
Median represents the value at the middle of the distribution and mean is the average of the dataset.
For distance, my mean is almost 6km, which is above my lowest requirement for a running workout. However it is still quite low compared to my target of 21km. I need to start running between 10km and 15km to prepare for a half-marathon.
The range is quite wide, which is 10km, showing me that there are runs below 1km. In this case, they shouldn't be even counted, the lowest I should have is 3km even though it is below my required specification. 16% of the runs are below 5km, let's look if there are many below 1km, which I consider a wrong entry. I must have clicked on the watch by mistake. However, there is only one below 1km that seems to have been logged by mistake with only 200m.
We can also analyze the standard deviation and variance.
cccccccc

How did I do comparing the time I did the activity? Did I do longer distances in the morning, afternoon or evening?
The one I did the longest distance was during a morning run, but also when I did one of the lowest distances. It has the highest variability. And the afternoon run has some outliers below the lower specification limit.

References:

Matplotlib histogram:
https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html

Matplotlib colors:
https://matplotlib.org/stable/gallery/color/named_colors.html

Use of colors in histogram from Stack overflow:
https://stackoverflow.com/questions/58972548/plot-histogram-using-python-with-different-colors-for-positive-and-negative-valu

