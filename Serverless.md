# SERVERLESS


__EC2 is certainly not serverless__

ECS and EKS run containers on clusters of EC2 instances. So in that case EC2 as the compute platform for your containers,

So thinking about serverless compute for containers.?

So here service AWS Fargate comes into the picture.

///////////////////////////////////////////////////////////////     

Amazon’s CTO, Werner Vogels, says, “No server is easier to manage than no server.” This quote summarizes the convenience you can have when running serverless solutions, like AWS Fargate and AWS Lambda.    

//////////////////////////////////////////////////////////////     

If you run your code on Amazon EC2, AWS is responsible for the physical hardware and you are responsible for the logical controls, such as guest operating system, security and patching, networking, security, and scaling.If you run your code in containers on Amazon ECS and Amazon EKS, AWS is responsible for more of the container management, such as deploying containers across EC2 instances and managing the container cluster. However, when running ECS and EKS on EC2, you are still responsible for maintaining the underlying EC2 instances.If you want to deploy your workloads and applications without having to manage any EC2 instances, you can do that on AWS with serverless compute.

///////////////////////////////////////////////////////////

> serverless mentions four aspects.

* No servers to provision or manage.
* Scales with usage.
* You never pay for idle resources.
* Availability and fault tolerance are built-in.

//////////////////////////////////////////////////////////

### Amazon ECS and Amazon EKS enable you to run your containers in two modes.

* __Amazon EC2 mode__
* __AWS Fargate mode__

// ex 
<img width="819" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/c635e52e-7d4d-407e-ab86-bd23a78e5731">

<br/>

### AWS Fargate

> AWS Fargate is a serverless compute platform for containers that you can use with either ECS or EKS. With AWS Fargate as the compute platform, you run your containers on a managed serverless platform. The scaling and fault tolerance is built-in, and you don't need to worry about the underlying operating system or environment

* AWS Fargate is a purpose-built serverless compute engine for containers.
* Fargate supports both Amazon ECS and Amazon EKS architecture and provides workload isolation and improved security by design.

> AWS Fargate can be used for all of the common container use cases including microservice architecture applications, batch processing, machine learning applications and migrating on-premises applications to the cloud

> 



### AWS LAMBDA

> If you want to deploy your workloads and applications without having to manage any EC2 instances or containers, you can use AWS Lambda.AWS Lambda lets you run code without provisioning or managing servers or containers.

> can run code for virtually any type of application or backend service, including data processing, real-time stream processing, machine learning, WebSockets, IoT backends, mobile backends, and web apps, like your corporate directory app!

> __HOW LAMBDA WORKS__

> There are three primary components of a Lambda function: the trigger, code, and configuration.The code is source code, that describes what the Lambda function should run.

* ex:
* <img width="301" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/8f31a632-72f3-4875-bd15-0ca1b383a7bf">

> When you create your Lambda function, you specify the runtime you want your code to run in. There are built-in runtimes such as Python, Node.js, Ruby, Go, Java, .NET Core, or you can implement your Lambda functions to run on a custom runtime.The configuration of a Lambda function consists of information that describes how the function should run. In the configuration, you specify network placement, environment variables, memory, invocation type, permission sets, and other configurations. To dive deeper into these configurations, check out the resources section of this unit.Triggers describe when the Lambda function should run. 

> AWS Lambda function handler
* The AWS Lambda function handler is the method in your function code that processes events. When your function is invoked, Lambda runs the handler method.

> Lambda Trigger

* Once you create a Lambda function, it isn't always running all of the time. Instead, Lambda functions run in response to triggers. You can configure a trigger for when you want your function to run, and from there the Lambda service waits for the trigger or polls for an event to trigger the function
* Examples of trigger funnction:
* an HTTP request, an upload of a file to the storage service Amazon S3, events originating from other AWS services, or even in-app activity from mobile devices.

<img width="440" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/ac1c2e98-5a9c-4905-a974-f4cd69af646b">

<br>

>  Lambda is currently designed to run code that has a runtime of under 15 minutes. So this isn't for long running processes like deep learning or batch jobs. You wouldn't host something like a WordPress site on AWS Lambda. It's more suited for quick processing like a web backend handling request, or a backend report processing service or microservice hosting

> 
