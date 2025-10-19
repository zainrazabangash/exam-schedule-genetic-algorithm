# Exams Schedule Generator Using Genetic Algorithm

This project creates exam schedules for university courses using a genetic algorithm. It makes sure no student has two exams at the same time and follows all the rules.

## What it does

The program takes a list of courses, students, teachers and classrooms. Then it uses a genetic algorithm to find the best way to schedule all exams. It makes sure:

- Every course gets an exam
- No student has two exams at the same time
- No teacher has two exams at the same time
- No classroom has two exams at the same time
- Students don't have exams back to back
- Friday 1-2pm break is respected

## Files

- `Exams_Schedule_Generator_GA.ipynb` - Main code file
- `Dataset/` - Contains all the data files
  - `courses.csv` - List of courses
  - `studentCourse.csv` - Which students are in which courses
  - `studentNames.csv` - Student names
  - `teachers.csv` - Teacher names
- `final_exam_schedule.csv` - Generated schedule (created after running)

## How to run

1. Open the notebook file
2. Run all cells
3. Check the final schedule

## Requirements

- Python 3.9+
- pandas
- numpy
- matplotlib

## How it works

The genetic algorithm tries different combinations of:
- Which course
- Which day
- What time
- Which classroom
- Which teacher

It keeps the best schedules and makes new ones by mixing the good ones together. After many tries, it finds a schedule that follows all the rules.

## Results

The program creates a schedule with 23 exams across 5 days. Each exam has its own classroom and teacher. No conflicts between students or teachers.

**Developer:** Muhammad Zain Raza, student of BS AI at FAST NUCES Islamabad