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

📌 Real-Life Example: Cleaning and Merging Data
Imagine one CSV has customer info, another has purchase history.
We:

1  Load both using pd.read_csv()

2  Remove nulls using dropna()

3  Merge using pd.merge() on CustomerID

4  Group by Product and summarize sales.
```python
df.isnull()         # Shows True/False for each cell

df.isnull().sum()   # Total missing in each column

df.dropna()               # Drops rows with ANY missing value

df.dropna(axis=1)         # Drops columns with ANY missing value

df.dropna(thresh=2)       # Drops rows with less than 2 non-null values

df.fillna(0)                        # Fill all NaNs with 0

df['Age'].fillna(df['Age'].mean()) # Fill Age column NaNs with mean

df.fillna(method='ffill')          # Forward fill (copy previous)

df.fillna(method='bfill')          # Backward fill (copy next)

df.groupby('Dept').mean()          #This gives average salary per Dept

df.groupby('Dept')['Salary'].agg(['mean', 'max', 'min'])

emp = pd.DataFrame({                             # Like SQL joins — used to combine two tables.
    'EmpID': [1, 2, 3],
    'Name': ['Aadarsh', 'Raj', 'Priya']
})

sal = pd.DataFrame({
    'EmpID': [1, 2, 4],
    'Salary': [50000, 60000, 45000]
})

pd.merge(emp, sal, on='EmpID')      #Merge (like INNER JOIN)
pd.merge(emp, sal, on='EmpID', how='left')   # Left Join
pd.merge(emp, sal, on='EmpID', how='right')  # Right Join
pd.merge(emp, sal, on='EmpID', how='outer')  # Full Outer Join

df.pivot_table(index='Department', values='Salary', aggfunc='mean')    #This gives average salary per department

df.pivot_table(index='Department', columns='Gender', values='Salary', aggfunc='mean', fill_value=0)

df['Age'].apply(lambda x: x ** 2)    #df['Age'].apply(lambda x: x ** 2)

df.apply(lambda row: row['Salary'] - row['Tax'], axis=1)   #axis=1 means row-wise









## 🧑‍💻 Sample Code 

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

