# Overview
This guide shows you how to deploy a solution demonstrating how AWS services can be used to interrogate the Enron email corpus made public by the FBI after the company was found to be commiting massive fraud in the US.

The architecture makes use of the following AWS services:

- Sagemaker Notebooks for cleaning and preparing data
- Comprehend for entity extraction and sentiment analysis
- Elasticsearch and Kibana for storing, querying and visualising the enriched data
- Neptune to store graph data
- Tom sawyer (a partner product) for graph visualisation and add-hoc queries

To set the scene on the demo see the following video.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/-w6duQhWuVk/0.jpg)](https://www.youtube.com/watch?v=-w6duQhWuVk){target="_blank"}

# Deployment guide
