# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
```
N=int(input())
students=[]
for _ in range(N):
    name = input()
    score =float(input())
    students.append([name,score])
    
scores = sorted(set(score for _, score in students))
second_lowest_score=scores[1]

second_lowest_students= sorted([name for name,score in students if score == second_lowest_score])

for students in second_lowest_students:
    print(students)
```

## Output
<img width="394" height="403" alt="image" src="https://github.com/user-attachments/assets/d5c568a9-7359-4b7f-a443-cacc145f8ba9" />


## Result
Thus, the output is verified successfully.


