# AWS Root User?
> When you first create an AWS account, you begin with a single sign-in identity that has complete access to all AWS services and resources in the account. This identity is called the AWS root user and is accessed by signing in with the email address and password that you used to create the account.
>
> ## AWS Root User Credentials
> The AWS root user has two sets of credentials associated with it.
* One set of credentials is the email address and password used to create the account. This allows you to access the AWS Management Console.
* The second set of credentials is called access keys, which allow you to make _programmatic requests from the AWS Command Line Interface (AWS CLI)_ or AWS API
* > Access keys consist of two parts:
  > * An access key ID, for example, A2lAl5EXAMPLE
  > * A secret access key, for example, wJalrFE/KbEKxE

## Best Practices When Working with the AWS Root User

> root user has complete access to all AWS services and resources in your account, as well as your billing and personal information

* Choose a strong password for the root user.
* Never share your root user password or access keys with anyone.
* Disable or delete the access keys associated with the root user.
* Do not use the root user for administrative tasks or everyday tasks.

# Understand Authentication
> Authentication ensures that the user is who they say they are. Usernames and passwords are the most common types of authentication, but you may also work with other forms, such as token-based authentication or biometric data like a fingerprint. Authentication simply answers the question, “Are you who you say you are?”


# Understand Authorization
> Once you’re inside your AWS account, you might be curious about what actions you can take. This is where authorization comes in. Authorization is the process of giving users permission to access AWS resources and services. Authorization determines whether the user can perform an action—whether it be to read, edit, delete, or create resources. Authorization answers the question, “What actions can you perform?”
> 
