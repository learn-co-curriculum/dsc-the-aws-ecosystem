# The AWS Ecosystem

## Introduction

In this lesson, we'll get set up to use **_Amazon Web Services_**, and then get to know our way around the platform. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/awscloud.svg'>

## Objectives 

- Set up an AWS account and explore the Amazon Resource Center 
- Explain what the "regions" are in AWS and why it is important to choose the right one
- Explain the purpose of AWS IAM


## Getting Started

Before we can begin exploring everything AWS has to offer, we'll need to create an account on the platform. To do this, start by following this link to [Amazon Web Services](https://aws.amazon.com/). While you're there, you may want to take the time to bookmark it -- chances are this is a website you'll use frequently in your career as a data scientist!

### Will This Cost Money?

Although you will need a credit card to register for AWS, working through this section will not cost any money. AWS provides a free tier for learning and prototyping on the platform -- this is the tier we'll use for everything going forward. As long as you correctly register for the free tier, this will not cost you any money. 

### Register Your Email

Begin by clicking the "Sign Up" button in the top right-hand corner of the page. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-1.png'>

Next, create an account by adding your email and password. You'll also need to set an **_AWS Account Name_**. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-2.png'>

On the next screen, enter your contact information. **_Make sure you set your account type to 'Personal'!_** 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-3.png'>

This next page is especially important -- be sure to select the **_Basic Plan_**! As a reminder, you will be asked to enter a credit card number during the next few steps. Although we will only be making use of the free tier of services for AWS, be aware that you will still need to enter a credit card number in order to complete the registration process. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-4.png'>

Now that you're all signed up, click the "Sign in to the Console" button to actually enter the AWS Console. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-5.png'>

Great, you've now created an AWS Account! Let's take a look around. 

## The AWS Console

Now that you're signed in, you'll see the **_AWS Console_**. This is your "home screen" for AWS -- it allows you to quickly navigate through the thousands of services offered on AWS to find what you need. The easiest way to find what you need is the "Find Services" search bar at the top of the body of the page. 

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-6.png'>

You can also click the "See All Services" dropdown to see a full list of services you can use in AWS. There are **a ton** of services, but don't let yourself get overwhelmed -- you'll probably never end up using the vast majority of these, as only a few apply to the work of a data scientist.

## A Note on Regions

### AWS Regions

AWS has data centers all over the world, and they are **not** interchangeable when it comes to your projects. Check out [this link](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/) to see a list of all of the current AWS regions across the globe. While it typically won't matter for your projects in this program, the different AWS regions vary in terms of latency, cost, legal compliance, and features.

Each AWS region is a separate geographic area and is designed to be completely isolated from the other regions. This helps achieve the greatest possible fault-tolerance and stability. Communication between regions is possible, but often costs money and/or requires additional security configuration.

### Implications for Your Projects

It is **_very important_** that you always choose the same region to connect to with your projects. Resources are not automatically replicated across regions! One of the most common mistakes newcomers to AWS make is thinking they've lost their project because they are connected to a different data center and don't realize it. We'll remind you of this again later, but it can't hurt to say it twice: always make sure you're connected to the correct data center! This goes doubly for when you're creating a new project. 

## AWS IAM

IAM stands for [Identity and Access Management](https://aws.amazon.com/iam/). AWS allows IT administrators to configure access to different services at a very granular level, which can get intimidating pretty quickly!

Essentially all you need to know is that access to services requires you to create a **role** in IAM, and then set a **policy** for that role's access permissions. In some cases, e.g. you want to run a cloud notebook in [AWS SageMaker](https://docs.aws.amazon.com/sagemaker/latest/dg/security-iam.html), that role should be restricted to just you, and you should have permission to take any action. In other cases, e.g. you want to store data in an [S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-overview.html), you might want to allow anyone to download the data, but only allow yourself to upload.

In our curriculum examples we'll advise on IAM settings, but you'll likely need to do your own research as you explore beyond these for your own projects. Luckily these are public projects so the risk of leaking data or models is low. In a job setting, make sure you consult with your IT team to make sure that you are not revealing private data.

## Using the Amazon Resource Center

As platforms go, you won't find many with more options than AWS. It has an amazing amount of offerings, with more getting added all the time. While AWS is great for basic use cases like hosting a server or a website, it also has all kinds of different offerings in areas such as Databases, Machine Learning, Data Analytics and other areas useful to Data Scientists.

It's not possible for us to cover how to use every service in AWS in this section -- but luckily, we don't need to, because Amazon already has! The [Getting Started Resource Center](https://aws.amazon.com/getting-started/) contains a ton of awesome tutorials, demonstrations, and sample projects for just about everything you would ever want to know about any service on AWS. We **_strongly recommend_** bookmarking this page, as the tutorials they offer are very high quality, and free!

<img src='https://github.com/learn-co-curriculum/dsc-the-aws-ecosystem/raw/master/images/aws-7.png'>

## Summary

In this lesson, we signed up for Amazon Web Services and explored some of the different options on the platform. 
