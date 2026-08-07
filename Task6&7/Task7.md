#Task7 - Relational Database Design
This task presents the relational database design the student activity management system. The design includes tables, primary keys, foreign keys, appropriate data types, and normalization up to Third Normal Form (3NF).

## User Table 
- Primary Key: userID
  
**Columns:**

- userID - INT
- name - VARCHAR(100)
- email - VARCHAR(100)

## Student Table
 - Primary Key: studentID
 - Foreign Key: userID → User(userID)
   
 **Columns:**

 - studentID - INT
 - userID - INT
 - activityHours - INT

  ## Organizer Table
  - Primary Key: organizerID
  - Foreign Key: userID → User(userID)
    
  **Columns:**
  
  - organizerID - INT
  - userID - INT
 
  ## StudentAffairs Table
  - Primary Key: departmentID
  - Foreign Key: userID → User(userID)
    
  **Columns:**
  
  - departmentID - INT
  - userID - INT
  - departmentName - VARCHAR(100)
