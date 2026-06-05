
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


---

### 2. DISTINCT Values
```sql
SELECT DISTINCT city FROM Students;
```

---

### 3. Aliases
```sql
SELECT name AS student_name, age, city AS location FROM Students;
```


---

### 4. Filtering
```sql
SELECT * FROM Students WHERE city = 'Chennai';
SELECT * FROM Students WHERE age > 22;
```


---

### 5. Arithmetic Operations
```sql
SELECT name, age, age + 5 AS age_after_5yrs FROM Students;
SELECT Credits * 2 AS DoubledCredits, CourseName FROM Courses;
```


---

### 6. Comparison Operators
```sql
SELECT CourseName, Credits FROM Courses WHERE Credits > 2;
SELECT CourseName, Credits FROM Courses WHERE Credits <> 2;
```


---

### 7. Logical Conditions
```sql
SELECT * FROM Students WHERE age > 20 AND status = 'Active';
```


---

### 8. NULL Handling
```sql
SELECT * FROM Students WHERE status IS NULL;
SELECT * FROM Students WHERE status IS NOT NULL;
```


---

### 9. IN / NOT IN
```sql
SELECT * FROM Students WHERE city IN ('Delhi', 'Chennai');
SELECT * FROM Students WHERE city NOT IN ('Delhi');
```


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
  
  
- `screenshots/comparison_operators.png`  
- `screenshots/logical_conditions.png`  
- `screenshots/null_handling.png`  
- `screenshots/in_not_in.png`  
- `screenshots/between.png`  
- `screenshots/like_operator.png`  
- `screenshots/conclusion.png`

---

## 📧 Contact
Created by **Saranya**  
📩 Email: [your-email@example.com]  
🔗 LinkedIn: [your-linkedin-profile]  
```
