## Overview

This project set up a jenkins CI to upload a HTML page from GitHub to Amazon S3 Bucket
by configuring all necessary stage and steps in Jenkinsfile.

## Before You Begin

Please make sure you have the following in place before you begin your project:

* **Software Requirements:** Latest Jenkins available and “tidy” linter
* **Cloud Requirements:** AWS Account, IAM username and password, EC2 Key pair
* **Github:** A personal GitHub repository

## Outline of this Project

We provide you some general guidance below to successfully complete the project. For many of the steps you will also need to apply what you've learned in the course.

Here is the outline of the steps you will take, which match the headers of the sections on the *Project Details* page:

* AWS Steps
* Install Jenkins On Ubuntu
* Set Up Jenkins
* Install required plugins
* Set up GitHub
* Set up AWS credentials in Jenkins
* Set up S3 Bucket
* Set up pipeline for AWS
* Add another stage in pipeline


In *AWS Steps* we create a group with permissions to manage AWS VPC (*AmazonVPCFullAccess*), EC2 (*AmazonEC2FullAccess*) and S3 (*AmazonS3FullAccess*). After that, we create a user and put him in the group created before. We also create a security group with inbound and outbound rules to be used by our EC2 instances.

After that we launch an EC2 instance running Ubuntu Server 18.04 and install and configure Jenkins on it, which include the installation of additionals plugins like *Pipeline: AWS Steps* and *BlueOcean Agregator*.

We create a S3 Bucket with public access and set jenkins to upload a index.html from github to S3 Bucket via Jenkinks pipeline.

## License

**Note:** All files in this repository that were made by me, which includes scripts and configuration files, are under MIT License. However, it might use third-party softwares each one with their own license. Please, check it out.

MIT License

Copyright (c) [2019] [[Matheus Liberato]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWA




