# Task 3

- Context Diagram
This is the Context Diagram for SAMS project.
What I did:
- Made the main process (0.0 SAMS System).
- Added entities: Student, Activity, Organizer and Student Affairs Department.
- Added data flows between entities and system (requests, details, approvals, and notifications).

<img width="604" height="415" alt="Context_Diagram" src="https://github.com/user-attachments/assets/c2b1ac25-3969-4c31-b4c0-c1b6324d7c2b" />

- Level-0 Data Flow Diagram (DFD)
 I created the Level-0 DFD for SAMS to show how data moves in the system.
  
What I added:

- Entities (3): Student, Activity Organizer, and Student Affairs.
- Processes (4): Manage Users, Manage Activities, Registration & Attendance, and Generate Reports.
- Data Stores (3): Users, Activities, and Enrolments.
- Data Flows: Arrows connecting all users, processes, and stores.

 <img width="519" height="1287" alt="sams_level0_dfd" src="https://github.com/user-attachments/assets/512a515c-fe89-4514-90c2-4105ff0565ce" />



I designed the Level-1 Data Flow Diagram (DFD) for the Manage Activities process (Process 2.0)

It breaks down the main process into three sub processes:

2.1 Create Activity: Handles new activity submissions from the Activity Organizer and saves them as draft records in the Activities Store (D2).
2.2 Approve Activity: Fetches pending requests for Student Affairs to approve or reject updating the activity status accordingly.
2.3 Update Cancel Activity: Processes update or cancellation requests from the Organizer by retrieving existing activity data and saving the final changes back to the database.







<img width="773" height="747" alt="Level-1 DFD for Manage Activities process" src="https://github.com/user-attachments/assets/956804de-014f-4838-b012-ee72a9b67eba" />


These diagrams model student registration, attendance, and reporting in SAMS. Process 3.0 allows students to browse events, confirm bookings, and record attendance via QR code to receive certificates. Process 4.0 uses enrollment and user data to track participation history, generate graduation transcripts, and deliver engagement reports for Student Affairs.

<img width="1183" height="564" alt="4 0" src="https://github.com/user-attachments/assets/58a3eb55-2cd8-4c7a-b53f-0ad8c8802745" />
<img width="897" height="1154" alt="3 0" src="https://github.com/user-attachments/assets/b2d9ff26-992a-4097-b260-75a7e87e2901" />










