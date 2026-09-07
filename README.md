## 💻 DAX Code - Main Logic

**KPI Measures:**
Total Employees = COUNTROWS(Employee_Data)
Total Departments = DISTINCTCOUNT(Employee_Data[Department])
Average Performance = AVERAGE(Employee_Data[Performance_Score])
Avg Attendance = AVERAGE(Employee_Data[Attendance_%])

**Top Performer:**
Top Score = MAX(Employee_Data[Performance_Score])

**Grading Logic:**
performance Grade =
SWITCH(
 TRUE(),
 Employee_Data[Performance_Score] >= 90, "A",
 Employee_Data[Performance_Score] >= 75, "B",
 Employee_Data[Performance_Score] >= 60, "C",
 "D"
)
