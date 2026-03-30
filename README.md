# Medical-Data-History-SQL-Project
SQL project analyzing patient medical data, including queries for history, conditions and insigh

## 📌 Project Description
This project analyzes healthcare data using SQL to extract meaningful insights about patients, doctors, and hospital operations.

## 🎯 Objectives
- Analyze patient demographics
- Identify unique cities and provinces
- Find common diseases
- Understand hospital trends

## 🛠️ Tools Used
- MySQL

## 📊 Key Queries

### 🔹 Query-14
**Requirement:** Show unique cities where patients live in province_id 'NS'

```sql
SELECT DISTINCT city
FROM patients
WHERE province_id = 'NS';

### 🔹 Query-18
SELECT *
FROM patients
WHERE name LIKE 's%s';

### 🔹 Query-18
-- Update NULL allergies
UPDATE patients
SET allergies = 'NKA'
WHERE allergies IS NULL;

## 📊 Queries Included
- Query-5: Update NULL values
- Query-14: Unique cities in province 'NS'
- Query-18: Pattern matching

## ⚠️ Note
UPDATE query may show permission error, so COALESCE was used as alternative.
SELECT COALESCE(allergies, 'NKA')
FROM patients;

📌 Conclusion

This project demonstrates SQL skills in data analysis, filtering, aggregation, and handling NULL values.
Faced real-time database permission issues and handled them using alternative SQL approaches like COALESCE.




Handled real-time SQL permission errors using alternative approaches.
