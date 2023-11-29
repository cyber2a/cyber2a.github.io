+++
title = "A Framework for Building and Finetuning Geospatial Foundation Models"
date = "2023-11-13T12:00:00-05:00"
tags = ["Geospatial foundation model"]
descriptions = [
    "Speakers:", 
    "Daniela Szwarcman, IBM Research",
    "Paolo Fraccaro, IBM Research"
]
banner = "img/banners/gfm-webinar.jpg"
logo = "img/pathfinders.png"

videoEmbed = "https://www.youtube.com/embed/E09KAyFLjBo"
video = "https://www.youtube.com/watch?v=E09KAyFLjBo"

register="https://asu.zoom.us/webinar/register/WN_XdJKEbmZQ0SqWKQNGcyhOw#/registration"

summary = '''Foundation models are artificial intelligence (AI) models that are pre-trained on large unlabeled datasets through self-supervision and then fine-tuned for different downstream tasks. There is increasing interest in the scientific community to investigate whether this approach can be successfully applied to domains beyond natural language processing and computer vision to effectively build generalist AI models that make use of different types of data. Here, IBM and NASA present the first end-to-end framework for pre-training and fine-tuning foundation models efficiently from a large source of geospatial data. We have implemented and applied this framework to produce Prithvi, a geospatial foundation model pre-trained on multispectral satellite imagery from the NASA Harmonized Landsat-Sentinel 2 (HLS) dataset. The framework supports automated statistical smart sampling strategies based on whether, land cover and other datasets to maximize impact and minimize waste of resources (e.g. avoiding areas and time ranges that would not bring any new information). 
'''
    
+++

![flyer](/img/banners/gfm-webinar.jpg)
--------------------------------------


Foundation models are artificial intelligence (AI) models that are pre-trained on large unlabeled datasets through self-supervision and then fine-tuned for different downstream tasks. There is increasing interest in the scientific community to investigate whether this approach can be successfully applied to domains beyond natural language processing and computer vision to effectively build generalist AI models that make use of different types of data. Here, IBM and NASA present the first end-to-end framework for pre-training and fine-tuning foundation models efficiently from a large source of geospatial data. We have implemented and applied this framework to produce Prithvi, a geospatial foundation model pre-trained on multispectral satellite imagery from the NASA Harmonized Landsat-Sentinel 2 (HLS) dataset. The framework supports automated statistical smart sampling strategies based on whether, land cover and other datasets to maximize impact and minimize waste of resources (e.g. avoiding areas and time ranges that would not bring any new information). Prithvi is a Temporal Vision Transformer that includes positional and temporal embeddings, which was trained on IBM Cloud Vela cluster (NVIDIA A100 GPUs) using a Masked Auto Encoder approach and Mean Squared Error loss function for a total of 10k GPUs hours. We demonstrated using the fine-tuning workflows built in our framework that Prithvi could be successfully fine-tuned to produce state-of-the-art AI models for Earth observation tasks: flood mapping, burn scar identification and multi-temporal crop classification. We carefully studied the impact of Prithvi's pre-trained weights on the downstream tasks by comparing learning curves for 1) fine-tuning the whole model, 2) fine-tuning only the downstream task decoder, 3) training the model without taking advantage of Prithvi's pre-trained weights. Furthermore, given the scarcity of labeled data for Earth observation tasks, we progressively decreased the amount of labeled data available for fine-tuning the model to assess data efficiency. This analysis showed that using Prithvi we could achieve peak performance on test data quicker and with less training data (i.e. up to 50% less). Finally, in order to increase the impact of this work, the pre-trained model and fine-tuning workflows have been made publicly available through Hugging Face ([https://huggingface.co/ibm-nasa-geospatial](https://huggingface.co/ibm-nasa-geospatial)).
