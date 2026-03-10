# 📘Course Eligibility Knowledge-Based System

## 👤Student Information
Name: Angel Wesonga  
Registration Number: 672296  
Course: Knowledge Based Systems  

## 🧠Overview
This project demonstrates a simple Knowledge Based System that determines whether a student is eligible for certain university courses.

The system uses two reasoning techniques:
- Forward Chaining (data driven reasoning)
- Backward Chaining (goal driven reasoning)

The program is implemented using Python and executed in a Jupyter Notebook.

## 🧩Knowledge Representation

Facts represent information about a student such as:

Completed courses  
GPA performance  

Example facts:

Programming I  
Statistics  
High GPA  

Rules define conditions that allow eligibility for other courses.

Example rule:

IF Programming I AND Statistics  
THEN Eligible for Machine Learning Basics

## 🔄Forward Chaining

Forward chaining starts with known facts and repeatedly applies rules to infer new facts.

Example:

Initial Facts:
Programming I  
Statistics  

Rule Applied:

IF Programming I AND Statistics  
THEN Machine Learning Basics

New fact inferred:
Machine Learning Basics

The process continues until no more new facts can be generated.

## 🔙Backward Chaining

Backward chaining begins with a goal and checks whether the required conditions can be satisfied.

Example query:

Is the student eligible for Machine Learning Basics?

The system checks which rule produces that goal and verifies if the conditions are satisfied by existing facts.

The result is returned as:

PROVED or NOT PROVED

## ✅Expected Output

Example output:

Student: Angel  
Completed Courses: Programming I, Statistics  
GPA: 3.2  

Forward Chaining Results:
Rule Fired → Machine Learning Basics  

Final Eligible Courses:
Machine Learning Basics  

Backward Chaining Query:
Is the student eligible for Machine Learning Basics?  

Result: PROVED

## ▶️How to Run

1. Open the notebook file `course_eligibility_kbs.ipynb`
2. Run all cells from top to bottom
3. Observe the forward chaining and backward chaining outputs