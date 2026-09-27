# Task 8 - Simple Data Filtering

## AI & ML Internship

**Author:** Swati Muttannavar  
**Task:** 8 - Simple Data Filtering  
**Level:** 1  
**Day:** 8  

## 1. Project Overview

This project demonstrates how structured student records can be filtered using Python conditions.

The student records are represented as a **list of dictionaries**. Each record contains:

- Student ID
- Name
- Age
- Department
- Marks

The project performs filtering based on marks, age, department, and combinations of multiple conditions.

## 2. Objective

The objective is to understand how conditional statements can be used to select only the records that satisfy specific requirements.

## 3. Tools Used

- Python 3
- Jupyter Notebook
- Optional: Pandas for the DataFrame example

## 4. Project Files

```text
Simple_Data_Filtering_Task8/
│
├── simple_data_filtering.py
├── simple_data_filtering.ipynb
└── README.md
```

## 5. Filtering Operations

The project includes the following filters:

1. **Marks filter:** students with marks greater than or equal to 80.
2. **Age filter:** students whose age is less than or equal to 21.
3. **Department filter:** students belonging to the CSE department.
4. **Multiple conditions:** CSE students with marks greater than or equal to 80.
5. **Multiple conditions:** students aged 21 or below with marks of at least 75.

## 6. Example Logic

A single condition can be written as:

```python
high_scorers = [
    student for student in students
    if student["marks"] >= 80
]
```

Multiple conditions can be combined using `and`:

```python
cse_high_scorers = [
    student for student in students
    if student["department"] == "CSE"
    and student["marks"] >= 80
]
```

## 7. How to Run the Python File

Open a terminal in the project folder and run:

```bash
python simple_data_filtering.py
```

## 8. How to Run the Jupyter Notebook

Install Jupyter if required:

```bash
pip install notebook
```

Start Jupyter:

```bash
jupyter notebook
```

Then open:

```text
simple_data_filtering.ipynb
```

Run the cells from top to bottom.

## 9. Expected Result

The program displays:

- All student records
- Students scoring 80 or above
- Students aged 21 or below
- CSE students
- CSE students scoring 80 or above
- Students aged 21 or below with marks of at least 75
- A filtering summary with record counts

## 10. Concepts Learned

- Lists
- Dictionaries
- List comprehensions
- `if` conditions
- Comparison operators
- Logical operator `and`
- Filtering structured data
- Basic DataFrame filtering concept

## 11. Interview Questions

### What is data filtering?

Data filtering is the process of selecting only the records that satisfy one or more specified conditions.

### How would you filter a Pandas DataFrame?

For example:

```python
result = df[df["marks"] >= 80]
```

For multiple conditions:

```python
result = df[
    (df["department"] == "CSE") &
    (df["marks"] >= 80)
]
```

### What is the difference between filtering and sorting?

**Filtering** selects or removes records based on conditions.

**Sorting** changes the order of records according to one or more columns or values.

## 12. Conclusion

This project demonstrates a simple and practical way to filter structured student data using Python. It builds a foundation for working with larger datasets and prepares for more advanced data analysis using Pandas and other data-processing tools.
