# bikesharing
Tableau

<p align="left">
  <img src="images/2011_surfing.png" width="100">
</p>

## Table of Contents
* [Overview](https://github.com/rkaysen63/bikesharing/blob/master/README.md#overview)
* [Resources](https://github.com/rkaysen63/bikesharing/blob/master/README.md#resources)
* [Results](https://github.com/rkaysen63/bikesharing/blob/master/README.md#results)
* [Summary](https://github.com/rkaysen63/bikesharing/blob/master/README.md#summary)
* [Code](https://github.com/rkaysen63/bikesharingblob/master/README.md#code)

## Overview:

## Resources 

* Data: https://www.citibikenyc.com/system-data
* Tools: 
  * Tableau
  * Jupyter Notebook
  * Python import Pandas
* Lesson Plan: UTA-VIRT-DATA-PT-02-2021-U-B-TTH, Module 14 Challenge
* Acknowledgements:
  * Des Moines Skyline Photo from:  https://en.wikipedia.org/wiki/Downtown_Des_Moines#/media/File:Skyline_downtown_Des_Moines.jpg
  * Attributed to By BarbaraLN - Flickr: Skyline, CC BY-SA 2.0, https://commons.wikimedia.org/w/index.php?curid=17089434

## Results:



## Summary:

## Code:
1. Create a DataFrame for the 201908-citibike-tripdata data.

        import pandas as pd

        # File to Load 
        citibike_data_to_load = "Resources/201908-citibike-tripdata.csv"
        citibike_df.head()

***Insert photo of dataframe here

2. Check the datatypes of your columns. 

        citibike_df.dtypes

***insert photo of dtypes here.

3. Convert the 'tripduration' column to datetime datatype.

        citibike_df['tripduration_dtobj'] = pd.to_datetime(citibike_df['tripduration'], unit='s')
        citibike_df.head()

***Insert photo of dataframe2 here

4. Check the datatypes of your columns. 

        citibike_df.dtypes
        
***insert photo of dtypes2 here.        
        
5. Export the Dataframe as a new CSV file without the index.

        citibike_df.to_csv("Resources/201908_citibike_tripdata_revised.csv", index=False)      
        

[Back to the Table of Contents](https://github.com/rkaysen63/bikesharing/blob/master/README.md#table-of-contents)
