# 🎓 Large-Scale Student Performance Analysis Using Hadoop, MapReduce & Python

<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Hadoop-3.4.2-yellow?logo=apachehadoop&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/MapReduce-Data%20Processing-orange" />
  <img src="https://img.shields.io/badge/HDFS-Distributed%20Storage-green" />
  <img src="https://img.shields.io/badge/Platform-Kali%20Linux-blue?logo=kalilinux&logoColor=white" />
</p>

## 📌 Project Overview

**Large-Scale Student Performance Analysis** is a Big Data Analytics project that analyzes **10,000 student records** using Apache Hadoop, HDFS, MapReduce and Python.

The project focuses on discovering meaningful patterns in student academic performance, analyzing attendance trends, comparing departmental results and identifying students who may be at academic risk.

It demonstrates how Big Data technologies can efficiently process and analyze large educational datasets.

## 🎯 Project Objectives

- Analyze academic performance across different departments.
- Compare student performance semester-wise.
- Understand grade distribution among students.
- Evaluate student attendance patterns.
- Identify academically at-risk students.
- Generate meaningful reports for data-driven decision-making.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Apache Hadoop 3.4.2 | Distributed data processing |
| HDFS | Distributed data storage |
| MapReduce | Large-scale data analysis |
| Python | Mapper and Reducer implementation |
| Kali Linux | Development environment |
| Microsoft Excel | Data visualization and dashboard |

## 📂 Dataset Description

The project uses a dataset containing **10,000 student records** with the following attributes:

| Attribute | Description |
|---|---|
| student_id | Unique student identifier |
| student_name | Student name |
| department | Academic department |
| semester | Current semester |
| attendance_percent | Attendance percentage |
| study_hours_per_week | Weekly study hours |
| assignment_score | Assignment marks |
| exam_score | Examination marks |

## ⚙️ Project Workflow

1. **Data Collection:** Prepare the student performance dataset.
2. **Data Storage:** Store the dataset in Hadoop Distributed File System (HDFS).
3. **Data Processing:** Use Python Mapper and Reducer programs.
4. **MapReduce Execution:** Process student records using distributed computation.
5. **Data Analysis:** Perform five different analytical operations.
6. **Result Storage:** Save processed outputs in HDFS.
7. **Visualization:** Prepare reports and an Excel dashboard.

## 📊 Key Analysis Performed

### 1. 🏢 Department-Wise Performance
Analyzes student academic performance across different departments to compare departmental results.

### 2. 📚 Semester-Wise Performance
Evaluates and compares student performance across different semesters.

### 3. 🏆 Grade Distribution
Examines the distribution of students across different grade categories.

### 4. 📈 Attendance Analysis
Studies attendance patterns and their relationship with academic performance.

### 5. ⚠️ At-Risk Student Identification
Identifies students who may need additional academic support based on academic performance indicators.

## 🗂️ Project Structure

```text
Student-Performance-Analysis-Hadoop/
│
├── dataset/
│   └── student_dataset.csv
│
├── mapper/
│   ├── mapper_department.py
│   ├── mapper_semester.py
│   ├── mapper_grade.py
│   ├── mapper_attendance.py
│   └── mapper_atrisk.py
│
├── reducer/
│   ├── reducer_department.py
│   ├── reducer_semester.py
│   ├── reducer_grade.py
│   ├── reducer_attendance.py
│   └── reducer_atrisk.py
│
├── reports/
│   └── CSV reports
│
├── dashboard/
│   └── Excel dashboard
│
├── screenshots/
│
└── README.md
```

*Note: The structure above is the intended organization. Update filenames to match the actual uploaded files.*

## 🚀 How to Run the Project

### Step 1: Start Hadoop Services

```bash
start-dfs.sh
```

### Step 2: Verify Hadoop Services

```bash
jps
```

### Step 3: Check HDFS Project Directory

```bash
hdfs dfs -ls /student_performance
```

### Step 4: View Analysis Results

**Department-wise performance**
```bash
hdfs dfs -cat /student_performance/mapreduce_department_output_v2/part-*
```

**Semester-wise performance**
```bash
hdfs dfs -cat /student_performance/mapreduce_semester_output/part-*
```

**Grade distribution**
```bash
hdfs dfs -cat /student_performance/mapreduce_grade_output/part-*
```

**Attendance analysis**
```bash
hdfs dfs -cat /student_performance/mapreduce_attendance_output/part-*
```

**At-risk student identification**
```bash
hdfs dfs -cat /student_performance/mapreduce_atrisk_output/part-*
```

## 📈 Project Results

The project performs five major analytical operations on 10,000 student records.

- Department-wise performance analysis.
- Semester-wise academic comparison.
- Grade distribution analysis.
- Attendance pattern analysis.
- Identification of potentially at-risk students.

The processed results are stored in HDFS and used to generate CSV reports and an Excel dashboard.

## 🔮 Future Enhancements

- Build an interactive web-based dashboard.
- Integrate Machine Learning for academic performance prediction.
- Implement real-time student performance monitoring.
- Develop an early-warning system for students requiring academic support.

## 👩‍💻 Author

**B.Tech – Computer Science and Engineering (Data Science)**

---

<p align="center">
  ⭐ If you find this project interesting, consider giving this repository a star!
</p>
