## 📊 Overview
Built an end-to-end HR Analytics dashboard in Power BI to monitor key employee KPIs, track productivity and attendance trends, and identify top performers. This solution helps HR and management take data-driven decisions for appraisals and resource planning.

## ✨ Features
- Total Employees, Average Performance Score
- Department-wise Performance Comparison
- Monthly Performance Trend
- Top 5 Performers
- Attendance & Productivity Analysis
- Filters by Department, Role, and Month

## 🛠️ Tools Used
- Power BI Desktop
- Excel / CSV for data cleaning
- DAX for measures

## 📸 Dashboard Preview
(Add your dashboard screenshot here - Drag & drop image)

## 🔍 Key Insights
- Identified low-performing departments
- Tracked monthly performance improvement
- Helped in decision making for appraisals

## 🚀 How to RUN
1. Download the .pbix file
2. Open in Power BI Desktop
3. Refresh data if needed

## 👩‍💻 Author
Bhargavi Yadhav | Aspiring Data Analyst | power BI


### 💻 DAX Code - Main Logic

**KPI Measures:**
```DAX
Total Employees = COUNTROWS(Employee_Data)
Total Departments = DISTINCTCOUNT(Employee_Data[Department])
Average Performance = AVERAGE(Employee_Data[Performance_Score])
Avg Attendance = AVERAGE(Employee_Data[Attendance_%])
Top Score = MAX(Employee_Data[Performance_Score])Grading Logic:DAXPerformance Grade =
SWITCH(
 TRUE(),
 Employee_Data[Performance_Score] >= 90, "A",
 Employee_Data[Performance_Score] >= 75, "B",
 Employee_Data[Performance_Score] >= 60, "C",
 "D"
)
Aspiring Data Analyst | Power BI | Excel | SQL
