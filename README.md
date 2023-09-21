# Learn-AWS

> ### Topics Covered

> - Hypervisor
> - Servers
> - User (Authentication, Authorization)
> -  IAM 
> - Compute as a Service
> -  EC2
> -  Containers (EKS, ECS, Docker)
> -  Serverless (Lambda)
> - Networking
> -  VPC
> 

<br> 

> ### Topics in progress
> Storage

<hr/>
<hr/>

# AWS Certificate

![Alt text](/assets/my_certificate.png)


<hr/>

# Build Projects with AWS

## 1. Serverless 

- Link: https://github.com/Akashay-Anand/Planetary-View

- Link: https://www.youtube.com/watch?v=_GXGRl76D00


#### *About*

- *Technologies Used*: NodeJS, Twilio, AWS, and Serverless Framework.

- Built a cloud base backend application which uses nasa.gov api to fetch latest space image and metadata. And periodically sends this data packet to my phone number as a SMS.
- This function uses NodeJS as a runtime for JavaScript and to maintain modules. here Axios library is used to interact with API. Serverless framework for integrating configuration files and code, it also simplify the deployment process on aws lambda. Finally, Twilio library is integrated with it to send the message whenever the lambda function gets evoked.
- Impact: The **API** is constrained by a rate **limit of 1000 requests per hour**, whereas the aws **lambda can uphold 1 million request and 3.2 million compute seconds** per month in free tier.

## 2. System Monitoring Application

- Link: https://github.com/Akashay-Anand/Cloud-Native_System-Monitoring-Application

#### *About*

- *Technologies Used*: AWS (ECR, Boto3, etc.) Python (Flask, psutil), Docker,
- It shows CPU and memory status of the system with proper messages.
- In this Project: created monitoring app using Flask, containerised it with docker and hosted on aws elastic container, deployed on kube.

## 3. Hosted Portfolio on AWS
- Hosted Portfolio website of AWS S3 .
- https://portfolio-anand.s3.ap-south-1.amazonaws.com/index.html

