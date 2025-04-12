# PBLJ_9_E18497
🟢 Easy Level – Spring Dependency Injection with Java Configuration
✅ Objective:
To understand and implement Dependency Injection (DI) using Spring's Java-based configuration with @Configuration and @Bean annotations.

📘 Assignment Description:
Create two classes:

Course: with fields courseName and duration.

Student: with fields name and a reference to Course.

Use @Configuration class to define the beans.

Load the application context in the main() method using AnnotationConfigApplicationContext.

Print the Student details, including their assigned course.

📥 Input (Expected Configuration/Usage):
 
Student name: John Doe  
Course name: Java Programming  
Duration: 3 Months
📤 Expected Output:
 
Student Name: John Doe  
Enrolled Course: Java Programming  
Course Duration: 3 Months
🎯 Learning Outcome:
Understanding of Dependency Injection.

Java-based Spring Configuration.

How beans are managed and injected in Spring.

🟡 Medium Level – Hibernate CRUD with MySQL
✅ Objective:
Use Hibernate ORM to perform basic CRUD operations on a Student entity with a MySQL database.

📘 Assignment Description:
Create a Hibernate configuration file (hibernate.cfg.xml) with DB connection info.

Define a Student entity with fields:

id (Primary Key)

name

age

Implement a DAO class using Hibernate SessionFactory to perform:

Create

Read

Update

Delete

Test all four operations using sample data.

📥 Input (Sample Operations):
Add:
Student ID: 1, Name: Alice, Age: 20

Update:
Update student ID 1 name to "Alicia"

Read:
Fetch details of student with ID 1

Delete:
Remove student with ID 1

📤 Expected Output:
yaml
 
Student added successfully.  
Student updated: Alicia  
Student fetched: ID=1, Name=Alicia, Age=20  
Student deleted.
🎯 Learning Outcome:
Practical use of Hibernate with MySQL.

Understanding of configuration, mapping, and session lifecycle.

Performing CRUD operations in a persistent layer.

🔴 Hard Level – Spring + Hibernate Transaction Management
✅ Objective:
Develop a transactional banking system using Spring + Hibernate where money transfers between accounts are atomic and transaction-consistent.

📘 Assignment Description:
Integrate Spring and Hibernate using Java configuration or XML.

Create two entity classes:

Account: id, name, balance

Transaction: id, fromAccount, toAccount, amount, timestamp

Implement transfer logic that:

Deducts from one account

Adds to another

Saves transaction info

Use transaction management so that if any part of the operation fails, the entire transaction rolls back.

Demonstrate:

A successful transfer

A failed transfer (e.g., insufficient balance)

📥 Input (Sample Transactions):
Successful Transfer

From Account ID: 101, To Account ID: 102

Amount: 1000

Both accounts exist and have sufficient balance

Failed Transfer

From Account ID: 101, To Account ID: 102

Amount: 1,000,000

Insufficient balance

📤 Expected Output:
✅ Successful Transfer:

javascript
 
Transaction Successful.  
$1000 transferred from Account 101 to 102.  
Updated Balances:  
Account 101: $4000  
Account 102: $6000
❌ Failed Transfer:

pgsql
 
Transaction Failed: Insufficient Balance.  
No changes were made to either account.
🎯 Learning Outcome:
Advanced use of Spring + Hibernate integration.

Ensuring transactional integrity in real-world applications.

Rollback mechanisms on failure.

