# Pewlett-Hackard-Analysis
PostgreSQL pgAdmin QuickDBD Schemas 

## Overview of the analysis: 
  Determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Deliver a written report that summarizes your analysis and helps prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.

## Results: Provide a bulleted list with four major points from the two analysis deliverables. Use images as support where needed.
  Using an ERD created in this module, and six csvs filled with data not quite combined in a usable form.  Using pgAdmin4 and PostgreSQL, I tablulate the data in the requested forms to get the information the company needs to determine amount of people up for retirement, which departments they are in, and how to get a Mentorship Program started to increase the amount of employees ready for senior roles.
  
![EmployeeDB](https://user-images.githubusercontent.com/102183530/169713935-fafd77f3-b2c0-4dc8-95aa-e6f9f049405e.png)

###### Figure 1. ERD map shows the flow of information from one table to another.

Using this as a map (Fig 1), above I was able to pair select tables and columns together for the desired information.

The first grouping sought was the titles of the retiring employees in a table.

![retirement titles code1](https://user-images.githubusercontent.com/102183530/169714505-c4001462-a6eb-4e7d-be3a-deccc063c955.png)

Following this grouping, I needed to delete duplicate employee numbers, as some of them have been employed at Pewlet Hackard long enough to have a couple different promotion dates.  I was only concerned about pulling the most up-to-date titles.

![Code 3 employee by title retiring](https://user-images.githubusercontent.com/102183530/169714516-65c30443-e9dd-48a4-8da9-4c01d510e66b.png)

Then ordered the number of retiring by department number.  This is helpful as a group to see the large numbers of people able to retire or looking to in the next couple years.

![Retiring Employees by department](https://user-images.githubusercontent.com/102183530/169713949-cf6b82f4-07d7-4654-b983-47afcc23fe29.png)

![Senior:Leader titles](https://user-images.githubusercontent.com/102183530/169715798-3a87ac90-0cbe-42cc-82d5-b7da9d19a362.png)

The next deliverable is to see about what starting a Mentorship program using the code above to see what the number of employees look like.

## Summary: Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."

![Retire by titles](https://user-images.githubusercontent.com/102183530/169714637-4b336827-fbf2-436c-9136-f77ebabd9f3b.png)

- How many roles will need to be filled as the "silver tsunami" begins to make an impact?
  - The total number of employees retiring  is 53,977
  - 19190 Senior Engineer
  - 18619 Senior Staff
  - 6916 Engineer
  - 5741 Staff
  - 2708 Technique Leader
  - 802 Assistant Engineer
  - 1 Manager
     
- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
- 
![Senior Leader titles](https://user-images.githubusercontent.com/102183530/169715888-7ea92f50-6837-4354-8090-6c9bf07b3594.png)

