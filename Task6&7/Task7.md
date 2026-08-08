# Task7 - Relational Database Design
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

## Activity Table
- Primary Key: activityID
- Foreign Keys :
 - organizerID → Organizer(organizerID)
 - departmentID → StudentAffairs(departmentID)
 - categoryID → ActivityCategory(categoryID)

**Columns:** 

- activityID - INT
- title - VARCHAR(100)
- date - DATETIME
- location - VARCHAR(100)
- capacity - INT
- status - VARCHAR(50)
- organizerID - INT
- departmentID - INT
- categoryID - INT

## Registration Table
- Primary Key: registrationID
- Foreign Keys:
 - studentID → Student(studentID)
 - activityID → Activity(activityID)

**Columns:**

- registrationID - INT
- registrationDate - DATETIME
- status - VARCHAR(50)
- studentID - INT
- activityID - INT

## ActivityCategory Table
- Primary Key: categoryID

**Columns:**

- categoryID - INT
- categoryName - VARCHAR(100)


## Attendance Table
- Primary Key: attendanceID
- Foreign Keys:
- studentID → Student(studentID)
- activityID → Activity(activityID)

**Columns:**

- attendanceID - INT
- attendanceTime - DATETIME
- method - VARCHAR(50)
- studentID - INT
- activityID - INT

## Notification Table
- Primary Key: notificationID
- -Foreign Key: studentID → Student(studentID)

**Columns:**

- notificationID - INT
- message - VARCHAR(200)
- type - VARCHAR(50)
- date - DATETIME
- studentID - INT

## Certification Table 
- Primary Key: certificateID
- Foreign Key: studentID → Student(studentID)


**Columns:**

- certificateID - INT
- issueDate- DATETIME
- studentID - INT

## AcrivityReport Table
- Primary Key: reportID
- Foreign Key: studentID → Student(studentID)

**Columns:**

ReportID - INT
totalHours - INT
totalActivites - INT
generatedDate - DATETIME
srudentID - INT
