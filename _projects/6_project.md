---
layout: page
title: Business Context Aware Data Center Monitoring
#description: 
img: assets/img/cs274/cs274.png
importance: 1
category: work
---

---

Ecommerce applications, which are built using a series of technologies, help businesses to use the Internet to conduct their business processes online. These ecommerce applications can either be found deployed in a private data center or the cloud. It’s important for businesses to proactively monitor the data center in which their application is deployed in because any data center downtime can lead a business to lose hundreds of thousands of dollars. In fact, according to a white paper written by Emerson, the average cost of data center downtime was approximately $5,600 per minute. To prevent businesses from losing money, it’s imperative to monitor data centers. System log data can be collected over a period of time to analyze the patterns of computation and storage, which are essential resources needed to execute ecommerce applications and others. By analyzing and recognizing how much compute, storage and network resources are being used over a period of time, we can predict what kind of situations arise so that appropriate maintenance can be done before the application stops running. For this purpose, I incorporated ElasticSearch, Beats, Kibana, and 2 machine learning (ML) models (Standard Logistic Regression and Multinomial Logistic Regression).

System and database log data were collected using Filebeat and Metricbeat, which are lightweight data shippers that are used to capture operational data. Metricbeat was used to collect system performance metric data from my local system. Filebeat was used to collect log data from MongoDB which was utilized in an ecommerce application that I found online. This data is then stored in inverted indices within Elasticsearch, which is a distributed search and analytics engine for all types of data. Essential data was extracted with the help of APIs to prepare training and testing datasets for the ML models. I trained two standard logistic regression models, one for CPU usage and another one for memory usage, using a dataset from GWA-T-12 Bitbrains distributed data center that consisted of performance metrics of 1,750 virtual machines. After testing this model on my local system data, the memory model was able to only achieve 28% accuracy. The CPU model was able to achieve 98% accuracy. The multinomial logistic regression model was trained on a dataset that consisted of performance metrics of a MongoDB database. This model was able to achieve 69% accuracy. Kibana was used as a visualization tool to view my local system in real-time.


For more information, please refer to the report

{% pdf "/assets/pdf/cs274/CS274_Report.pdf" %}

and the GitHub repository for this project

{% linkpreview "https://github.com/amala-wilson/CS274_Project" %}

---
