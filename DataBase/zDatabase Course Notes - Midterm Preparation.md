## Tutorial 1-2: Applications of Database & Database Concepts

### Question 1
**purpose of database in e-commerce**:
<pre>
- Inventory
- Product detail
- Customer detail
- Orders detail
  
- Personalisation
- Market trend
- Fraud detection
</pre>

These databases are used to:

<pre>
- Identify best seller / hot selling products
- Identify activity time for different customers (customer behaviour)
- Display product detail/ shipping status/ order status
- Identify frequently asked questions via chat
</pre>

<br></br>

### Question 2
**Q: You are trying to justify a computerised data management system to your supervisor. You work in a service industry that deals directly with customers. How could collecting information about your customers provide a competitive advantage? What kind of software would you need to detect trends and make predictions about customer activities?**

Competitive advantage through customer information:
<pre>
- Personalised services and offers
- Identifies market trends and adapts quickly (To know the best selling products)
- Enhances customer satisfaction and loyalty
</pre>

Software needed for trends and projections:
<pre>
- Customer Relationship Management (CRM) Systems: Salesforce, HubSpot
- Analytics Tools: Google Analytics, Tableau, PowerBI (Able to do the analysis according to your data)
- Machine Learning: TensorFlow, Scikit-learn
</pre>

<br></br>

### Question 3
**Q: Explain the relationship between information, data and knowledge. Use relevant examples for different organizations.**

#### Definitions:
<pre>
1. **Data**: Raw facts, unprocessed facts and figures without context or meaning (e.g: Student ID, Student Name, Student Email)
2. **Information**: Processed or organised data that has meaning and is useful for analysis or decision-making
3. **Knowledge**: Insights, expertise, or understanding derived from the application of information in a particular context
</pre>

Examples by Application areas:
>[!TIP]
>You Need To Know At Least THREE (3) Application Areas
><pre>1. healthcare
> 2. finance
> 3. airline
> 4. university
> 5. telecommunicaton
> 6. social media
> 7. e-commerce
> 8. inventory
> 9. library
></pre>


**Healthcare Facility**:
- Data: Patient's vital signs (blood pressure: 120/80 mmHg, temperature: 98.6°F, heart rate: 72 bpm)
- Information: Vital signs indicate patient's condition is stable
- Knowledge: Doctor knows these signs are within normal ranges and can decide on treatment

**Institution of Higher Learning**:
- Data: Students' grades in a semester (85, 90, 78, 92)
- Information: Class average is 86%, 10% scored below 70%
- Knowledge: Faculty understands lower-performing students need additional support

**Law Enforcement Agency**:
- Data: Records of criminal activities in a city
- Information: Analysis shows burglaries peak between 8 PM and midnight
- Knowledge: Officials deploy additional patrols during peak hours

<br></br>

### Question 4
**Q: How is a file-based system different from a database management system?**

File System:
- Many separate and unrelated files
- Files normally not sharable

Database:
- Logically related data stored in a single logical repository
- Data is not owned by any individual department
- Access to data controlled by DBMS

<br></br>

### Question 5
**Q: Lei Tai Kor runs a convenience store business (EasBuy Sdn Bhd), selling daily use and household items. Currently, he uses a system written entirely in C++ to monitor his business transactions and inventories. He plans to expand his business in the near future to nearby housing estates and if that proves successful, he will then expand to nearby cities. Explain with relevant examples THREE problems that EasBuy will face when he tries to expand the business due to the file-base system that he is using now. Also explain how a database system can overcome these problems.**

Problems with file-based system:
1. require more complex coding to locate files
2. Duplicate of data appears frequently
3. Data ont updated synchrously (data inconsistency)
4. Excessive program maintenance required
5. data structure dependence issues arise

Database solutions:
1. Simplified data access with centralised management
2. Flexible data structure and reduced coding complexity
3. No uncontrolled redundancy - only one database
4. Programs can be maintained easily
5. DBMS allows modification of data dependence or database structure without affecting operations

<br></br>

### Question 6
**Q: What is data redundancy, and which characteristics of the file system can lead to it?**

Data redundancy is the duplication of data in multiple places, such as in a database system. It can occur:
- Intentionally or accidentally
- When unnecessarily duplicated data are found in the database

Causes in file systems:
1. Lack of normalization: Data may be repeatedly stored in multiple places without proper organization. For example, customer addresses might appear in several files or records
2. Poor file structure or organization: The same data might be stored in multiple files, folders, or directories
3. Poor design of the file-based system leading to unnecessary duplication

<br></br>

### Question 7
**Q: Explain any 5 types of databases with reference to the number of supported users. Also explain the locations of databases.**

Types based on number of supported users:
1. Single-User Database: Supports 1 user at a time
2. Multi-User Database: Supports multiple users at the same time
3. Desktop Database: Supports single users and designed for use on personal computers
4. Workgroup Database: Supports a small group of users or a single department
5. Enterprise Database: Supports a large group of users or entire organisations

Locations of Database:
1. Centralised Database: Only involves one database server and it is accessible by every device
2. Distributed Database: Database that is allocated as a distributed site

<br></br>

### Question 8
**Q: What is a DBMS, and what are its functions?**

A DBMS is a software suite that creates, processes, and administers databases. It has features to:
1. Create and process forms
2. Process user queries
3. Create and process reports
4. Execute application logic
5. Control applications

<br></br>

# Tutorial 3-5: Data Models (Entity Relationship Diagram)

### Question 1
**Q: What are models? Provide some examples of models. Why is data model important? Provide a logical view of data which stores supplier details.**

Models Definition:
Data model is a representation, usually graphical, of a real-world data structure.

Examples:
- Physical Models: Scale models of buildings or airplanes
- Data Models: Frameworks for organizing data within databases, like relational models, hierarchical models, object-oriented models, and entity-relationship (ER) models

Importance of data models:
1. Acts as a communication tool to facilitate interaction among system designers, applications programmers, and end users
2. Act as foundation for good database design
3. Data model provides the whole view of data for end users
4. Data model organises data for various users who have different needs for data

Logical view of supplier details:
Key Field:
- Supplier_ID: This uniquely identifies each supplier record

Non-Key Fields:
- Supplier_Name: The name of the supplier company
- Contact_Person: The main contact person at the supplier
- Phone_Number: The phone number to contact the supplier
- Email_Address: The supplier's email address for correspondence
- City: The city where the supplier is located
- Country: The country of the supplier's location

### Question 2
**Q: Define what 'business rules' are. Give TWO examples of business rules used in a payment system. Explain FOUR main purposes of business rules.**

Business Rules Definition:
A business rule is a brief, precise, and unambiguous description of a policy, procedure, or principle within a specific organisation.

Main sources include:
- Company managers
- Policy makers
- Department managers
- Written documentation (company procedures, standards, operations manuals)

Examples in payment system:
1. A single account can have multiple invoices, but each invoice must belong to one and only one account
2. A single invoice can only belong to one and only one payment, each payment belongs to one and only one invoice

Four main purposes:
1. They standardise the company's view of data
2. They serve as a communication tool between users and database designers
3. They allow database designers to understand the nature, role, and scope of data
4. They help designers to understand business processes

### Question 3
**Q: Create a Crow's Foot ERD to include the following business rules for the ProdCo company. List any FOUR characteristics of a relation in a relational database model.**

Business Rules:
- Each sales representative writes many invoices
- Each invoice is written by one sales representative
- Each sales representative is assigned to one department
- Each department has many sales representatives
- Each customer can generate many invoices
- Each invoice is generated by one customer

Characteristics of a relation in a relational database model:
1. Two-dimensional structure - rows and columns
2. Rows represent a single entity
3. Columns represent attributes/fields
4. Tables must have attributes to indicate Primary Key, Foreign Key, Composite Key

# Tutorial 3-5: Data Models (Continued)

### Question 4
**Q: Using the Microsoft Access Tiny College relational diagram as your guide, identify each relationship type and write all of the business rules.**

The relationships in the Tiny College database are structured as follows:

Course to Class relationship:
- A course can be offered in many classes
- Each class is associated with one course
- This creates a one-to-many relationship between course and class

Class to Enrollment relationship:
- A class can have many enrollments
- Each enrollment is associated with one class
- This establishes a one-to-many relationship between class and enrollment

Student to Enrollment relationship:
- A student can enroll in many classes
- Each enrollment is associated with one student
- This forms a one-to-many relationship from student to enrollment

### Question 5
**Q: Create an ERD and revised ERD for ROBCOR cinema based on these business rules. Provide a list of attributes for each entity.**

Business Rules for ROBCOR Cinema:
- A cinema can play many movies
- Each movie can be played at many cinemas
- Date and time of a movie played at a particular cinema must be recorded
- Each ticket is referred to only one movie
- Each movie can issue many tickets
- Each ticket may or may not be reserved by an audience
- Each audience can reserve many tickets

Attributes for entities:
1. Movie:
   - Movie ID (PK)
   - Title
   - Actors
   - Category

2. Cinema:
   - Cinema Code (PK)
   - Cinema Name

3. Ticket:
   - Ticket No (PK)
   - Price
   - Seat No
   - IC (FK)
   - Movie ID (FK)

4. Audience:
   - IC (PK)
   - Name
   - Contact No

5. Movie time:
   - Movie ID (FK)
   - Cinema Code (FK)
   - Time
   - Date

### Question 6
**Q: Draw an ERD and provide DBDL for a housing property based on the given business rules.**

Business Rules:
- A buyer can purchase many condominium units
- A unit can be owned by many shared owners
- A condominium unit has many rooms
- A room may have zero or many tenants
- Each tenant can rent only one room

Database Design Language (DBDL):
```
Buyer (B_Name, B_NRIC, B_Address, B_Phone, B_Email)
Own (B_NRIC*, Unit No*, Date_of_Purchase)
Unit (Unit No, Floor Level, Sqr Feet, No of room)
Room (Room No, Unit No*, Room type)
Tenants (T_NRIC, T_Name and T_Phone, Room No*)
```

# Tutorial 3-5: Data Models (Final Question)

### Question 9
**Q: For the city of Kuala Lumpur's high school system: What attributes are described for the entity STUDENT? Which attribute should you use as the STUDENT entity's identifier and why? What is the relationship between student and school? What is the relationship between schools and administrators? Draw the ERD for the system.**

System Description:
The city maintains information about:
- High schools
- Teachers and their university degrees
- Students
- Administrators
- Subjects taught

Student Attributes:
- Student number
- Name
- Home address
- Home telephone number
- Current grade
- Age

Identifier Selection for STUDENT:
Student number should be used as the identifier because:
- It is unique for each student
- It remains constant (never changes)
- It enables easy access to student's personal information

Relationships:
1. Student to School:
   - Many-to-one relationship
   - System only tracks current school attendance

2. School to Administrators:
   - One-to-many relationship
   - Each school has several administrators

Database Design Language (DBDL):
```
STUDENT (StudentId, Name, HomeAddress, HomeTelephoneNum, CurrentGrade, Age, SchoolName*)
SCHOOL (SchoolName, Address, YearBuilt, TelephoneNum, Size)
ADMINISTRATORS (AdminId, Name, TelephoneNum, OfficeNum, SchoolName*)
```

# Tutorial 6-8: Structured Query Language

### Simple Queries (Important for Midterm)
Key SQL commands and their usage:

1. Show manager for each department:
```sql
SELECT manager_id, department_id, department_name
FROM DEPARTMENTS;
```

2. Show employees named 'Alexander':
```sql
SELECT employee_id, first_name, last_name, email
FROM EMPLOYEES
WHERE first_name = 'Alexander';  -- Exactly Equal to Alexander

-- OR using LIKE (When there is a '%' MUST use LIKE)
SELECT employee_id, first_name, last_name, email
FROM EMPLOYEES
WHERE first_name LIKE 'Alexander%';  -- Any first name start with Alexander
```

Important LIKE patterns:
- `%` : Matches any sequence of characters
  - `'%Alexander'` - ends with Alexander
  - `'Alexander%'` - starts with Alexander
  - `'%Alexander%'` - contains Alexander
- `_` : Matches exactly one character
  - `'A_i'` - matches 'Ani', 'Abi', etc.

3. Department-specific queries:
```sql
SELECT employee_id, first_name, last_name
FROM EMPLOYEES
WHERE department_id = 170;

-- With salary condition and ordering
SELECT employee_id, first_name, last_name
FROM EMPLOYEES
WHERE department_id = 170
  AND salary < 10000
ORDER BY salary DESC;
```

4. Salary-based queries:
```sql
SELECT job_id, job_title
FROM JOBS
WHERE min_salary >= 15000;
```

Let me continue with the SQL examples from your course notes:

# Tutorial 6-8: Structured Query Language (Continued)

### Additional SQL Query Examples

5. Location-based queries:
```sql
-- Find locations with street address containing '8'
SELECT location_id, street_address, city
FROM LOCATIONS
WHERE street_address LIKE '%8%';

-- Find locations with specific postal code endings
SELECT postal_code, location_id, street_address, city 
FROM locations 
WHERE postal_code LIKE '%18' 
   OR postal_code LIKE '%28' 
   OR postal_code LIKE '%98';
```

6. Employment duration queries:
```sql
-- Find employees with 5-8 years of service
SELECT * 
FROM employees 
WHERE SYSDATE - hire_date BETWEEN 5*365 AND 8*365;

-- Alternative approach using MONTHS_BETWEEN
SELECT employee_id, start_date, end_date
FROM Employees
WHERE (MONTHS_BETWEEN(sysdate, hire_date) / 12) BETWEEN 5 AND 8;
```

### Key SQL Concepts to Remember for Midterm:

1. Basic Commands:
   - SELECT: Retrieves data from tables
   - CREATE TABLE: Creates new tables
   - UPDATE: Modifies existing records
   - DELETE: Removes records
   - INSERT: Adds new records
   - ORDER BY: Sorts results (ASC/DESC)

2. Comparison Operators:
   - Equal to (=): Exact match
   - LIKE: Pattern matching
   - BETWEEN: Range of values
   - IN: Multiple possible values

3. Wildcards in LIKE:
   - %: Represents any number of characters
   - _: Represents a single character

4. Date Functions:
   - SYSDATE: Current system date
   - MONTHS_BETWEEN: Calculates months between two dates

These SQL commands form the foundation for database manipulation and are essential for the midterm examination. The examples provided show common use cases and patterns that you might encounter in real-world database management scenarios.

Remember: When using comparison operators, be particularly careful with:
- String comparisons (use LIKE with wildcards)
- Date comparisons (consider using appropriate date functions)
- Numeric comparisons (use appropriate operators like =, <, >, BETWEEN)
