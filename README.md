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
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/10728956-e5f2-40f3-97f4-b4e70239cc36" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/d87377be-31db-4472-9be6-1cb9cb10026d" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/1a006821-2463-40c9-ba4d-07e7a83a3769" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/d9527fd4-a3f7-4df3-8524-5f27fae629af" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/e2bbef00-8c0c-4c73-955f-4ab5931a5162" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/046981c6-3262-48c4-bf02-59e9ba4c1dd4" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/1423d40b-b562-4053-91b9-090abc688df7" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/ff16357e-b93b-4d4d-81ea-06bd70f28af0" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/9f6f58e5-74d1-4abe-87a2-1c8f510ae23e" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/988783b7-0dff-4002-a2dd-51f968e241fc" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/264209ca-6e51-4862-b79b-097bed720e71" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/569fb9d5-787d-47c2-a255-c05b68acc0f6" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/7cf60d02-bd22-4786-88c6-83d68a0fdd03" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/bf7e8111-e9ce-40f7-bb83-122a6e3be681" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/0d99b135-4967-42ec-bb09-f0a6546c9b08" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/9b6f2ebf-7f44-42fa-8bf2-7d188978a562" />

## Result

Thus, an Amazon RDS database instance was successfully created and configured as a cloud data storage server. The database was securely connected to a web application, and data operations such as inserting, updating, and deleting records were successfully performed through the application.


