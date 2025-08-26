
# Exam Data Logger

A basic Python script for recording and displaying student exam grades using CSV files. It allows users to input multiple students' grades, saves the data to a file, and prints a formatted grade report to the console.

## Features

* Prompt-based input for student names and three exam scores
* Saves all entered data into a file named `grades.csv`
* Automatically writes headers to the CSV file
* Neatly displays all student records in a formatted table
* Designed for small-scale, manual entry and review of grades

## How It Works

1. The script prompts the user for the number of students to enter
2. For each student, it collects:

   * First name
   * Last name
   * Exam 1 grade
   * Exam 2 grade
   * Exam 3 grade
3. All records are saved to `grades.csv` in the current directory
4. Once data entry is complete, the script reads from the CSV file and prints all the records in a formatted table with aligned columns

## Sample Interaction

Enter the number of students: 2
Enter the student's first name: Alice
Enter the student's last name: Johnson
Enter Exam 1 grade: 85
Enter Exam 2 grade: 90
Enter Exam 3 grade: 88

Enter the student's first name: Bob
Enter the student's last name: Smith
Enter Exam 1 grade: 78
Enter Exam 2 grade: 82
Enter Exam 3 grade: 80

Data has been written to grades.csv.

## First Name      Last Name       Exam 1     Exam 2     Exam 3

Alice           Johnson          85         90         88
Bob             Smith            78         82         80

## Code Overview

**write\_grades()**
Prompts the user for student information and writes it to `grades.csv` with headers.

**read\_grades()**
Reads data from `grades.csv` and prints it in a formatted table.

**main()**
Calls both `write_grades()` and `read_grades()` functions in sequence.
