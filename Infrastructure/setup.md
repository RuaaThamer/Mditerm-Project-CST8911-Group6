# Azure SQL Database Connection Guide

This document explains how team members can connect to the Azure SQL Database and Azure Data Factory created for the project.

⚠️ **Security Notice**  
For security reasons, the database password is **not stored in this repository**.  
The password shared privately with team members.

---

# Azure Resources Information

## Azure SQL Database

Server:
sql-midtermproject-server.database.windows.net

Database:
sqldb-midtermproject

Username:
sqladmin

Port:
1433

Authentication:
SQL Authentication

---

# Template Connection String

Server=tcp:sql-midtermproject-server.database.windows.net,1433;  
Initial Catalog=sqldb-midtermproject;  
Persist Security Info=False;  
User ID=sqladmin;  
Password=password provided privately;  
MultipleActiveResultSets=False;  
Encrypt=True;  
TrustServerCertificate=False;  
Connection Timeout=30;

---

# Connecting with SQL Server using (SSMS) or VS Code with the SQL Server (mssql) extension

1. Open **SQL Server Management Studio (SSMS)**
2. In **Server name**, enter:

sql-midtermproject-server.database.windows.net

3. Authentication Type:

SQL Server Authentication

4. Username:

sqladmin

5. Enter the password shared privately.

6. Click **Connect**

---

# Connecting from Azure Data Factory

1. Go to **Azure Portal**
2. Open **Azure Data Factory**
3. Click **Launch Studio**
4. Create a **Linked Service**
5. Choose:

Azure SQL Database

6. Enter the following details:

Server: sql-midtermproject-server.database.windows.net  
Database: sqldb-midtermproject  
Username: sqladmin  
Password: (provided privately)

---

# Connecting from Power BI

1. Open **Power BI Desktop**
2. Click **Get Data**
3. Select **Azure SQL Database**
4. Enter:

Server: sql-midtermproject-server.database.windows.net  
Database: sqldb-midtermproject

5. Choose **SQL Server Authentication**
6. Enter username and password.

---

# Azure Data Factory Information

Data Factory Name:
adf-midtermproject

Resource Group:
Mid_Term_Project

Region:
Canada Central

Access is provided through Azure RBAC permissions.

---

# Support

If you has trouble accessing the resources or connecting to the database, contact walt0180@algonquinlive.com in Microsoft Teams.
