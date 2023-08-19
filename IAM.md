# IAM
With IAM, you can share access to an AWS account and resources without having to share your set of access keys or password.

### To help control access and manage identities within your AWS account, IAM offers many features to ensure security.
* IAM is global and not specific to any one Region. This means you can see and use your IAM configurations from any Region in the AWS Management Console.
* IAM is integrated with many AWS services <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html">by default </a>
* You can establish password policies in IAM to specify complexity requirements and mandatory rotation periods for users.
* IAM supports MFA.
*IAM supports identity federation, which allows users who already have passwords elsewhere—for example, in your corporate network or with an internet identity provider—to get temporary access to your AWS account.


### WHAT IS AN IAM GROUP?
> An IAM group is a collection of users.   
> All users in the group inherit the permissions assigned to the group.    
> it’s a more convenient and scalable way of managing permissions for users in your AWS account

### features of groups
* Groups can have many users.
* Users can belong to many groups.
* Groups cannot belong to groups.

<br/>

> EX:
> group can be created from IAM > user group > create Group
<img width="653" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/daddaa67-c664-4039-be21-04f718e73b3b">



__[Note]: <br/>
a) The root user can perform all actions on all resources inside an AWS account by default. This is in contrast to creating new IAM users, new groups, or new roles.
<br/>
b) New IAM identities can perform no actions inside your AWS account by default until you explicitly grant them permission.
<br/>
c) The way you grant permissions in IAM is by using IAM "policies".__


### WHAT IS AN IAM POLICY?
> To manage access and provide permissions to AWS services and resources, you create IAM policies and attach them to IAM users, groups, and roles. Whenever a user or role makes a request, AWS evaluates the policies associated with them.

> Most policies are stored in AWS as JSON documents with several policy elements.

> Ex:

``` json
// Example 1

{
"Version": "2012-10-17",    
     "Statement": [{        
          "Effect": "Allow",        
          "Action": "*",        
          "Resource": "*"     
     }]
}

// In this policy, there are four major JSON elements: Version, Effect, Action, and Resource.

"Version" element defines the version of the policy language. It specifies the language syntax rules that are needed by AWS to process a policy. To use all the available policy features, include "Version": "2012-10-17" before the "Statement" element in all your policies.
"Effect" element specifies whether the statement will allow or deny access. In this policy, the Effect is "Allow", which means you’re providing access to a particular resource.
"Action" element describes the type of action that should be allowed or denied. In the above policy, the action is "*". This is called a wildcard, and it is used to symbolize every action inside your AWS account.
"Resource" element specifies the object or objects that the policy statement covers. In the policy example above, the resource is also the wildcard "*". This represents all resources inside your AWS console.

>* utting all this information together, you have a policy that allows you to perform all actions on all resources inside your AWS account. This is what we refer to as an (administrator policy).

// Example 2

{"Version": "2012-10-17",    
     "Statement": [{        
          "Effect": "Allow",        
          "Action": [            
               "iam: ChangePassword",            
               "iam: GetUser"            
               ]        
          "Resource": 
"arn:aws:iam::123456789012:user/${aws:username}"    
     }]
}

// this policy allows the IAM user to change their own IAM password (iam:ChangePassword) and get information about their own user (iam:GetUser). It only permits them to access their own credentials because the resource restricts access with the variable substitution ${aws:username}.

```

<img width="609" alt="image" src="https://github.com/Akashay-Anand/Learn-AWS/assets/82114930/9cf5ca0e-8d65-4ea3-b57d-f439cbc6085f">

<br/>



<br/>
<br/>
## Resources
<br/>
* https://docs.amazonaws.cn/en_us/IAM/latest/UserGuide/introduction.html  
* https://docs.amazonaws.cn/en_us/IAM/latest/UserGuide/id.html  
* https://docs.amazonaws.cn/en_us/IAM/latest/UserGuide/access.html  

