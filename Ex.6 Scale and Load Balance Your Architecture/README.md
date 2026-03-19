# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : DHARUN ARULSELVAN   Reg no : 212224220024   Date : 19/03/2026

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

1.Launch multiple servers.

2.Deploy the application on each server.

3.Create a load balancer.

4.Add servers to the load balancer.

5.Configure auto-scaling.

6.Test load distribution.

---

## Output Screenshots 
![7cd599b2-29f2-488c-8118-9ec9128b4447](https://github.com/user-attachments/assets/fdb7d06b-288e-46ca-bcb3-1292c51f6f9a)
![a032809c-852f-4dcb-8141-9199e9475a52](https://github.com/user-attachments/assets/ea6b9b76-2a97-446d-aae9-b8d09b8e811e)
![fbe05757-9561-41a5-8f45-3d4ac6c8b79f](https://github.com/user-attachments/assets/b470ba2c-b23d-48c7-ad7a-b1b1a6023f93)
![09191993-e3dc-436b-8b3e-cbd4b3abbd70](https://github.com/user-attachments/assets/47ef458a-7cb7-4db3-acbe-81f7e2e225be)
![84b30e81-a1ab-40c0-b1ad-9bdedd03ddaa](https://github.com/user-attachments/assets/5ad72e15-d299-499a-98da-f5acb9a0c36f)
![b8ced0b6-b798-4d1a-8359-352421f8060c](https://github.com/user-attachments/assets/cd33575a-d7f5-47dd-ad93-7d542d51df12)
![dc12f4da-af95-42bd-b840-6f624c722891](https://github.com/user-attachments/assets/6200dd3a-42bf-4f72-8b4d-591245502719)


---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
