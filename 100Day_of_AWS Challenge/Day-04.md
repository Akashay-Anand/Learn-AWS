# Prerequisites & AWS Free Account

> Before directly jumping on Cloud Platforms… if to truly grasp the power and potential of AWS, it’s essential to have an understanding of some foundational concepts.

> having an understanding of these concepts will ultimately help you to understand various cloud services in a better and faster way.


## Prerequisites/core concepts of It services in Cloud

### Servers

Servers are the backbone of modern computing and play a crucial role in AWS infrastructure. In the AWS environment, servers refer to virtual instances that run on physical hardware within AWS data centers. These instances can be configured to suit various computing needs, from simple web hosting to complex data analytics.

> Ex:

- Amazon Elastic Compute Cloud (Amazon EC2) is AWS’s flagship service for server provisioning. It allows you to launch virtual servers, or instances, in the cloud, with full control over the operating system, instance type, and scalability.

### Hypervisor

A hypervisor is a software or hardware layer that enables multiple virtual machines (VMs) to run on a single physical server. It acts as a mediator between the VMs and the physical hardware, ensuring efficient resource allocation and isolation.

> Ex:

- AWS uses a custom-built hypervisor called the Nitro Hypervisor, which we need for creating EC2 instances.

### Virtualization

Virtualization is the process of creating virtual instances of computing resources such as servers, storage, and networking. It enables better resource utilization, isolation, and flexibility, making it a fundamental concept in cloud computing.

> Ex:

- Elastic Load Balancing uses virtualization to efficiently manage your website’s visitors across multiple virtual servers (EC2 instances).

- AWS provides various virtualization options, including hardware-assisted virtualization (HVM) and paravirtualization (PV), depending on the instance type. This allows users to choose the most suitable virtualization technology for their workloads

### Cloud Type

*There are three primary cloud types:*

> **public cloud:** 
- In a public cloud, services and resources are owned and operated by a third-party cloud provider, like AWS, GCP, or Azure. They are made available to the general public over the Internet.

> **private cloud:** 
- A private cloud is dedicated to a single organization, providing the benefits of cloud computing within a controlled, private network. AWS offers solutions like Amazon Virtual Private Cloud (Amazon VPC) to create isolated, secure environments.

> **hybrid cloud:**
- A hybrid cloud combines both public and private cloud environments, allowing data and applications to move seamlessly between them.

<br>
<br>

> *Ex:*

- Netflix, a prominent AWS customer, employs a hybrid cloud architecture. They use AWS for public-facing streaming services while maintaining their own private cloud infrastructure for sensitive data and content delivery.

<br/>
<br/>
<br/>

## Now it is time to initiate our interaction with AWS.

> AWS Free Account

Well, You can follow any video from YouTube to create a free Tier account.

*Here, I have found one for you.👩🏻‍💻🤴🏻*
- https://www.youtube.com/watch?v=SFaSB6vgp8k