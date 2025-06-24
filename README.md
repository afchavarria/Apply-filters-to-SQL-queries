# Apply filters to SQL queries
## Project description
My team was charged with obtaining specific data from employees to analyze any potential security issues and to update computers. This task was done by filtering the required information from the database. First, we filtered to find all failed login attempts after business hours, login attempts on specific dates, and logins that didn't originate in Mexico. We retrieve information about certain employees in the Marketing department, information about employees in the Finance or the Sales department and information about employees who are not in the Information Technology department. By doing this, we were able to ensure the system is safe, investigate all potential security issues, and update employee computers as needed.

## Retrieve after hours failed login attempts
 My team was tasked with investigating faild login attempts that were made after business hours. To retrieve this information from the login activty, I used the following commands.
  <img width="855" alt="Image" src="https://github.com/user-attachments/assets/92362340-80a5-4f31-a78d-0173530af578" />
In my input, I filtered the login attempts that failed after business hours (18:00). There are two conditions after the WHERE clause where the login times are filtered after 18:00 and the success = FALSE to filter the failed attempts.
  
## Retrieve login attempts on specific dates
A suspicious event occurred on 2022-05-09. Any login activity that happened on 2022-05-09
or on the day before needs to be investigated. The following code demonstrates how I created a SQL query to filter for login attempts that occurred on specific dates.
<img width="1011" alt="Image" src="https://github.com/user-attachments/assets/65635897-acd5-42af-bdf1-a5d70050c333" />
The first part of the screenshot is my query, and the second part is a portion of the output. This inquery returns all login attempts that occurred on 2022-05-09 or 2022-05-08. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an OR operator to filter my results to output only login attempts that occurred on either 2022-05-09 or 2022-05-08. The first condition is login_date = '2022-05-09', which filters for logins on 2022-05-09. The second condition is login_date = '2022-05-08', which filters for
logins on 2022-05-08.

## Retrieve login attempts outside of Mexico
<img width="1008" alt="Image" src="https://github.com/user-attachments/assets/2d0a3c74-a9e7-4804-911e-f66f57d5c9ae" />

## Retrieve employees in Marketing
<img width="1008" alt="Image" src="https://github.com/user-attachments/assets/8b0a4be4-3062-4c45-803c-1e4d9a979f19" />

## Retrieve employees in Finance or Sales
<img width="1012" alt="Image" src="https://github.com/user-attachments/assets/60dd723b-9942-4d20-b0ec-b288fb091f09" />

## Retrieve all employees not in IT
<img width="1012" alt="Image" src="https://github.com/user-attachments/assets/2ca2754d-985a-4590-adfb-d6e20811f510" />

## Summary
In all, I was able to obtain specific information about employees, their machines, and the departments they belong to from the database to investigate potential security issues and to update computers. By filtering with AND, OR, and, NOT, I was able to obtain the required information from the database.
