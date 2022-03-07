---
layout: page
title: Privacy Preserving for Multiple Computer Vision Tasks
#description: 
img: assets/img/cs298/cs298.png
importance: 1
category: work
---

---

Privacy-preserving visual recognition is an important area of research that is gaining momentum in the field of computer vision. In a production environment, it is critical to have neural network models learn continually from user data. However, sharing raw user data with a server is less desirable from a regulatory, security and privacy perspective. 

Federated learning addresses the problem of privacy-preserving visual recognition. More specifically, we closely examine and dissect a framework known as Dual User Adaptation (DUA) presented by Lange et al. at CVPR 2020, due to its novel idea of bringing about user-adaptation on both the server-side and user device side. Data in the server and user device is predefined into a series of tasks prior to training and testing. However, since user data is constantly evolving, it’s important to see how DUA performs on unseen data or tasks. A few implementations are also executed to see if the performance of the DUA model can be improved on unseen data. In addition, two other federated learning frameworks are implemented to compare how it performs with DUA. 

Through this research we show that retraining the classifier layer of the merged model with all data categories greatly improves the performance for real-world implementation of DUA.

For more information, please refer to the report of my M.S. writing project.

{% pdf "/assets/pdf/cs298/cs298_report.pdf" %}

---
