# Group-7-Big-Data
# Student Management System & Palindrome Checker

## Project Overview
This repository contains two Python programs developed as a collaborative group project:
1. *Student Management System* - A console application for managing student information and calculating grade averages
2. *Palindrome Checker* - A utility to check if a given string reads the same forwards and backwards

---

## 📋 Table of Contents
- [Features](#features)
- [Installation & Setup](#installation--setup)
- [Usage Guide](#usage-guide)
- [Code Structure & Documentation](#code-structure--documentation)
- [Testing & Validation](#testing--validation)
- [Team Contributors](#team-contributors)

---

## 🚀 Features

### Student Management System
- Input student information (name, age, grades)
- Calculate average grades automatically
- Display formatted student reports
- Handle multiple students (up to 3 in current implementation)

### Palindrome Checker
- Check if any string is a palindrome
- Case-sensitive palindrome detection
- Interactive console interface

---

## 💻 Installation & Setup

### Prerequisites
- Python 3.6 or higher installed on your system
- No additional libraries or dependencies required
- Basic understanding of command line/terminal usage

### Installation Steps
1. *Clone the repository:*
   bash
   git clone https://github.com/gasar0/Group-7-Big-Data.git
   cd Group-7-Big-Data
   

2. python --version
   jupyter --version
   

3. *Run the program:*
    jupyter notebook "StudentManagement&Palindrome.ipynb"
   

### System Requirements
- *Operating System*: Windows, macOS, or Linux
- *Python Version*: 3.6+
- *Memory*: Minimal requirements (< 50MB)
- *Storage*: Less than 1MB for source code

### Quick Start
No compilation needed! Simply download the Python files and run them directly from your terminal or command prompt.

---

### Running the Student Management System

1. *Execute the program:*
   bash
   python main.py
   

2. *Follow the interactive prompts:*
   - The system will ask for information for 3 students
   - Enter each student's name, age, and 3 course grades
   - The program automatically calculates and displays results

3. *Sample Session:*
   
   Enter information for student 1:
   Enter student name: Aimee
   Enter student age: 21
   Enter grade for course 1: 78
   Enter grade for course 2: 82
   Enter grade for course 3: 90
   
   --- Student Information ---
   Name: Aimee
   Age: 21
   Grades: [78.0, 82.0, 90.0]
   Average Grade: 83.33
   

### Running the Palindrome Checker

1. *The palindrome checker runs automatically after the student system*

2. *Enter a string when prompted:*
   
   Enter a string: madam
   Yes, it is a palindrome
   

3. *Example Test Cases:*
   - "madam" → Yes, it is a palindrome
   - "hello" → No, it is not a palindrome
   - "racecar" → Yes, it is a palindrome
   - "Python" → No, it is not a palindrome

### Input Guidelines
- *Student names*: Any text string
- *Student ages*: Positive integers only
- *Grades*: Decimal numbers (0-100 recommended)
- *Palindrome strings*: Any text (case-sensitive)

---

### Student Management System Architecture

#### input_student_info()
- *Purpose*: Collects student information from user input
- *Returns*: Dictionary containing student data
- *Data Structure*: {"name": str, "age": int, "grades": list}
- *Process*: Prompts for name, age, and 3 course grades sequentially

#### calculate_average(grades)
- *Purpose*: Computes the arithmetic mean of student grades
- *Parameters*: grades (list of float values)
- *Returns*: Float representing the average grade
- *Algorithm*: sum(grades) / len(grades)

#### display_student_info(student)
- *Purpose*: Formats and displays student information
- *Parameters*: student (dictionary with student data)
- *Output*: Formatted console display with name, age, grades, and average
- *Formatting*: Average rounded to 2 decimal places

#### student_management_system()
- *Purpose*: Main program orchestrator
- *Process*: 
  1. Initializes empty students list
  2. Loops 3 times to collect student data
  3. Calculates averages for each student
  4. Displays all student information

### Palindrome Checker Architecture

#### check_palindrome()
- *Purpose*: Determines if a string reads the same forwards and backwards
- *Algorithm*: String comparison using slice notation text[::-1]
- *Input*: User-provided string via console
- *Output*: Boolean result displayed as user-friendly message
- *Comparison*: Case-sensitive exact match

### Data Flow
1. *Input Collection* → *Processing* → *Storage* → *Display*
2. *User Input* → *Validation* → *Calculation* → *Output Formatting*

---
