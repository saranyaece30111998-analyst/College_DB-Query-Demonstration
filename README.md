
# 📊 College Database Project – SQL Query Demonstration

## 📌 Project Overview
This project demonstrates **SQL querying techniques** on a Student Database.  
It covers:
- Basic record retrieval
- DISTINCT, ALIAS, WHERE, IN, BETWEEN, LIKE operators
- Arithmetic operations on columns
- Filtering with NULL checks and logical conditions


---

## 🎯 Objectives
- Retrieve and display complete records from tables (Students, Courses, Enrollment).
- Extract unique values using DISTINCT.
- Improve readability with column aliases.
- Apply filtering conditions (WHERE, IN, BETWEEN, LIKE).
- Perform arithmetic operations on columns.
- Handle NULL values effectively.
- Demonstrate comparison operators (>, <>, NOT IN).



---

## 🛠 Tools Used
- **Database:** MySQL  
- **Tables:**
  - Students (student details: name, age, city, status)  
  - Courses (course name, credits)  
  - Enrollment (student-course mapping with enrollment date)



---

## 📂 Key Queries & Results

### 1. Basic Retrieval
```sql
SELECT * FROM Students;
SELECT * FROM Courses;
SELECT * FROM Enrollment;
```
<img width="835" height="842" alt="Screenshot 2026-06-05 112159" src="https://github.com/user-attachments/assets/88ef7f9c-0c8c-4c30-8016-a8c5412dfa20" />


---

### 2. DISTINCT Values
```sql
SELECT DISTINCT city FROM Students;
```
<img width="430" height="415" alt="Screenshot 2026-06-04 221948" src="https://github.com/user-attachments/assets/d5022e3f-3c0e-43c1-8c8e-22acd2360253" />

---

### 3. Aliases
```sql
SELECT name AS student_name, age, city AS location FROM Students;
```
<img width="533" height="427" alt="Screenshot 2026-06-04 222026" src="https://github.com/user-attachments/assets/f1d81f86-046d-4782-8b0c-e5869456fb98" />


---

### 4. Filtering
```sql
SELECT * FROM Students WHERE city = 'Chennai';
```
<img width="638" height="307" alt="Screenshot 2026-06-04 222202" src="https://github.com/user-attachments/assets/17ba6b70-d08c-47ce-b5f8-f68d28f6991f" />

```
SELECT * FROM Students WHERE age > 22;
```
<img width="676" height="346" alt="Screenshot 2026-06-04 222246" src="https://github.com/user-attachments/assets/e36f0a8a-adb4-49b9-a5d7-1b4cfa854cdc" />


---

### 5. Arithmetic Operations
```sql
SELECT name, age, age + 5 AS age_after_5yrs FROM Students;
```
<img width="546" height="555" alt="Screenshot 2026-06-04 222336" src="https://github.com/user-attachments/assets/07ac2b20-1604-4a78-a3be-5589d26d2104" />

```
SELECT Credits * 2 AS DoubledCredits, CourseName FROM Courses;
```
<img width="500" height="430" alt="Screenshot 2026-06-04 222412" src="https://github.com/user-attachments/assets/51548768-d85e-4940-9dc5-1693a130b143" />


---

### 6. Comparison Operators
```sql
SELECT CourseName, Credits FROM Courses WHERE Credits > 2;
```
<img width="417" height="402" alt="Screenshot 2026-06-04 222441" src="https://github.com/user-attachments/assets/ef43ee17-7cec-45ad-8593-4bd26eaa12b8" />

```
SELECT CourseName, Credits FROM Courses WHERE Credits <> 2;
```
<img width="488" height="372" alt="Screenshot 2026-06-04 222511" src="https://github.com/user-attachments/assets/06f4778d-3f5d-46fb-8e02-54c3e81ae3e1" />


---

### 7. Logical Conditions
```sql
SELECT * FROM Students WHERE age > 20 AND status = 'Active';
```
<img width="653" height="465" alt="Screenshot 2026-06-04 222537" src="https://github.com/user-attachments/assets/841f15c2-a8f2-4417-8b36-506f8aee7b41" />


---

### 8. NULL Handling
```sql
SELECT * FROM Students WHERE status IS NULL;
```
<img width="576" height="302" alt="Screenshot 2026-06-04 222604" src="https://github.com/user-attachments/assets/50573e6c-ce41-4fb8-a265-0bbae80f9a50" />

```
SELECT * FROM Students WHERE status IS NOT NULL;
```
<img width="673" height="565" alt="Screenshot 2026-06-04 222642" src="https://github.com/user-attachments/assets/43561410-0684-42c9-b7b8-0aeb8ea8038c" />


---

### 9. IN / NOT IN
```sql
SELECT * FROM Students WHERE city IN ('Delhi', 'Chennai');
```

```
SELECT * FROM Students WHERE city NOT IN ('Delhi');
```
<img width="725" height="527" alt="Screenshot 2026-06-04 222716" src="https://github.com/user-attachments/assets/927ab8eb-03c4-4a59-ba41-0a9e57ad4a58" />


---

### 10. BETWEEN
```sql
SELECT * FROM Students WHERE age BETWEEN 20 AND 24;
SELECT * FROM Enrollment WHERE enrollmentdate BETWEEN '2024-01-15' AND '2024-02-29';
```


---

### 11. LIKE Operator
```sql
SELECT * FROM Students WHERE name LIKE 'A%';
SELECT * FROM Courses WHERE CourseName LIKE '%Analysis%';
```


---

## ✅ Conclusion
This project demonstrates:
- Core SQL operations for data retrieval and filtering
- Use of operators (DISTINCT, ALIAS, WHERE, IN, BETWEEN, LIKE)
- Arithmetic and comparison logic in queries
- Handling NULL values for data quality checks.    

---

## 📧 Contact
Created by **Saranya**  
 

```
