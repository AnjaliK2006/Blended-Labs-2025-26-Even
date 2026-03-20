# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
## Author : 
## Name: ANJALI K   
## Reg no : 212224040024  

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. Open the AWS Management Console and navigate to the EC2 dashboard.

2. In the left panel, select Instances and verify that Web Server 1 is in a running state (2/2 status checks passed).

3. Select Web Server 1, then go to Actions → Image and templates → Create image.

4. Enter the required details:

    Image Name: WebServerAMI
    Description: Lab AMI for Web Server

5. Click Create image to generate the AMI, which will be used later for Auto Scaling.

---

## Output Screenshots 

Creation of AMI from EC2 Instance (Web Server 1)

<img width="1919" height="1079" alt="Screenshot 2026-03-20 134337" src="https://github.com/user-attachments/assets/1b42e64e-476d-4436-aad3-503be3b6111d" />

Application Load Balancer and Target Group Configuration

<img width="1919" height="1079" alt="Screenshot 2026-03-20 134622" src="https://github.com/user-attachments/assets/41073ee9-ec41-44f9-a00f-9ca85b12c1dd" />

Auto Scaling Group with Dynamic Instance Scaling

<img width="1919" height="1079" alt="Screenshot 2026-03-20 135947" src="https://github.com/user-attachments/assets/68910cc1-e4b3-44bd-8756-47de5e2970b9" />


<img width="1919" height="1079" alt="Screenshot 2026-03-20 140740" src="https://github.com/user-attachments/assets/5411ba89-01f8-4467-9458-75621d37d3a7" />

Instance Termination

<img width="1919" height="1079" alt="Screenshot 2026-03-20 141549" src="https://github.com/user-attachments/assets/33e38c21-f659-402a-80f6-7378c8fd288a" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
