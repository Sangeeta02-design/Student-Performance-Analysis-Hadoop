Large-Scale Student Performance Analysis Using Hadoop, MapReduce and Python

Project Overview

This project focuses on analyzing large-scale student academic data using Apache Hadoop, HDFS, MapReduce and Python. It processes 10,000 student records to identify academic performance patterns, attendance trends and students who may be at academic risk.

The project demonstrates how distributed storage and processing can be used to analyze educational data efficiently.

Objectives

Analyze student performance across different departments.

Compare academic performance semester-wise.

Identify grade distribution among students.

Analyze attendance patterns.

Identify students who may be at academic risk.

Generate reports to support data-driven academic decisions.

Technologies Used

Apache Hadoop 3.4.2 – Distributed data processing framework.

HDFS – Distributed storage of student datasets and results.

MapReduce – Large-scale data processing.

Python – Mapper and Reducer implementation.

Kali Linux – Project execution environment.

Microsoft Excel – Data visualization and dashboard creation.

Dataset Description

The project uses a dataset containing 10,000 student records with the following attributes:

Student ID

Student Name

Department

Semester

Attendance Percentage

Study Hours per Week

Assignment Score

Exam Score

Project Workflow

Collected and prepared the student dataset.

Stored the dataset in Hadoop Distributed File System (HDFS).

Implemented Mapper and Reducer programs using Python.

Processed the dataset using MapReduce.

Generated five analytical outputs.

Stored the results in HDFS.

Prepared CSV reports and an Excel dashboard.

Key Analyses Performed

1. Department-Wise Performance

Analyzes academic performance across different departments.

2. Semester-Wise Performance

Compares student performance across semesters.

3. Grade Distribution

Shows the distribution of students across different grade categories.

4. Attendance Analysis

Analyzes student attendance patterns.

5. At-Risk Student Identification

Identifies students who may require additional academic support based on performance indicators.

Project Structure

Student-Performance-Analysis-Hadoop/
│
├── dataset/
├── mapper/
├── reducer/
├── reports/
├── dashboard/
├── README.md
└── screenshots/

How to Run

1. Start Hadoop Services

start-dfs.sh

2. Verify Hadoop Services

jps

3. View HDFS Project Directory

hdfs dfs -ls /student_performance

4. View MapReduce Results

hdfs dfs -cat /student_performance/mapreduce_department_output_v2/part-*
hdfs dfs -cat /student_performance/mapreduce_semester_output/part-*
hdfs dfs -cat /student_performance/mapreduce_grade_output/part-*
hdfs dfs -cat /student_performance/mapreduce_attendance_output/part-*
hdfs dfs -cat /student_performance/mapreduce_atrisk_output/part-*

Results

The project successfully performs five types of student performance analysis using Hadoop and Python-based MapReduce processing. The generated outputs are stored in HDFS and used to prepare reports and an Excel dashboard.

Future Scope

Develop an interactive web-based dashboard.

Apply Machine Learning to predict student academic performance.

Integrate real-time student performance monitoring.

Improve early identification of academically at-risk students.
