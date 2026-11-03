# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/1abf5e73-8715-4b06-a24d-ec5df98c2cf7" />
<img width="982" height="667" alt="WhatsApp Image 2026-11-02 at 10 29 53 PM" src="https://github.com/user-attachments/assets/b08212e4-8e28-49e5-a8f5-74259bc5d5f8" />


### Entities and Attributes

## Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
| Member | M_ID (PK), Name, Type, Start_date, Email_ID, Phone | Stores member details |
| Membership | M_ID (PK, FK), Type, Start_date, End_date, Fee | Membership details linked to Member |
| Program | P_ID (PK), Name, Description, Duration | Fitness programs such as Yoga, Zumba, Weight Training |
| Trainer | T_ID (PK), Name, Designation, Phone | Trainer details |
| Session | S_ID (PK), Date, Time, Status | Personal training session details |
| Payment | Payment_ID (PK), Amount, Payment_date, Status | Payment details |
| Attendance | A_ID (PK), Date, Status | Records session attendance |

## Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|-------------|---------------|-------|
| Member — Enrolls — Program | M:N | Partial on both sides | Members can enroll in multiple programs |
| Member — Holds — Membership | 1:N | Membership: Total; Member: Partial | A member can hold membership records over time |
| Membership — Makes — Payment | 1:N | Payment: Total; Membership: Partial | Membership payments are recorded |
| Payment — For — Session | N:1 | Payment: Total; Session: Partial | A payment is for a training session |
| Trainer — Conducts — Session | 1:N | Session: Total; Trainer: Partial | A trainer can conduct multiple sessions |
| Session — Records — Attendance | 1:1 | Total on both sides | Each session has an attendance record |
| Program — Handled by — Trainer | M:N | Partial on both sides | Programs can have multiple trainers |

### Assumptions
- 
- 
- 

---

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
<img width="1600" height="1520" alt="image" src="https://github.com/user-attachments/assets/d123b435-1845-46e4-bb52-439e7cde0a8c" />

<img width="1462" height="692" alt="WhatsApp Image 2026-11-02 at 10 30 03 PM" src="https://github.com/user-attachments/assets/aadff396-68d9-4d4a-bb04-b2f81e5a2519" />

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
<img width="1600" height="1356" alt="image" src="https://github.com/user-attachments/assets/5211fa68-0faf-4cec-a0d8-de5fb590b7b6" />
<img width="942" height="722" alt="WhatsApp Image 2026-11-02 at 10 30 10 PM" src="https://github.com/user-attachments/assets/c87ea901-28da-4602-a752-8367a576394a" />

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
