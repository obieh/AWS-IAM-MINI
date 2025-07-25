# AWS-IAM-MINI
## This project will demonstrate the use and purpose of IAM in AWS

### IAM (Identity and Access Management) is a web service that allows you to manage access to AWS resources securely. It enables you to control who can access which AWS services and resources, and under what conditions. Essentially, IAM helps you manage users, security credentials (like access keys), and permissions to control access to your AWS environment.

### IAM gives secure access to company resources—like emails, databases, data, and applications—to verified entities, ideally with a bare minimum of interference. The goal is to manage access so that the right people can do their jobs and the wrong people, like hackers, are denied entry.

## IAM Role
### Identity and Access Management (IAM) roles are entities you create and assign specific permissions to that allow trusted identities such as workforce identities and applications to perform actions within the organization's resources. n IAM role does not have any credentials and cannot make direct requests to AWS services. IAM roles are meant to be assumed by authorized entities, such as IAM users, applications, or an AWS service such as EC2


## IAM Policy
### An IAM policy is a way to allow or deny users to perform certain actions in an AWS account. When a user or a role is created, by default they only have permission to login. They cannot view, modify, or create any new resources. IAM policies are used to grant additional permissions.


## IAM Group
### IAM users represent individuals or applications on AWS, accessing resources through the console or programmatically. They have access to resources, and their permissions can be set individually or in groups. IAM groups are collections of users with shared access control policies.