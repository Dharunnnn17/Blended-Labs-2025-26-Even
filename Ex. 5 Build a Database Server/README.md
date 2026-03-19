# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: DHARUN ARULSELVAN
* **Register Number**: 212224220024
* **Date of Submission**: 19.03.2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

1. First, a security group named DB Security Group was created to allow the web server to connect to the database using port 3306 (MySQL).
2. A DB Subnet Group was created with subnets from two Availability Zones to allow the database to run in a Multi-AZ environment for high availability.
3. A MySQL RDS instance named lab-db was created with the database name lab, username main, and password lab-password.
4. The database was associated with the DB Security Group and the Lab VPC so that the web server can securely connect to the database.
5. The web application running on the EC2 server was opened using its IP address, and the RDS endpoint, database name, username, and password were entered to interact with the database.
---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

![027d76c5-9017-4769-8d25-e10be87e7046](https://github.com/user-attachments/assets/a58aabea-5bc5-41b7-806d-a87c7f757869)
![38cf72aa-c3be-4f71-afee-ea333575b14d](https://github.com/user-attachments/assets/f1a8e8e5-a647-416b-bec9-33071bcece7b)


---

### Screenshot 2: Database Service Running
![57c2cfbd-d4f8-43dd-b601-90b52fafac94](https://github.com/user-attachments/assets/fa08aabb-1508-4bcd-9b21-f5e34e96dc91)
![4607766b-1dd1-4c38-89b2-8ddf66fb9ff2](https://github.com/user-attachments/assets/86945c77-7b2c-4a7a-94e2-3843b199d76e)


---

### Screenshot 3: Sample Database and Table
![8fb1d844-98cd-4eeb-8585-aed430efea2f](https://github.com/user-attachments/assets/bcc4b48f-a665-4cf6-bead-b3edc3809ec7)



---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
