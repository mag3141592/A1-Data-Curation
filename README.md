### English Wikipedia Page Traffic Dec. 2007 - Sept. 2018

## Goal
This repository contains all files required for Human Centered Data Science's (DATA 512) "Assignment 1: Data Curation." The objective of this project is to retrieve, clean, and analyize English Wikipedia's page traffic. This project is intended to be fully reproducible, with more information available [here](https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018)/Assignments#A1:_Data_curation).
<center> https://github.com/mag3141592/data-512-a1/blob/master/en-wikipedia_traffic_2000712-201809.png <center>
## Directory

## Data Acquisition
This project leverages two Wikimedia REST API endpoints:
* The [Legacy Pagecounts API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts) provides access to Dec.2007 through Jul. 2016 desktop and mobile traffic data. [Endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)
* The [Pageviews API]() accesses data from Jul. 2015 for desktop, mobile-app, mobile-web. [Endpoint]()

The Legacy Pagecounts API access the old definition page views, while Pageviews API accesses the new definition. This new definiton of page traffic eliminates counts of web crawlers. mobile-app + mobile-web

Please also refer to the Wikimedia Foundation REST API terms of use [here](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions). This data is available under the CC0 1.0 license. 

## Output
The cleaned data 

## Reproducibility


--Data retrieved 10/17 values may change
