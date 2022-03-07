---
layout: page
title: Survey on Anomaly Detection in Wireless Sensor Networks
#description: 
img: assets/img/cs268/cs268.png
importance: 1
category: work
---

---

The high availability of low cost sensors and capabilities of wireless sensor networks (WSNs) has given rise to a phenomenon known as Internet of Things (IOT), where everyday objects are turned into smart objects. A common example can be found in homes such as Nest thermostats or Alexa devices. With so many devices being connected to the Internet, the risk of transmitting and receiving erroneous information also increases. Processing erroneous data can lead to detrimental decisions which could cost an organization in the long-term. For this reason, it’s important and essential to detect anomalies within a WSN so that an efficient, secure and reliable network can be provided.

An anomaly is an inconsistent data point within a set of data and three main types of anomalies exist within a WSN: node, network and data anomalies. This project solely focuses on different methodologies on identifying data anomalies. More specifically, this project incorporated a statistical-based and clustering-based approach. A simulated version of a WSN was built using a SenseHat device that read environmental data (temperature, pressure, humidity) from its sensors and sent that data to IBM Bluemix, IBM’s cloud service, through a Raspberry Pi that was used as a gateway device for the transmission of data. The Raspberry Pi was connected to a Personal Hotspot to ensure that the sensor data can be transmitted to the cloud. The statistical-based, or Interquartile Range (IQR), method was implemented in the cloud using Node-Red to identify outliers. Due to limited resources, a temperate dataset from Kaggle was used to program the IQR method. Since the same dataset was used for both implementations, the accuracy of the results were determined by comparing the output values of both implementations and it turned out to be equal.


For more information, please refer the following [article](https://ieeexplore.ieee.org/document/8935827)

**Survey on Anomaly Detection in Wireless Sensor Networks (WSNs)**\
Chirayil, Amala, Maharjan, Rajendra, and Wu, Ching-Seh\
*20th IEEE/ACIS International Conference on Software Engineering, Artificial Intelligence, Networking and Parallel/Distributed Computing (SNPD) 2019*

---
