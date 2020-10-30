+++
title = "a. Services & Architecture"
date = 2019-09-18T10:46:30-04:00
weight = 40
tags = ["tutorial", "IAM", "ParallelCluster", "Serverless"]
+++

Here are a few more details on what you will be deploying and the services you will be using.


#### Services used during this lab

In this lab we combine the following services:

- [AWS ParallelCluster](https://docs.aws.amazon.com/parallelcluster/index.html) enables you to create an HPC system in AWS.
- [AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/getting-started.html) are serverless functions in AWS.
- [AWS Systems Manager (SSM)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html) to execute the user commands through a secure channel without granting direct SSH access nor exposing the nodes.
- [Amazon API Gateway](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html) provides the API interface to your Lambda Function.
- [AWS Identity and Access Management (IAM)](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html) manages what or who can conduct an action on a resource. For example for Lambda to connect to SSM.


#### Architecture Diagram

Below is the serverless architecture which shows the components required to create the cluster and interact with the solution

![Serverless Architecture](/images/serverless/serverless-arch2.png)