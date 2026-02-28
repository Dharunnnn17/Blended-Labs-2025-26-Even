# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: DHARUN ARULSELVAN
* **Register Number**: 212224220024
* **Date of Submission**: 28/02/2026

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1.The EC2 Dashboard was accessed through the AWS Management Console to explore its various features.
2.A new EC2 instance was launched using the Amazon Linux 2 AMI and the t2.micro instance type for free-tier eligibility.
3.The security group was configured to allow SSH access from the specified IP address and HTTP access from all IPs.
4.The instance was connected via SSH using the downloaded key pair, and basic operations such as stop, start, and reboot were performed.
5.Finally, the instance was monitored using the Monitoring tab before being terminated to avoid additional charges.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1600" height="862" alt="image" src="https://github.com/user-attachments/assets/c4f51d3b-7b58-4cdb-908c-15a4021ef149" />
<img width="1600" height="850" alt="image" src="https://github.com/user-attachments/assets/e7ff38c9-403c-4687-a4f0-65ff506cdaac" />


---

### Screenshot 2: SSH Connection to Instance

<img width="1600" height="812" alt="image" src="https://github.com/user-attachments/assets/60cc3a42-ee6e-43e4-87c9-f999b1f608f2" />
<img width="1600" height="851" alt="image" src="https://github.com/user-attachments/assets/050923a9-6f2f-4979-8bd8-2cb08970299a" />



---

### Screenshot 3: Instance Monitoring / Status

<img width="1600" height="865" alt="image" src="https://github.com/user-attachments/assets/5345400e-f750-4e6e-ab22-a39eec62e4db" />
<img width="1600" height="817" alt="image" src="https://github.com/user-attachments/assets/fb3efd45-197a-445e-a82d-d8fbdcede89a" />
<img width="1600" height="862" alt="image" src="https://github.com/user-attachments/assets/ac841055-ce67-43f9-a9f4-908a042e5c23" />
<img width="1600" height="860" alt="image" src="https://github.com/user-attachments/assets/a44002e9-3cdd-4f5f-81da-97df5dfa05ad" />




---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
