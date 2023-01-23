# pandas-challenge

Georgia Tech Data Analytics BootCamp - January 2023

Homework Module 04 - Pandas Challenge
By Priscila Menezes Briggs

This challenge is based on the data analysis for a city's school district. In this capacity, our task as a Chief Data Scientist is to help the school board and mayor make strategic decisions regarding future school budgets and priorities. The main methodology to analyze the data will be to aggregate the data to showcase obvious trends in school performance. An analysis of the district-wide standardized test results in math and reading will be made, as well as analysis for additional information about the schools, such as school size and type.  

In this challenge, a script on Jupyter Notebook using Pandas has been developed to calculate the desired values and analyze the schools trends. 
Two datasets called schools_complete.csv and students_complete.csv had been provided as resources, which were composed of the following columns:

schools_complete.csv: School ID, School Name, School Type, SChool Size, School Budget.
students_complete.csv: Student ID, Student Name, Gender, Grade, School Name, Reading Score, Math Score.

Data for each block below has been calculated and a correspondent DataFrame has been created to gather the results. The topics under analysis were:

- District Summary: calculus of totals for schools and students' information with the district as the base.
- School Summary: data calculated per school and per student.
- Highest-Performing Schools (by % Overall Passing): identification and calculation of data for the best schools in the district according to their results in overall passing.
- Lowest-Performing Schools (by % Overall Passing): similar as with the highest-performing schools, but this time analyzing the characteristics of schools that had the poorest results in overal passing.
- Math Scores by Grade: list of all students's scores in Math, classified by grade.
- Reading Scores by Grade: list of all students's scores in Reading, classified by grade.
- Scores by School Spending: analysis of the impact of the school budget on the students' scores and pass rates.
- Scores by School Size: analysis of the impact of the school size on the students' scores and pass rates.
- Scores by School Type: analysis of the impact of the school type (charter or district) on the students' scores and pass rates.

Some of the conclusions from this analysis are described below and are also written in the notebook:

Topic: Scores by School Size
* As a whole, the math passing rate in schools with less than 2,000 high school students (small and medium-sized schools) was, on average, 34% better than in schools with more than 2,000 students (large schools). The same happened with the passing rate in reading, where large schools performed, on average, 14% worse than small and medium-sized schools.
* While smaller schools (< 1,000 students) scored higher in reading and math, pass rates in both subjects and the overall pass rate were higher in medium-sized schools (1,000 to 2,000 students), for which the average spending per student was only 1.8% higher than the average amount spent per student by smaller schools.

Topic: Scores by School Spending
* The average budget per student is 620.0. Schools with a per-student budget below this value had, on average, a 46% higher overall passing rate than schools with a per-student budget above 620.0.
* As a whole, all grades and pass rates were the highest when spending per student was the lowest (<$585). On the opposite side, all grades and pass rates were the lowest when spending per student was the highest ($645-680). The overall pass rate was 69% greater among schools with the lowest per-student spending compared to the highest spending schools.

Topic: Highest-Performing Schools (by % Overall Passing)
* The 5 highest-performing schools had the following characteristics: 4 out of 5 were small and medium-sized schools; 3 out of 5 had a lower than average spending per student; overall passing rates in math and reading at these schools were over 90% on average.

Topic: Lowest-Performing Schools (by % Overall Passing)
* The 5 lowest-performing schools had the following characteristics: all 5 were large sized schools and had above-average spending per student; the reading pass rate was still very good, over 80% on average, but math had a much lower pass rate: 66% on average, which resulted in an overall pass rate of just 53% on average.

Topics: Math and Reading Scores by Grade
* As a whole, the average score in mathematics was 80.4 and in reading was 82.5, considering all schools and grades. The 11th grade students had the best performances in mathematics and reading on average, but the difference in comparison to the other grades was not significant in both cases.

Topic: Scores by School Type
* As a whole, district schools had an average pass rate of 53.7%, while charter schools had 90.4% for this same measurement. Formed mostly by small and medium-sized schools, charter schools spent on average about 7% less per student than district schools, which were made up only of large schools.


The file main.ipynb inside the PyCitySchools folder contains the script for this challenge. A starter code previously provided was used as reference for the calculations. 

The references to build this script were the activities and lessons given in class and in tutoring session in addition to the websites below. 

References:

All webpages visited in January/2023.

Setting index name to Data Frames
#https://sparkbyexamples.com/pandas/pandas-set-index-name-to-dataframe/#:~:text=Use%20pandas.,the%20index%20name%20as%20well.

Data Frames - drop duplicates
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.drop_duplicates.html

Understanding inplace:true in Pandas
https://stackoverflow.com/questions/43893457/understanding-inplace-true-in-pandas

Setting up headings and changing cell type in Jupyter notebook
https://www.tutorialspoint.com/jupyter/jupyter_notebook_markdown_cells.htm

Basic syntax for markdown cell writing
https://www.markdownguide.org/basic-syntax/

The script and written analysis for this homework are found in the GitHub's repository on:
https://github.com/PrisBriggs/pandas-challenge