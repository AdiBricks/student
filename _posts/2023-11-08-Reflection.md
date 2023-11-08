---
toc: true
comments: true
title: Reflection
layout: post
description: My reflection for the Trimester
courses: { csp: {week: 12}}
type: tangibles
---

Over the last trimester, I have learned quite a bit. I have gone from having knowledge of Python 5 years ago to being more comfortable with the language, creating popups, working on background design with HTML, fetching APIs to get information, knowing how to use iterations and algorithms, and creating/using my own procedures. This has not only grown the amount of things I've learned but at the same time helped make my coding more efficient. 

As for growth, I plan to work on the student teaching lessons (Procedures, Iteration, Libraries, etc) to maximize my understanding of them as I need more than going over them once. 
Learn to communicate with my team better in order to be more efficient and get better results out of our work. 
Start committing more often, and document the changes I make in my work regularly (through issues, team tickets, and plans)	

| Assignment          | Pseudocode                  | Python              |
| ------------------- | ----------------------------| ------------------- |
| a ← expression      | a ← expression              | a = expression      |
| Equal Operator      | a = b                       | a == b              |
| Not Equal Operator  | a ≠ b                       | a != b              |
| Iteration           | REPEAT n TIMES              | for i in range(n):  |
| Conditional Iteration| REPEAT UNTIL (condition)   | while condition:      |
| List indexing       | list[1] is first item       | list[0] is first item |
| Lists               | pslist ← [C,S,P]            | pylist = ["S", "S", "P"] |
| Printing            | DISPLAY(CSP IS FUN!)        | print(“CSP IS FUN!”) |
| Assigning lists     | psList ← pyList             | psList == pyList     |
| List Iteration      | FOR EACH item IN pslist { } | for i in list:        |
| Printing            | DISPLAY(CSP IS FUN!)        | print(“CSP IS FUN!”) |
| Modulo              | a MOD b                     | a % b                |
| Procedure           | PROCEDURE psProcedure(parame| def pyProcedure(arg1, arg2, ...)
                        ter1, parameter2, ...) { <br>| : <br> Put procedure here |
                         Put procedure here }       |   

PSEUDO CODE vs PYTHON EXAMPLES
Psuedo area calculator: 
PROCEDURE psProcedure calculateRectangleArea(length, width):
    area = length * width
    RETURN area
Python area calculator:
def pyProcedure (length, width):
    area = length * width
    return area

NUMBER SUMMATION:
Psuedo Code:
Display(Enter a number to sum up till: )
  Input n
  sum = 0
  For i from 1 to n
    sum = sum + i
  End For
  Display sum
Stop

Python Code:
N = int(input("Enter a number to sum up till: "))
sum = 0

for i in range(1, N + 1):
    sum = sum + i

print(sum)