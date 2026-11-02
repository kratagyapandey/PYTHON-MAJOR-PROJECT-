# Student Management and Performance Analytical System

A simple command-line Student Management System made in Python using OOP. You can add students, enter their marks, and see a report card with total, average and grade. All data is saved in a JSON file, so it stays even after you close the program.

## Features

- Add a student (roll number, name, age, course and marks of any number of subjects)
- Search a student's report card by roll number
- View report cards of all students
- Delete a student record (asks for confirmation first)
- Total, average and grade are calculated automatically
- Data is saved in `students.json` and loaded again on the next run
- Handles basic errors like blank or duplicate roll numbers and wrong number input

## Requirements

- Python 3.8 or above
- No external libraries needed (only `json` and `os`, which come with Python)

## How to Run

```bash
git clone https://github.com/kratagyapandey/PYTHON-MAJOR-PROJECT-.git
cd PYTHON-MAJOR-PROJECT-
python main.py
```

## Menu

```
1. Create Student Object (Add Details & Marks)
2. Search & Display Student Report
3. Display All Students Complete Reports
4. Delete Student Record
5. Exit
```

## Grading

Grade is based on the average marks.

| Average | Grade |
|---------|-------|
| 90 and above | A+ |
| 80 - 89 | A |
| 70 - 79 | B |
| 60 - 69 | C |
| 50 - 59 | D |
| Below 50 | F (Fail) |

## Sample Output

```
==================================================
          STUDENT COMPLETE REPORT CARD
==================================================
 Roll Number   : 101
 Name          : Kratagya Pandey
 Age           : 20
 Course        : BCA
--------------------------------------------------
 Marks List    : [85.0, 90.0, 78.0, 92.0, 88.0]
 Total Marks   : 433.0
 Average Marks : 86.60
 Grade         : A
==================================================
```

## How the Data is Stored

Records are saved in `students.json` with the roll number as the key:

```json
{
    "101": {
        "roll_no": "101",
        "name": "Kratagya Pandey",
        "age": 20,
        "course": "BCA",
        "marks": [85.0, 90.0, 78.0, 92.0, 88.0]
    }
}
```

## Concepts Used

- Classes and objects (`Student`, `StudentManagementSystem`)
- Constructor and class method (`from_dict`)
- File handling with JSON
- Exception handling (`try / except`)

## Future Plans

- Edit existing student records
- Check that marks are between 0 and 100
- Store subject names along with marks
- Export report cards to PDF or CSV
- Make a GUI version using Tkinter

## Author

Kratagya Pandey

Project Repository: [PYTHON-MAJOR-PROJECT-](https://github.com/kratagyapandey/PYTHON-MAJOR-PROJECT-)
