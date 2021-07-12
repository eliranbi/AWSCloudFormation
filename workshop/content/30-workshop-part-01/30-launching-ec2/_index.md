---
title: 'Launching an EC2 Instance'
date: 2019-10-22T12:06:55+01:00
weight: 30
chapter: true
---

# LAUNCHING AN EC2 INSTANCE

# Launching an EC2 Instance

![](ec2-1.png)

In the previous chapter, you learnt the CloudFormation fundamentals and about various _Template_ sections.

You have created an EC2 instance with Elastic IP. This is a simplistic scenario.

In this chapter you will improve the existing template with the following features:

+ Use Systems Manager Parameter Store to deploy the latest Amazon Linux 2 AMI in any region.
+ Attach an IAM role to the instance and login to it using SSM Session Manager.
+ Bootstrap the instance using a _UserData_ script.
+ Use `cfn-init` to assist bootstrapping an EC2 instance.

- [Lab 06: Multi Region Latest AMI](/workshop/content/30-workshop-part-01/30-launching-ec2/100-lab-06-ami/_index.md)
- [Lab 07: SSM - Session Manager](/workshop/content/30-workshop-part-01/30-launching-ec2/200-lab-07-session-manager/_index.md)
- [Lab 08: User Data](/workshop/content/30-workshop-part-01/30-launching-ec2/300-lab-08-user-data/_index.md)
- [Lab 09: Helper Scripts](/workshop/content/30-workshop-part-01/30-launching-ec2/400-lab-09-helper-scripts/_index.md)