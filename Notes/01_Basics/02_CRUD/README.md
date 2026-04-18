# CRUD Operations in PostgreSQL

CRUD means the four basic operations used in databases:

- **Create** → Used to create table and insert new data  
- **Read** → Used to fetch/view data  
- **Update** → Used to modify existing data  
- **Delete** → Used to remove data  

These operations are used in almost every database project.

---

## 1️⃣ CREATE

Create is used to create a new table and add records.

### Syntax

CREATE TABLE table_name (column1 datatype, 
column2 datatype);

### Example

CREATE TABLE students(
student_name CHAR(50),
student_age INT,
div CHAR(1)
);

### Insert Data Syntax

INSERT INTO table_name 
VALUES(value1, value2, value3);

### Example

INSERT INTO students
VALUES ('Akanksha',20,'A');

---

## 2️⃣ READ

Read is used to display data from table.

### Syntax

SELECT column_name FROM table_name;

OR

SELECT * FROM table_name;

### Example

SELECT student_name FROM students;

SELECT * FROM students;

---

## 3️⃣ UPDATE

Update is used to change old data.

### Syntax

UPDATE table_name  
SET column_name = new_value  
WHERE condition;

### Example

UPDATE students
SET student_name = 'Lavale Akanksha'
WHERE student_name = 'Akanksha';

### Check Updated Data

SELECT * FROM students;

---

## 4️⃣ DELETE

Delete is used to remove records from table.

### Syntax

DELETE FROM table_name
WHERE condition;

### Example

DELETE FROM students
WHERE student_name = 'Lavale Akanksha';

---

## Important Notes

- SELECT * shows all columns.
- WHERE is important in UPDATE and DELETE.
- Without WHERE all rows may be affected.

---

## Output Example

| student_name      | student_age | div |
|-------------------|------------|-----|
| Lavale Akanksha   | 20         | A   |
