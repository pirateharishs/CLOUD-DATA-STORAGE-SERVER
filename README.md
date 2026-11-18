# CLOUD-DATA-STORAGE-SERVER

### NAME: HARISH S
### REG NO: 212223230071

## Aim

To create and configure an Amazon Relational Database Service (Amazon RDS) instance as a cloud data storage server, configure the required security settings, connect it to a web application, and perform database operations using the application.

## Algorithm / Steps

1. Create a Security Group for the RDS database.
2. Add an inbound rule to allow MySQL (Port 3306) access from the Web Security Group.
3. Create a DB Subnet Group using two Availability Zones.
4. Launch an Amazon RDS MySQL database instance.
5. Configure the database with the required identifier, username, password, storage, and instance class.
6. Associate the database with the created Security Group and Subnet Group.
7. Wait until the database status becomes **Available**.
8. Copy the RDS endpoint.
9. Open the web application using the provided Web Server IP address.
10. Enter the RDS endpoint, database name, username, and password.
11. Connect the application to the database.
12. Verify the connection by adding, editing, and deleting records in the Address Book application.


## Program

### Security Group Configuration

* Security Group Name: **DB Security Group**
* Inbound Rule: **MySQL/Aurora (3306)**
* Source: **Web Security Group**

### DB Subnet Group

* Name: **DB-Subnet-Group**
* VPC: **Lab VPC**

### Amazon RDS Configuration

* Engine: **MySQL**
* Template: **Dev/Test**
* Availability: **Multi-AZ**
* DB Instance Identifier: **lab-db**
* Username: **main**
* Password: **lab-password**
* Instance Class: **db.t3.micro**
* Storage: **20 GB (General Purpose SSD)**

### Connect the Application

```text
Endpoint : <RDS Endpoint>
Database : lab
Username : main
Password : lab-password
```

After submitting the above details, perform Add, Edit, and Delete operations on the Address Book application.

## Output
<img width="1920" height="1200" alt="Screenshot (129)" src="https://github.com/user-attachments/assets/ab97522c-1447-46ad-a05c-725fc838672d" />

<img width="1920" height="1200" alt="Screenshot (130)" src="https://github.com/user-attachments/assets/9907c0a2-0bda-4895-ad36-a5c3b6bb003b" />

<img width="1920" height="1200" alt="Screenshot (131)" src="https://github.com/user-attachments/assets/c9ae69a3-169b-4a28-924b-e8c737defb1e" />

<img width="1920" height="1200" alt="Screenshot (132)" src="https://github.com/user-attachments/assets/2e23b05e-32a7-4293-83c8-e6d0f40e752c" />

<img width="1920" height="1200" alt="Screenshot (133)" src="https://github.com/user-attachments/assets/473ad34f-db00-48c4-b926-93c6d35397ec" />

<img width="1920" height="1200" alt="Screenshot (134)" src="https://github.com/user-attachments/assets/08b7e3fc-54ae-4604-acd1-347cf52a3ce3" />

<img width="1920" height="1200" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/e8952756-58f0-4138-be21-596c9032513e" />

<img width="1920" height="1200" alt="Screenshot (136)" src="https://github.com/user-attachments/assets/88746d2b-7201-4d68-adff-0063a6421519" />

<img width="1920" height="1200" alt="Screenshot (137)" src="https://github.com/user-attachments/assets/7566aecd-453f-473a-a576-e80b7a69f5e5" />

<img width="1376" height="712" alt="image" src="https://github.com/user-attachments/assets/ca00e09f-dd4b-4b06-bcee-da12f7205107" />

## Result

Thus, an Amazon RDS database instance was successfully created and configured as a cloud data storage server. The database was securely connected to a web application, and data operations such as inserting, updating, and deleting records were successfully performed through the application.


