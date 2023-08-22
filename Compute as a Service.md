# Compute
"Compute" refers to the act of performing calculations, processing data, executing instructions, and carrying out operations using a computer's central processing unit (CPU) or other processing components. In simpler terms, compute involves using the processing power of a computer to perform various tasks and operations.


### Compute Service
A compute service is a cloud computing offering that provides virtualized computing resources over the internet.

_Compute services generally provide the following key resources:_ 

__Virtual Machines (VMs):__ Virtual machines are instances of virtualized operating systems running on a physical server. Each VM behaves like a standalone computer and has its own CPU, memory, storage, and networking resources. Customers can choose the specifications of VMs, such as the number of CPU cores, amount of RAM, and storage capacity.

__CPU (Central Processing Unit):__ The CPU is the "brain" of the computer that performs calculations and executes instructions. Compute services allow customers to select the number of CPU cores and processing power that best suits their application's requirements.

__Memory (RAM):__ Memory is used to store data and code that the CPU needs to access quickly. Compute services offer various memory options to accommodate different workloads.

__Storage:__ Compute services provide various types of storage, including block storage and object storage. Block storage is akin to traditional hard drives and is used for storing operating systems and application data. Object storage is suited for storing large amounts of unstructured data, such as files and media.

__Networking:__ Compute services offer networking capabilities to connect virtual machines and other resources to the internet or private networks. This includes features like IP addresses, load balancers, firewalls, and virtual private networks (VPNs).

<hr/>

# Compute as a Service
__> OverView__   
> Every business needs raw compute capacity to run applications. These applications could be web servers, batch jobs, databases, HR software, machine learning       
  
> The time, money, and effort it takes to get up and running with on-premises computing resources are fairly high. The worst part is, once you buy these physical servers, you are stuck with them whether you use them or not. It's not easy to just suddenly provision more physical compute capacity when you need it, and it's even harder to get your money back on servers you no longer need

> Compute as a Service model resolve this issue by providing compute resources through the internet
> It is much easier to get started and support operations over time.


<hr>

# AWS Compute services
<img width="281" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/c92cd806-5582-451e-ab88-4ae2a46e5d51">

<hr>

## Choose the Right Compute Option

> We have many compute options. You need to know which service to use for which use case.

> At a fundamental level, there are three types of compute options:     
1. __virtual machines__,  
2. __container services__,  
3. __serverless__.   

<br/>
<hr/>

1.  __virtual machine__
> A _virtual machine_ can often be the easiest compute option in AWS to understand. This is because a virtual machine emulates a physical server and allows you to install an HTTP server to run your applications.    
> these virtual machines are called Amazon Elastic Compute Cloud or Amazon __EC2__

 <hr/>

 2. __container services__

> A container is a standardized unit that packages up your code and all of its dependencies. This package is designed to run reliably on any platform, because the container creates its own independent environment. This makes it easy to carry workloads from one place to another,
> 

Q) THE DIFFERENCE BETWEEN CONTAINERS AND VMS?
* Containers share the same operating system and kernel as the host they exist on, whereas virtual machines contain their operating system.
* Since each virtual machine has to maintain a copy of an operating system, there’s a degree of wasted space. A container is more lightweight. They spin up quicker, almost instantly. This difference in startup time becomes instrumental when designing applications that need to scale quickly during input/output (I/O) bursts.
* While containers can provide speed, virtual machines offer you the full strength of an operating system and offer more resources, like package installation, a dedicated kernel, and more.

<img width="572" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/9f73f2ec-d949-47dc-bcee-b16733dd5055">

<br/>

> AWS offers two container orchestration services: Amazon Elastic Container Service __(ECS)__ and Amazon Elastic Kubernetes Service __(EKS)__.

<hr/>

3. __Serverless__

> serverless mentions four aspects.

* No servers to provision or manage.
* Scales with usage.
* You never pay for idle resources.
* Availability and fault tolerance are built-in.


> I like to think of AWS services as existing on a spectrum. On one side of the spectrum, you have convenience and on the other side, you have control. Many services exist to give you control like Amazon EC2 whereas other services exist to give you convenience, like the serverless compute AWS Lambda.

<hr/>




<br/>
<br/>
<br/>



<br/>
<br/>
<br/>

### Resources 📑

* https://docs.aws.amazon.com/whitepapers/latest/aws-overview/compute-services.html
* https://aws.amazon.com/products/compute/
* https://aws.amazon.com/blogs/compute/


