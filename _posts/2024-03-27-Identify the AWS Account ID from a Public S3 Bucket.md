---
title: 'Identify the AWS Account ID from a Public S3 Bucket'
date: 2024-03-27
permalink: /posts/2024/02/AWS Cloud pentest/
tags:
  - Vulnerability
  - OWASP TOP 10
  - cloud security
---
#Identify the AWS Account ID from a Public S3 Bucket
Scenario

In a world increasingly reliant on cloud technologies, the ability to expose and leverage even the smallest oversights has become a coveted skill. Amidst this backdrop, a leading tech enterprise has reached out to your specialized cyber team for assistance and have provided the IP address of their website. Your objective? Use this IP to pinpoint their AWS account ID via a public S3 bucket so we can commence the process of enumeration.

Before going to Enumerate We first need to know what is AWS Account ID
AWS account ID looks like unique Identifier associated with 12-digit alphanumeric string in AWS (Amazon Web Services).

    arn: This indicates that it's an Amazon Resource Name.
    aws: Denotes that it's an AWS resource.
    iam: Indicates that the resource is an IAM (Identity and Access Management) resource.
    123456789127: This is the AWS account ID associated with the IAM role.
    role/dev: This is the name of the IAM role. It seems to be named "dev" within the account.



