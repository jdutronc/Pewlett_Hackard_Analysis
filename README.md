# Pewlett_Hackard_Analysis

## Project Overview
Pewlett-Hackard is a large company of thousands of employees that has been around for a long time. Many babyboomer employees are due to retire in the next few years and we have been tasked with analyzing employee data to prepare for the future: employees eligible for retirement packages, hiring needs per department and position, mentorship programs etc. Specifically in this challenge, we are to determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program.

## Software & Resources
pgAdmin 4

## Results of the Analysis
1. Out of a total workforce of 300,024 at Pewlett-Hackard some 72,458 employees will retire in the next few years (24.2%)
2. About half of the employees retiring are engineers of all levels, as we can see in the 'Retiring Titles' table below, and about a third are senior staff from all departments:
<img align='center' src='Retiring_Titles.png' height='200'>
<br>

3. The three departments that will be most impacted by the 'silver tsunami' are Development (25.3% of positions due to retire), Production (22.3%) and Sales (16.0%), as we can see in the 'Retirement by Dept' table below:
<img align='center' src='Retirement_by_Department.png' height='200'>
<br>

4. Only 1,549 employees are eligible to enroll in the mentorship program.

## Summary

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?
Some 72,458 employees will retire in the next few years (24.2% of the PH workforce). Pewlett-Hackard need to plan quickly to replace a huge portion of their workforce, and for that purpose we can exploit the data csv files and format into graphs in pandas using matplotlib.

### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
Assuming all 72,458 positions will be replaced, the mentorship program would only provide a whopping 46 trainees per mentor, which is clearly insufficient so the criteria of the mentorship program have to be revised to include other senior employees born after 1965. We can easily revise the SQL query in pgAdmin to include progressively senior employees born in 1966-1970 until we reach a ratio of 2-4 trainees per mentor.
