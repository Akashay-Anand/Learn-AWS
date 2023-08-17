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

<hr/>
<hr/>

## Types of Hypervisor used by AWS for VM's

1. __Xen__  
Xen is an __open-source__ hypervisor that provides virtualization technology to run multiple operating systems on a single physical machine simultaneously. It is designed to create isolated environments called "virtual machines" (VMs) or "guests" on a host system. Each virtual machine operates independently as if it were running on its own dedicated hardware while sharing the physical resources of the host machine.

* __Hypervisor Architecture__: Xen operates as a Type 1 hypervisor, also known as a "bare-metal" hypervisor. This means it runs directly on the hardware without needing a host operating system. This architecture enhances performance and security

* __Paravirtualization and Hardware Virtualization__: Xen initially introduced the concept of paravirtualization, which involves modifying guest operating systems to be aware of the hypervisor, resulting in optimized performance and better resource utilization. Over time, Xen also incorporated hardware virtualization extensions (such as Intel VT-x and AMD-V), enabling the virtualization of unmodified operating systems.

* __Isolation and Resource Allocation__: Xen ensures strong isolation between virtual machines, enhancing security and stability. It provides tools for administrators to allocate CPU, memory, storage, and network resources to each VM.

* __Multiple Operating Systems__: Xen supports running a variety of guest operating systems, including Linux, Windows, and other Unix-like systems. These guest operating systems can run concurrently on the same physical hardware.

* __Performance__: Xen's architecture typically results in minimal overhead compared to traditional virtualization solutions

2. __Nitro__
The Nitro Hypervisor is a lightweight, high-performance hypervisor developed by Amazon Web Services (AWS) as a fundamental component of the Nitro System. it is a bare-metal hypervisor that replaces the Xen hypervisor previously used in EC2 instances. It's specifically designed to offload most of the virtualization work from the main host CPU to dedicated hardware components. This approach improves overall instance performance and security.

* _Bare-Metal Hypervisor_: Similar to other Type 1 hypervisor, the Nitro Hypervisor is a "bare-metal" hypervisor, meaning it runs directly on the physical hardware without the need for an underlying host operating system. This architecture minimizes overhead and maximizes performance.

* _Hardware Offloading_: One of the core advantages of the Nitro Hypervisor is its ability to offload virtualization tasks to dedicated hardware components. This includes tasks related to memory management, CPU scheduling, and interrupt handling. By offloading these tasks, the main CPU is freed up to focus on executing application workloads.

* _Isolation and Security_: The Nitro Hypervisor provides strong isolation between instances, ensuring that workloads are isolated from each other

> The Nitro Hypervisor is part of AWS's continuous effort to optimize the performance and capabilities of its cloud services. As AWS services evolve, the Nitro System and its components play a crucial role in delivering efficient, secure, and scalable infrastructure to customers.

