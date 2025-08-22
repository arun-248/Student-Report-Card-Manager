# Student Report Card Manager

A Python-based console application for managing student grades and report cards with data persistence.

## 📋 Overview

The Student Report Card Manager is a console-based application that allows educators to:
- Add student records with multiple subject scores
- Update existing scores or add new subjects
- View detailed grade reports with averages and letter grades
- Delete student records
- Save and load data to/from a JSON file

## 🚀 Features

- **Student Management**: Add, update, view, and delete student records
- **Grade Calculation**: Automatic average calculation and letter grade assignment
- **Data Persistence**: Save and load data using JSON files
- **User-Friendly Interface**: Simple console menu for easy navigation
- **Input Validation**: Proper error handling for invalid inputs

## 🛠️ Installation

1. Ensure you have Python 3.6 or higher installed
2. Download all the project files
3. No additional dependencies required - uses only Python standard libraries


## 🎯 How to Use

### Running the Application

1. Open a terminal or command prompt
2. Navigate to the project directory
3. Run the application with: `python main.py`

### Menu Options

The application provides a menu with the following options:

1. **Add Student**: Create a new student record with name and subject scores
2. **Update Scores**: Modify existing scores or add new subjects for a student
3. **View Report**: Display a student's report card with average and grade
4. **Delete Student**: Remove a student record from the system
5. **Save Data**: Save all student data to a JSON file (grades.json)
6. **Load Data**: Load student data from a JSON file
7. **Exit**: Quit the application

### Grade Scale

- A: 90-100%
- B: 80-89%
- C: 70-79%
- D: 60-69%
- F: Below 60%

## 💾 Data Persistence

The application automatically handles data storage:
- Data is saved to `grades.json` in the same directory
- The file format is human-readable JSON
- Data is preserved between sessions when saved properly

## 🔧 Customization

You can easily modify:
- Grade thresholds in the `get_grade()` method
- Subject requirements by modifying the input validation
- File storage location by changing the filename parameter

## ❓ Troubleshooting

**Common issues:**
- File not found errors: Ensure you save data before exiting
- Invalid input errors: Follow prompt instructions carefully
- Permission errors: Check write permissions in the directory

**Note**: This application is designed for educational purposes and demonstrates object-oriented programming principles in Python with practical file I/O operations.

## For Google Colab Users

If running in Google Colab, use the provided helper functions to download and upload your grades.json file to persist data between sessions.

```python
# Download your data file
download_grades_file()

# Upload a previously saved data file
upload_grades_file()
