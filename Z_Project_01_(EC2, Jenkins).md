# Project - 
### create *EC2* instance and Install *Jenkins* with the help of *CLI Terminal from your local System.*

<br>

[Note] Windows PowerShell and git bash, both work with SSH

<br>

### Step 1: Creating a new EC2 instance on AWS

Path> AWS > EC2 > Launch Instance

Details: 
- Name: Test Jenkins ; 
- OS Image (AMI): Amazon Linux ; (the default one)
- AMI Type: Amazon Linux 2023 AMI ; (available in free tiers ; default one) ;
![Alt text](/assets/p01_os_selection.png)

- Instance Type: t2.micro ; (available in free tiers ; default one) ;
![Alt text](/assets/p01_instance_type.png)

- Key Pair: creating a key pair (tempApp) ; this will help to access instance from remote device. 
- ![Alt text](/assets/p01_keypair.png)

- leave rest as defoult ; click on Launch Instance ;

![Alt text](/assets/p01_all_instance.png)

### Step 2: connect to instance from powershell

- navigate to CONNECT option from top menu on instance page; go to 'SSH client' tab and copy SSH command ; this 
- 



// Basic linux Command /////////////////////

1. whoami : print current user
2. sudo : if I am not root user, I can access   get administrator access using sudo; 
3. sudo su - : switch to root user
4. su <user_name> : switch to different user; no need of sudo while working with root user;
5. sudo apt update :  update all files ; apt might fail ; install or update apt first or use 'yum'
6. sudo yum update : update all files ;
7. chmod 400 < file name > : can change permissions of files

/////////////////////

Q) if using windows termninal or git bash for cli access of any instance
> some linux commands might won't work for example: 
> - sudo apt update. 

> in that case find ulternative. 
> - sudo yum update –y

<br>
<br>

# Resource
> setup EC2, install jenkins in AWS linux instance.
> - https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/#prerequisites

> Now follow these steps to install JENKINS.
> - https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/#downloading-and-installing-jenkins
>
> 