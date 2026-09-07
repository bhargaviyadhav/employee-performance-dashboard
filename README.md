DAX
Total Employees = COUNTROWS(Employee_Data)
Average Performance = AVERAGE(Employee_Data[Performance_Score])
Attendance % = DIVIDE(SUM(Employee_Data[Present_Days]), SUM(Employee_Data[Working_Days])) * 100
