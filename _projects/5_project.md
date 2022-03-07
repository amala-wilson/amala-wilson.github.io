---
layout: page
title: Comparative Evaluation of Finetuned Faster R-CNN Model on Low-light Images
#description: 
img: assets/img/cs256/cs256.png
importance: 1
category: work
---

---

Many state-of-the-art (SOTA) convolutional neural networks exist today due to the high availability of datasets. Research shows that the majority of the images in these datasets are visible light images. In fact, according to two researchers, only 2% of total images were low-light in successful public benchmark datasets such as PASCAL VOC, ImageNet and MS COCO. Human and object detection is important to recognize, detect and classify in low-light images just as it is important in visible-light images. For this purpose, my team and I examined the performance of a SOTA real-time object detection CNN called Faster R-CNN by incorporating it into different architectures which are constructed from a combination of image filters and another CNN called EnlightenGAN.

For our project, we decided to use the Faster R-CNN model provided by Detectron2, which is a Pytorch-based modular object detection library. The Faster R-CNN variation that we used consisted of ResNet50 as the backbone and a Feature Pyramid Network (FPN). The model was executed on an AWS EC2 instance with the Deep Learning Base AMI (Ubuntu 16.04) Version 19.3 that used the p2.xlarge GPU. In order to save on cost, Faster R-CNN was also executed on Google COLAB to run inference as well as finetune the model on our own custom dataset. Through transfer learning, we fine tuned the Faster R-CNN model using a combination of images from the Exclusively Dark dataset and our own set of low-light images. We used ImgLab to annotate our dataset in COCO format because Detectron2 supports this format. The second dataset was taken from COCO validation dataset. The other components that were used are two image filters, CLAHE and USM, and another CNN called EnlightenGAN.

Out of the set of architectures we used, the one that showed the high accuracy is when dark images were fed into EnlightenGAN and then the output of EnlightenGAN was fed into finetuned Faster R-CNN.

For more information, please refer to the report

{% pdf "/assets/pdf/cs256/CS256_ProjectReport.pdf" %}

and the GitHub repository for this project

{% linkpreview "https://github.com/ksheeraj/CS256-AI-ObjectDetection" %}

---
