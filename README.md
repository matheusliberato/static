# Before You Begin

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




