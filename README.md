# AWS-IAM-MINI

## This project will demonstrate the use and purpose of IAM in AWS

### IAM (Identity and Access Management) is a web service that allows you to manage access to AWS resources securely. It enables you to control who can access which AWS services and resources, and under what conditions. Essentially, IAM helps you manage users, security credentials (like access keys), and permissions to control access to your AWS environment.

### IAM gives secure access to company resources—like emails, databases, data, and applications—to verified entities, ideally with a bare minimum of interference. The goal is to manage access so that the right people can do their jobs and the wrong people, like hackers, are denied entry.

## IAM Role

### Identity and Access Management (IAM) roles are entities you create and assign specific permissions to that allow trusted identities such as workforce identities and applications to perform actions within the organization's resources. n IAM role does not have any credentials and cannot make direct requests to AWS services. IAM roles are meant to be assumed by authorized entities, such as IAM users, applications, or an AWS service such as EC2

## IAM Policy

### An IAM policy is a way to allow or deny users to perform certain actions in an AWS account. When a user or a role is created, by default they only have permission to login. They cannot view, modify, or create any new resources. IAM policies are used to grant additional permissions.

## IAM Group

### IAM groups are collections of users with shared access control policies.These policies define what actions the group members are allowed to perform on specific objects within the group’s scope. For example, let’s say you have a group called “Developers.” In the group’s access control policy, you grant read-only access to all of your EC2 instances. Now, any user added to the “Developers” group will automatically have the permission to view information about those EC2 instances, but they won’t have permission to make any changes to them.

## IAM Users

### IAM users are like representatives for people or applications using AWS. They can access AWS through the console or programmatically. IAM users help manage access to AWS resources securely, and you can set permissions for them individually or in groups. They have names and passwords for console access and can create access keys for programmatic access. IAM users ensure only authorized users and apps can access your AWS resources.

## Create EC2 Full Access Policy for Eric.

- Head over to your AWS GUI and search for IAM using the search bar. Click on IAM.

![](./img/Pasted%20image.png)

- On the IAM dashboard, navigate to the left sidebar and click 'Policies'

![](./img/Pasted%20image%20(2).png)

- Search for 'EC2' then select 'AmazonFullAccess' form the policies list and click 'Create policy'

![](./img/Pasted%20image%20(3).png)

- Check 'All EC2 actions (ec2\*)' under 'Manual actions'

![](./img/Pasted%20image%20(4).png)

- On the 'Resources' section select 'All' and click 'Next' at the bottom right of the page.

![](./img/Pasted%20image%20(5).png)

- Add a name for the policy, optional description and click 'create policy'

![](./img/Pasted%20image%20(6).png)

- A success page should appear if the policy creation was successful

![](./img/Pasted%20image%20(7).png)

- Use "Filter by Type" select "Customer managed" to see the policy created for Eric.

![](./img/Pasted%20image%20(8).png)

## Create User

- Head over to the 'Users' section and click 'Create user'

![](./img/Pasted%20image%20(9).png)

- Enter a username, setup user password, check 'user must change password at next sign-in'. this allows the user to change the password you setup while creating the account. Click 'Next'.

![](./img/Pasted%20image%20(10).png)

- Sellect 'Attach policies directly' on the permissions tab. Select the policy created earlier 'Policy_for_Eric' and click 'Nect'.

![](./img/Pasted%20image%20(11).png)

- Review and click 'Create user' bottom left.

![](./img/Pasted%20image%20(12).png)

- The next page should show that you have successlick 'Download .csv file' to download user details in .csv format.

![](./img/Pasted%20image%20(13).png)

### AWS Policies: AWS has different policy types.

- Managed Policies: These type of policies are made and managed by AWS for users to used.
- Customer Managed: created and managed by user,you can create and manage them.
- Inline policies are created for specific reasons

## Create User Group.

- Back to the IAM GUI click 'User groups'

![](./img/Pasted%20image%20(15).png)

- Add a Group name 'Dev-team'

![](./img/Pasted%20image%20(16).png)

- Scroll down and click 'Create user group'

![](<./img/Pasted%20image%20(17).png)

- Dev-team group created successfully.

![](./img/Pasted%20image%20(18).png>)

## Create User Jack

- Back on the IAm GUI click Users.

![](./img/Pasted%20image%20(20).png)

- provide 'Jack' for the username and click next.

![](./img/Pasted%20image%20(21).png)

- In the permission sector click, Select 'Add user to group', check the dev-team group you have just create and click 'next'.

![](./img/Pasted%20image%20(22).png)

* Now click 'Create user'.

![](./img/Pasted%20image%20(23).png)

* Success page shows up with list of users including user-jack. 

## Create User Ade
* Click create user to begin creating another user account.

![](./img/Pasted%20image%20(24).png)

* Type-in a user name (Ade) and click 'next'.

![](./img/Pasted%20image%20(25).png)

* In the permission sector click, Select 'Add user to group', check the dev-team group you have just create and click 'next'.

![](./img/Pasted%20image%20(26).png)

* Review and click 'Create user'.

![](./img/Pasted%20image%20(27).png)

* A success page shows up confirming user account was created successfully.

![](./img/Pasted%20image%20(28).png)

