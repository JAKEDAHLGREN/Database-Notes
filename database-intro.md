# Database Intro 4/12/2023

class Student
  def initialize(name, cohort)
    @name = name
    @cohort = cohort
  end
end

Student.new('Felix', 'Bravo') # new instance of class Student
Student.new('James', 'Bravo') # new instance of class Student
Student.new('Chris', 'Hotel') # new instance of class Student

# Databases
- Model - the class(defines the structure, the types of data that can be stored)
- Primary key - unique identifier for each object
- rows and columns (think excel spreadsheet)
  - each row is an object(instance of a class)
- Primary key - unique identifier for each object/row

# PostgresSQL

- talk to databases
- open-source
- Object-Relational Database Managment System (ORDMS)
- OOP - Object oriented programing approach

terminal command: psgl , then \l

# pgAdmin 4 

- Single '' only, it will not recognize ""
- Keyword - convention is ALL UPPERCASE, new line for each keyword
   # important keywords: SELECT, FROM
   - * - splat operator = get all 
   - LIMIT - returns the number you pass to it (EX. LIMIT 10)
   - WHERE - conditional statement (ex. WHERE continent = 'North America') or (ex. WHERE continent != 'North America': not equal to North America)
   - WHERE ... IS NOT ... - (Ex. WHERE indepyear IS NOT null, or WHERE indepyear NOTNULL)
   - AND - Both statements must be true
   - OR - Only one statement must be true
   - LIKE - has 'specified pattern' in the return
     - % - Wildcard used infront of a the search term (Ex. Like '%America')
   - ORDER BY - DESC (descending)
     - for numbers you can use 1e6, meaning 1 followed by 6 zeros (ex.WHERE population < 1e6)
   - For more commands search "SQL Commands"
 - data is returned in the order that it is entered into the table, unless otherwise stated


