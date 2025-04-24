# MY-SQL-QUERY-FOR-NYSC-DEPLOYMENT
This is to summarize post based on a university's graduated student record

NYSC DATA ANALYSIS FROM DAYO
Highest nos of student from university
SELECT university_attended,COUNT(university_attended)AS UniNos FROM `nysc_data` GROUP by university_attended ORDER by university_attended desc limit 1
COMPARISON
COMPARISON  entails : We have greater than, less than, greater than =, Less than =, Not equal to
On numbers
!=           <>  represent Not equal to
SELECT fullname,year_of_graduation FROM `nysc_data` WHERE year_of_graduation <> 2020
SELECT fullname,year_of_graduation FROM `nysc_data` WHERE year_of_graduation != 2020
COMPARISON
On string 
SELECT fullname,university_attended FROM `nysc_data` WHERE university_attended !='Imo State University'
LOGICAL
And, or, Not

OR
SELECT * FROM `NYSC_Data` WHERE state_of_origin = 'ekiti' or state_of_origin ='ogun' or state_of_origin = 'lagos'
SHORTCUT FOR “OR”
SELECT * FROM `NYSC_Data` WHERE state_of_origin IN ('lagos','ekiti','ogun')
SHORTCUT FOR “NOT IN”
SELECT * FROM `NYSC_Data` WHERE state_of_origin NOT IN ('lagos','ekiti','ogun')
Not in
SELECT * FROM `NYSC_Data` WHERE university_attended NOT in ('Delta State University','Imo State University', 'Nnamdi Azikiwe University')

Wildcard Characters
Symbol 	Description
% 	Represents zero or more characters
_ 	Represents a single character
[] 	Represents any single character within the brackets *
^ 	Represents any character not in the brackets *
- 	Represents any single character within the specified range *
{} 	Represents any escaped character **
NOTE FROM TUTORIAL WITH DAYO
Dayo taught me that if I mistakenly type Delete on SQL, it will delete all data records.
Also, He mentioned to me that when you use “Update” I should always specify the column and row I want to update. If not properly stated. SQL will update all
Drop is for Database and Table
Alter is for Column and Row
WHERE is Where is used when you have a specific request on SQL
GROUPBY: When you are trying to find a result that you aren’t specific about, you use groupby 
Having - it to add more condition : Like condition from a condition . .Like there is already a condition, like groupby, order or another condition like where,… Like you already use a condition, but you want sql to perform another condition with having before giving the final result 

I now understand why a table name is attached to each if the column e.g appointment.Patientid
This is the reason why I was seeing this ambiguous error. 
I understand why my join formulae didn’t work. This was cos the data that I used it in before has a unique column name all through.


When SQl declares that a column is ambiguous. It means that the column name isn’t a distinct name, there are many column from another table with that same name
I get to know that I can a particular database or table jn new tab 
2ND day tutorial
You can drop Database and table while you can delete row and column
Varchar accomodate number, symbol and words. It is also known as strings
Data type generally talks about the data structure 

Koko SQL
Logical reasoning 
Conditional reasoning 
Comparison 

Type of Errors
Logical Error ; You code give result but the answer isn’t corrent
Syntax Error: code no run

And, or, not
And: Daddy and mummy from Iwo. These conditions have to be met for SQL to give result
Or : one of them is from iwo. Once one of the conditions is met. Then it gives result
Not: none of them is from iwo. Or not Ileogbo

Not in
SELECT * FROM `NYSC_Data` WHERE university_attended NOT in ('Delta State University','Imo State University', 'Nnamdi Azikiwe University')

NOTE
UPDATE IS TO EDIT
INSERT IS TO ADD NEW ROW

