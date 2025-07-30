# 🐍 Aadarsh's Python Practice Repo

![Project Pipeline](https://repository-images.githubusercontent.com/146619556/010dd080-4d26-11ea-8350-5916fe9db853))

Hi! I'm Aadarsh, and this is my personal Python learning journey.  
Here I share simple, real-world Python programs that I'm writing and practicing daily as part of my Data Science preparation.  
From basic syntax to real-world logic — all code here is beginner-friendly and cleanly written.

---

## 📌 What You’ll Find Here

✅ Python basics (variables, loops, functions, classes)  
✅ Real-life examples (grading system, billing logic, etc.)  
✅ Practice scripts (with explanations)  
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




## 📚 Object-Oriented Programming Example – Book Class

```python
class Book:
    def __init__(self, title, author, pages):
        self.title = title
        self.author = author
        self.pages = pages

    def boss(self):
        print(f"The title of the book is {self.title}")
        print(f"The author of the book is {self.author}")
        print(f"The number of pages is {self.pages}")


## 🚗 Encapsulation Example – Car Class

This example demonstrates **encapsulation** in Python using private variables (`__speed`) and controlled access through methods.

```python
class Car:
    def __init__(self):
        self.__speed = 0

    def accelerate(self, amount):
        if amount > 0:
            self.__speed += amount
            print(f"Accelerated by {amount}. Current speed: {self.__speed} km/h")
        else:
            print("Speed increase must be positive!")

    def brake(self, amount):
        if amount > 0:
            self.__speed = max(0, self.__speed - amount)
            print(f"Braked by {amount}. Current speed: {self.__speed} km/h")
        else:
            print("Brake amount must be positive!")

    def get_speed(self):
        return self.__speed

