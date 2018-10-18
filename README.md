# English Wikipedia Page Traffic Dec. 2007 - Sept. 2018

![image](https://github.com/mag3141592/data-512-a1/blob/master/en-wikipedia_traffic_2000712-201809.png)  

## Goal
This repository contains all files required for Human Centered Data Science's (DATA 512) "Assignment 1: Data Curation." The objective of this project is to retrieve, clean, and analyize English Wikipedia's page traffic. This project is intended to be fully reproducible, with more information available [here](https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018)/Assignments#A1:_Data_curation).

This project will walk you through accessing Wikimedia's REST APIs and retrieving 5 source files. Next, the data is cleaned and aggegrated to produce our final vizualition above and [cleaned data output](https://github.com/mag3141592/data-512-a1/blob/master/en-wikipedia_traffic_200712-201809.csv).

## Directory
> data-512-a1/
>> data/... >> Contains 5 .json files containing the raw API response data. <br/>
>> LICENSE  >> A standard MIT license. <br/>
>> README.md >> What you're currently reading. <br/>
>> en-wikipedia_traffic_2000712-201809.png >> The final visualization. <br/>
>> en-wikipedia_traffic_2000712-201809.csv >> The cleaned data. <br/>
>> hcds-al-data-curation.ipnb >> The source code. <br/>

## Data Acquisition
This project leverages two Wikimedia REST API endpoints:
* The [Legacy Pagecounts API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts) provides access to Dec.2007 through Jul. 2016 desktop and mobile traffic data. [Endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)
* The [Pageviews API]() accesses data from Jul. 2015 for desktop, mobile-app, mobile-web. [Endpoint]()

The Legacy Pagecounts API access the old definition page views, while Pageviews API accesses the new definition. This new definiton of page traffic eliminates counts of web crawlers. Addtionally, Pageviews API breaksdown the mobile traffic by mobile-web and mobile-app. However, in cleaning the data we aggregate to a total mobile monthly traffic count.

Please also refer to the Wikimedia Foundation REST API terms of use [here](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions). This data is available under the CC0 1.0 license. 

## Output
The cleaned data can be found in [en-wikipedia_traffic_200712-201809.csv](https://github.com/mag3141592/data-512-a1/blob/master/en-wikipedia_traffic_200712-201809.csv). It consists of 130 rows (excluding header) and 8 colums.
The columns have the following format:
* year = year(YYYY)
* month = month(MM)
* pagecount_all_views = number
* pagecount_desktop_views = number
* pagecount_mobile_views = number
* pageviews_all_views = number
* pageviews_desktop_views = number
* pageviews_mobile_views = number

## Reproducibility
Again, this work is intended to be fully reproducible. This can be done by accessing the source [code](https://github.com/mag3141592/data-512-a1/blob/master/hcds-a1-data-curation.ipynb) and running the notebook. 

### Caution:
* My data was retrieved 10/17 and values are subject to change in the future.
