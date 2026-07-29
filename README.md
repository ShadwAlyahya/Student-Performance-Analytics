# Student Performance Analytics

## AI-Assisted Data Cleaning | Power BI Dashboard

![Dashboard Preview](images/student-performance-dashboard.png)

## Project Overview

Student Performance Analytics is a mini data analytics project that explores academic performance and examines how factors such as study hours, attendance, sleep, participation, and extracurricular activities relate to student outcomes.

The project follows an end-to-end analytical workflow, starting with data quality assessment and cleaning, followed by data analysis and interactive dashboard development.

AI was used exclusively to support the data quality review and data-cleaning process within Excel. The data modeling, analytical measures, visual design, dashboard development, and interpretation of results were completed independently using Power BI.

---

## Objectives

The project aims to:

- Assess the overall academic performance of students.
- Compare average scores across different subjects.
- Examine the relationship between weekly study hours and academic scores.
- Evaluate the association between attendance and student performance.
- Analyze the distribution of student performance levels.
- Identify students who may require additional academic support.
- Present key findings through an interactive Power BI dashboard.

---

## Dataset

The dataset contains student academic and behavioral information across 12 fields:

| Column | Description |
|---|---|
| `Student_ID` | Unique student identifier |
| `Education_Level` | High School or University |
| `Grade_Level` | Student grade or university year |
| `Subject` | Academic subject |
| `Score` | Student academic score |
| `Study_Hours_Per_Week` | Weekly study hours |
| `Attendance_Percentage` | Student attendance rate |
| `Sleep_Hours_Per_Night` | Average sleep hours per night |
| `Participation_Level` | Low, Medium, or High participation |
| `Extracurricular_Activities` | Number of extracurricular activities |
| `Performance_Level` | High Performance, Average, or Needs Support |
| `Result` | Pass or Fail |

The original dataset contained **505 records**. After data cleaning, the final analytical dataset contained **500 records**.

---

## AI-Assisted Data Quality Review and Cleaning

GPT for Excel was used to review the original dataset, identify data-quality issues, and support the creation of a cleaned dataset.

The AI-assisted review identified the following issues:

| Data Quality Issue | Records Affected | Cleaning Action |
|---|---:|---|
| Full duplicate rows | 5 | Removed duplicate records |
| Missing attendance values | 10 | Filled using the column median |
| Missing sleep-hour values | 12 | Filled using the column median |
| Missing participation values | 8 | Filled using the most frequent category |
| Inconsistent participation labels | 15 | Standardized to `High`, `Medium`, and `Low` |
| Negative study-hours value | 1 | Replaced using the median of valid values |
| Invalid attendance values | 2 | Corrected using a data-driven approach |

### Data Cleaning Results

- Original records: **505**
- Duplicate records removed: **5**
- Final cleaned records: **500**
- Missing values addressed: **30**
- Inconsistent category values standardized: **15**
- Invalid numeric values corrected: **3**
- Performance level and result consistency: **0 mismatches**

The cleaned dataset was validated to ensure that `Performance_Level` and `Result` remained fully consistent with the corresponding `Score` values.

> **Note:** AI was used only to assist with data-quality assessment and data cleaning. The Power BI dashboard, analytical measures, visualizations, and interpretation were developed independently.

---

## Power BI Dashboard

The interactive dashboard was developed in Power BI and includes:

### Key Performance Indicators

- **Total Students:** 500
- **Average Score:** 81.63
- **High Performance Rate:** 57.80%
- **Needs Support Rate:** 5.20%

### Visual Analysis

- Average Score by Subject
- Study Hours vs. Academic Score
- Performance Level Distribution
- Average Score by Attendance Rate

### Interactive Filters

- Education Level
- Grade Level
- Subject

---

## Key Insights

### 1. Overall Academic Performance

The dataset shows strong overall academic performance, with an average score of **81.63**.

### 2. High-Performing Students

**57.80%** of students were classified as **High Performance**, indicating that more than half of the students achieved strong academic outcomes.

### 3. Students Requiring Support

Only **5.20%** of students were classified as **Needs Support**, highlighting a relatively small group that may benefit from targeted academic intervention.

### 4. Attendance and Academic Performance

Students with higher attendance rates generally achieved higher average scores, indicating a positive relationship between attendance and academic outcomes.

### 5. Study Hours and Academic Performance

The analysis shows a positive relationship between weekly study hours and academic scores. Students who studied more frequently tended to achieve stronger academic results.

### 6. Subject Performance

Computer Science recorded the highest average score, while History recorded the lowest average score among the analyzed subjects.
