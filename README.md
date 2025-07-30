# 🐍 Aadarsh's Python Practice Repo

![Banner](assets/banner.png)

Hi! I'm Aadarsh, and this is my personal Python learning journey.  
Here I share simple, real-world Python programs that I'm writing and practicing daily as part of my Data Science preparation.  
From basic syntax to real-world logic — all code here is beginner-friendly and cleanly written.

---

## 📌 What You’ll Find Here

✅ Python basics (variables, loops, functions, classes)  
✅ Real-life examples (grading system, billing logic, etc.)  
✅ Practice scripts (with explanation)  
✅ Python for Data Science (coming soon)  

---

## 🧑‍💻 Sample Code – Student Grading System

```python
class Student: 
    def __init__(self, name, marks):
        self.name = name
        self.marks = marks

    def grade(self):
        print(f"Marks of {self.name} is {self.marks}")
        if self.marks >= 40:
            print("Result: Passed ✅\n")
        else:
            print("Result: Failed ❌\n")

# Create students
student1 = Student("Aalok", 50)
student2 = Student("Aadarsh", 38)

student1.grade()
student2.grade()
