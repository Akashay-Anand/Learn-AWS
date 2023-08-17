# Hypervisor

> Hypervisor is a software program that allows multiple virtual machines (VMs) to run on the same physical server. The hypervisor allocates resources, such as CPU, memory, and storage, to each VM so that they can run independently of each other.

* Type 1 hypervisors are also known as bare-metal hypervisors. They are installed directly on the physical hardware, and they do not require an operating system. This makes them very efficient, but they also require more technical expertise to set up and manage.
* > If you need a high-performance VM group, then you should choose a type 1 hypervisor
* Type 2 hypervisors are installed on top of an operating system. This makes them easier to set up and manage, but they are not as efficient as type 1 hypervisors.
* > If you need a VM group that is easy to set up and manage, then you should choose a type 2 hypervisor

> When you create a VM group for a hypervisor for AWS, you are essentially creating a group of VMs that will be managed by the hypervisor. The hypervisor will ensure that each VM has the resources it needs to run properly, and it will also prevent VMs from interfering with each other

<br/>
<br/>
<br/>

__[Note]:__ Amazon Web Services (AWS), you don't typically work with a hypervisor directly like you might in a traditional virtualization environment. Instead, In AWS, when you launch an EC2 (Elastic Compute Cloud) instance, you are creating a virtual machine, but you don't interact with the hypervisor directly. AWS handles the hypervisor layer and provides you with a variety of instance types that offer different levels of CPU, memory, and other resources.

# EC2 (Amazon Elastic Compute Cloud)

> It is a cloud computing service that provides resizable compute capacity in the cloud. With EC2, you can launch as many or as few virtual machines (VMs) as you need, and scale them up or down as your needs change. You can also customize your VMs with the operating system, storage, and networking that you need.
* EC2 is a pay-as-you-go service, so you only pay for the resources that you use.

### EC2 is a popular choice for a variety of workloads, including:
* Web servers
* Database servers
* Application servers
* Development and testing environments
* High-performance computing (HPC)
* Machine learning

<br/>

> When you launch an EC2 instance in AWS, you're essentially creating a virtual machine
> Each instance is backed by the AWS infrastructure, including the hypervisor layer, but you don't need to interact with the hypervisor itself.

