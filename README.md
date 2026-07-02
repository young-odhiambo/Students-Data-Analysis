# Student Data Analysis

An interactive Power BI report that analyzes student enrollment, academic performance, attendance, teacher allocation, and school financial data across 12 schools.
The project demonstrates the complete Business Intelligence workflow, from data transformation and dimensional modelling to interactive dashboard development.

---

# Objective

The dashboard was developed to answer the following questions:

- How many students are enrolled across all schools?
- What is the overall academic performance?
- Which schools have the highest enrollment?
- How are students distributed across counties and regions?
- How are teachers distributed?
- Which subjects perform best?
- Which schools have the highest fee balances?
- Is teacher allocation balanced across schools?

---

# Dashboard Overview
![image alt](https://github.com/young-odhiambo/Students-Data-Analysis/blob/0923201452dd4943e3675af400e20eb9c727f64e/Screenshot%202026-07-01%20165111.png)


---



# Key Insights

## Student Enrollment

The data records **321 students** distributed across **12 schools**, giving an average enrollment of approximately **27 students per school**.

Regional analysis indicates that:

- **Nairobi** has the highest student population.
- **Central**, **Coast**, and **Rift Valley** have moderate enrollment levels.
- **Eastern** has the lowest number of students.

This suggests that student enrollment is concentrated in urban regions, particularly Nairobi.

---

## Academic Performance

The overall **average student score is 59.06**, while the overall **pass rate stands at 49%**.

This indicates that:

- Slightly fewer than half of the students are meeting the required pass mark.
- Academic interventions may be necessary to improve student outcomes.

---

## Attendance

Students recorded an average attendance rate of **78%**

Although attendance is relatively high, there remains a **22% attendance gap**, which may contribute to the relatively low pass rate.

Improving attendance could positively impact academic performance.

---

## Subject Performance

The highest-performing subjects include:

- Kiswahili
- Computer Studies
- Business Studies
- Biology

These subjects consistently achieve average scores above approximately **55 marks**, indicating stronger student performance compared to other subjects.

---

## Teacher Distribution

Teacher allocation varies by county.

From the analysis:

- **Kiambu** has the highest teacher count.
- Kisumu, Nairobi, and Mombasa follow closely.

Although the number of teachers differs slightly across counties, staffing appears relatively balanced.

---

## Student–Teacher Ratio

The Student to Teacher Ratio analysis shows that most schools maintain a ratio between **25 and 28 students per teacher**.

The relatively uniform ratios indicate that teachers are distributed fairly evenly across schools, helping maintain balanced classroom sizes.

---

## Gender Distribution

The analysis compares male and female enrollment across all schools.

Key observations include:

- Gender distribution is generally balanced.
- Some schools have slightly higher female enrollment.
- Others have slightly higher male enrollment.

No significant gender disparity is observed across the schools.

---

## Fee Balance Analysis

Outstanding fee balances total approximately **KSh 1.60 million**.

Schools with the highest fee balances include:

- Lurambi Green
- Naivasha Bright
- Mvita Coast
- Eldoret Valley

These schools account for the largest proportion of unpaid fees and may require targeted fee collection strategies.

---

# Data Modelling

The original dataset was normalized into a **Star Schema** to improve model efficiency and simplify reporting.

---

## Schema
![Image alt](https://github.com/young-odhiambo/Students-Data-Analysis/blob/68afc6b96d404f0710a11c7f12fd5a8afc10857d/Screenshot%202026-07-02%20142156.png)

---

### Fact Table

**Fact Records**

Contains transactional student records and numerical measures used for reporting.

---

### Dimension Tables

***Dim Student***

Stores demographic information about students.

***Dim School***

Stores school names and location information.

***Dim Teacher***

Contains teacher details linked to schools.

***Dim Subject***

Stores academic subject information.

---

# Relationships

Each dimension table connects to the Fact table using a **One-to-Many (1:*)** relationship.

| Dimension | Fact Table| Cardinality |
|------------|-------------|-----------|
|Dim Students | Facts Table| 1 : *|
| Dim School | Facts Tables | 1 : * |
| Dim Teacher | Facts Tables | 1 : * |
| Dim Subject | Facts Table | 1 : * |

---


# Key Findings

- 321 students were analyzed across 12 schools.
- The average score is **59.06**.
- Only **49%** of students passed while **51%** failed.
- Students maintain an average attendance of **78%**.
- Nairobi has the highest student enrollment.
- Kiswahili is the highest-performing subject.
- Mathematics and English require academic intervention.
- Teachers are relatively evenly distributed across schools.
- The student-to-teacher ratio is **1:54**.
- Schools have outstanding fee balances totaling **KSh 1.60 million**.

---

# Recommendations

- Improve Mathematics and English performance through targeted remedial programs.
- Increase attendance beyond **78%** by implementing attendance monitoring initiatives.
- Recruit additional teachers to reduce the current **1:54 student-to-teacher ratio**.
- Prioritize fee collection in schools with the highest outstanding balances.
- Replicate teaching practices from high-performing schools across lower-performing institutions.
- Continue monitoring gender balance to maintain equitable student representation.

---
