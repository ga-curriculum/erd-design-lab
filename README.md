# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) ERD Design Lab: Relational Database Modeling

## Lab Overview

In this lab, you will design an **Entity Relationship Diagram (ERD)** for a relational database system. The goal is to practice **SQL-based relational modeling**, focusing on identifying entities, defining attributes, and establishing correct relationships using **Primary Keys (PK)** and **Foreign Keys (FK)**.

You will analyze a real-world scenario and translate it into a well-structured ERD that includes **one-to-one (1–1)**, **one-to-many (1–M)**, and **many-to-many (M–M)** relationships.

⚠️ This lab focuses on **design only**. You will not write SQL queries or create tables.

---

## Learning Objectives

By the end of this lab, you will be able to:

- Analyze a real-world problem and identify database entities
- Design entities with appropriate attributes
- Correctly assign Primary Keys (PK) to entities
- Establish Foreign Keys (FK) to represent relationships
- Model 1–1, 1–M, and M–M relationships
- Resolve many-to-many relationships using junction tables
- Apply relational database best practices in ERD design

---

## Scenario: Online Learning Management System

You are tasked with designing a database for an **Online Learning Management System (LMS)** used by a training institute. The platform allows students to enroll in courses, instructors to teach courses, and administrators to manage content and assessments.

The system must track users, courses, enrollments, assessments, and certifications while maintaining proper relational structure.

---

## Business Rules and Requirements

Read the requirements carefully and design your ERD accordingly.

### Core Entities and Descriptions

1. **Student**
   - Represents learners enrolled in the platform
   - Each student has personal and academic details

2. **Instructor**
   - Represents instructors who teach courses
   - Each instructor has professional details

3. **StudentProfile**
   - Stores extended profile information for a student
   - Each student has exactly one profile

4. **Course**
   - Represents a course offered on the platform
   - A course is taught by one instructor

5. **Enrollment**
   - Tracks which students are enrolled in which courses
   - A student can enroll in many courses
   - A course can have many students

6. **Assessment**
   - Represents quizzes or exams for a course
   - Each course can have multiple assessments

7. **Certification**
   - Represents a certificate issued upon course completion
   - A certification is issued to a student for a specific course

---

## Relationship Requirements

Your ERD must clearly represent the following relationships:

- **One-to-One (1–1)**
  - Each *Student* has exactly one *StudentProfile*
  - Each *StudentProfile* belongs to exactly one *Student*

- **One-to-Many (1–M)**
  - One *Instructor* can teach many *Courses*
  - One *Course* can have many *Assessments*
  - One *Student* can receive many *Certifications*

- **Many-to-Many (M–M)**
  - Students can enroll in many courses
  - Courses can have many students
  - This relationship must be resolved using the *Enrollment* entity

---

## Design Instructions

1. Identify **at least 7 entities** based on the scenario
2. Assign a **Primary Key (PK)** to each entity
3. Add relevant attributes to each entity (do not overcomplicate)
4. Define **Foreign Keys (FK)** to represent relationships
5. Resolve all many-to-many relationships using junction tables
6. Clearly label relationship cardinalities (1–1, 1–M, M–M)
7. Follow standard **SQL relational database design practices**

---

## Deliverables

- A complete **ERD diagram** (hand-drawn or digital)
- Clearly labeled entities, attributes, PKs, and FKs
- Clearly defined relationship lines and cardinalities

---

## Key Takeaways

- ERDs are essential for planning relational databases
- Primary Keys uniquely identify records in a table
- Foreign Keys establish relationships between tables
- One-to-one, one-to-many, and many-to-many relationships require different modeling approaches
- Many-to-many relationships must be resolved using junction tables
- Good ERD design leads to efficient and maintainable SQL databases

---

## Conclusion

This lab strengthens your ability to think like a database designer by translating real-world requirements into a structured relational model. Mastering ERD design is a critical step before writing SQL queries or building database-driven applications.

---

## Additional Resources

- **ERD Basics and Crow’s Foot Notation**  
  Learn how to read and design Entity Relationship Diagrams using standard Crow’s Foot notation:  
  [Understanding ER Diagrams](https://www.lucidchart.com/pages/er-diagrams)  
  [ERD Design Guide](https://www.visual-paradigm.com/guide/data-modeling/what-is-entity-relationship-diagram/)

- **Database Normalization (1NF, 2NF, 3NF)**  
  Explore the principles of database normalization and how they improve data integrity and reduce redundancy:  
  [Database Normalization Explained](https://www.geeksforgeeks.org/database-normalization/)  
  [Normalization Tutorial](https://www.studytonight.com/dbms/database-normalization.php)

- **Relational Database Design Best Practices**  
  Understand industry best practices for designing efficient and scalable relational databases:  
  [Relational Design Best Practices](https://www.sqlshack.com/relational-database-design-best-practices/)  
  [IBM Relational Database Design Guide](https://www.ibm.com/docs/en/db2/11.5?topic=design-relational-database)

- **Primary Key and Foreign Key Concepts**  
  Review how primary and foreign keys enforce data integrity in SQL databases:  
  [SQL Primary Key](https://www.w3schools.com/sql/sql_primarykey.asp)  
  [SQL Foreign Key](https://www.w3schools.com/sql/sql_foreignkey.asp)

- **Online ERD Design Tools**  
  Use free online tools to create and visualize ER diagrams:  
  [Draw.io](https://draw.io)  
  [DB Diagram](https://dbdiagram.io)  
  [ERDPlus](https://erdplus.com)

