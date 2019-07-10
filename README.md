# Overview
This guide shows you how to deploy a solution demonstrating how AWS services can be used to interrogate the Enron email corpus made public by the FBI after the company was found to be commiting massive fraud in the US.

The architecture makes use of the following AWS services:

- Sagemaker Notebooks for cleaning and preparing data
- Comprehend for entity extraction and sentiment analysis
- Elasticsearch and Kibana for storing, querying and visualising the enriched data
- Neptune to store graph data
- Tom sawyer (a partner product) for graph visualisation and add-hoc queries

To set the scene on the demo see the following video.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/-w6duQhWuVk/0.jpg)](https://www.youtube.com/watch?v=-w6duQhWuVk)

# Deployment guide

Deploy the CF template. This will setup the infrastructure ready to import the backups.

Once the termplate has deployed you have to make a change to the ES cluster to integrate Kibana with Cognito. Sadly this isn't yet support by Cloudformation.

Open the ES tab in the console, select the enron cluster and click **Configure Cluster**.

Check the **Enable Amazon Cognito for Authentication**. enter the following details.

![Alt text](/images/cognito.png?raw=true)
