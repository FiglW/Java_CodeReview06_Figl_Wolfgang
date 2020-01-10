create a SQL statement that reports all the student a specific class when you know a specific class ID (aka something like “show all students of the class 1b, which has the ID=2”)

--> 
SELECT class.name,student.name,student.surname FROM student INNER JOIN class ON student.classID_FK = class.classID WHERE class.classID = 2








create a SQL statement that reports all the student a specific class when you know a specific class name (aka something like “show all students of the class ‘1b’; I do not know the class ID”)

-->

SELECT class.name,student.name,student.surname FROM student INNER JOIN class ON student.classID_FK = class.name WHERE class.name = "2A"