# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: ANJALI K
* **Register Number**: 212224040024
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

1. Create a Security Group for RDS
2. Create a DB Subnet Group
3. Launch an RDS MySQL DB Instance
4. Configure Connectivity and Security
5. Connect Web App to Database and Test

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1919" height="1030" alt="Screenshot 2026-03-18 154015" src="https://github.com/user-attachments/assets/a0e25b68-ee05-464f-abc0-c08a7d5b3608" />



---

### Screenshot 2: Database Service Running

<img width="1919" height="1029" alt="Screenshot 2026-03-18 161203" src="https://github.com/user-attachments/assets/71108a2b-c20c-4401-b390-97820b2c2956" />


---

### Screenshot 3: Sample Database and Table

<img width="1919" height="1027" alt="Screenshot 2026-03-18 161737" src="https://github.com/user-attachments/assets/4fc7bf9c-11c5-45df-8be8-7a08913103df" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were understood.
