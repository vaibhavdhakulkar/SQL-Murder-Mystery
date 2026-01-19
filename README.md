🕵️ SQL Murder Mystery – Complete Investigation Using SQL
📌 Project Overview

This repository contains a complete, step-by-step solution to the SQL Murder Mystery challenge.
The goal of this project is to solve a fictional murder case using only SQL, by exploring relational data, analyzing witness interviews, and narrowing down suspects through logical filtering.
This project demonstrates real-world SQL problem-solving skills, including data exploration, debugging empty result sets, and combining information across multiple tables.

🧠 Problem Statement
A murder took place on January 15, 2018, in SQL City.
Using the available database, the objectives are:
Identify the murderer
Identify the mastermind who hired the murderer
All conclusions are derived purely from SQL queries.

🔗 Dataset & Environment
This project uses the official SQL Murder Mystery database, which is available by default at:
👉 https://mystery.knightlab.com/

The platform provides:
A preloaded relational database
An in-browser SQL editor
All required tables available by default
No database setup or data import is required.

🗂️ Database Tables Used
The investigation uses multiple related tables, including:
crime_scene_report
person
interview
drivers_license
get_fit_now_member
get_fit_now_check_in
facebook_event_checkin
income
These tables are connected using primary and foreign keys, requiring extensive use of JOINs.

🔍 Investigation Approach
Instead of attempting to solve the case with a single complex query, the investigation follows a structured, step-by-step analytical approach.

1️⃣ Crime Analysis
Queried the crime_scene_report table to identify the crime details.
Extracted information about the location, date, and witnesses.

2️⃣ Witness Identification & Interviews
Identified two witnesses based on address clues.
Retrieved interview transcripts to extract critical clues related to:
Gym membership
Membership type
Vehicle plate number pattern
Physical descriptions

3️⃣ Suspect Filtering
Used gym membership data (Get Fit Now Gym) to narrow suspects.
Applied membership type (Gold) and membership ID pattern (48Z).
Cross-checked suspects using vehicle plate information.
✅ This led to identifying the murderer: Jeremy Bowers.

🧩 Mastermind Identification
The murderer’s interview provided additional clues about the person who hired him:
Height between 65–67 inches
Drives a Tesla Model S
Attended the SQL Symphony Concert
Has a very high income
By joining driver information, event check-ins, and income data, and ordering by annual income, the mastermind was identified.

✅ Final Result:
Miranda Priestly

🛠️ SQL Concepts Demonstrated

This project demonstrates practical usage of:
INNER JOIN
Subqueries
Filtering using WHERE
Pattern matching using LIKE
Sorting and limiting results
Progressive query debugging
Data validation using DISTINCT

▶ How to Run the Project
Visit https://mystery.knightlab.com/
Open the built-in SQL editor
Copy queries from sql_murder_mystery_solution.sql
Execute queries step by step by following the comments

🏁 Final Answer :
🔍 Murderer: Jeremy Bowers
🧠 Mastermind: Miranda Priestly
