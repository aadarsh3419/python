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
```├── All Permutations
├── Backward Each Word
├── Backward String
├── Check if a Number is Prime
├── Double numbers but only if odd, else square
├── Exception Handling
├── Filter strings starting with a vowel
├── Find Remainder
├── Find the factorial of a number (reduce)
├── Find the longest word in a sentence
├── First Word (simplified
├── Flatten a 2D list
├── Get unique elements from list (order preserved)
├── Integer Sign Determination
├── Is Even
├── Just Fizz!
├── Merge two lists into a dictionary (zip)
├── Multiply (Intro)
├── Probability & Statistics Examples in Python
├── Python + Pandas – Clean and Summarize Data
├── README.md
├── Rectangle Perimeter
├── Reverse each word in a sentence
├── Sample Walking Data
├── Sort dictionary by value in descending order
├── analysis by pd
├── bmi calculater
├── calculater
├── central tendancy
├── class book
├── delete,fill,see nan value , for nan value use
├── df.iloc use
├── difference =, ==
├── erroe handaling of  ZeroDivisionError
├── factoriyal
├── filw handaling with write
├── find outlier
├── for cleaning data
├── health data cleaning for py
├── lambda_use
├── largest element
├── list comp
├── list comparistions
├── map(),filter()
├── max min
├── more_lambda
├── num
├── oops
├── palindrome
├── pd 1
├── pd for data analysis
├── prime
├── prime nu
├── python-basics
    ├── README.md
    ├── array_operations.py
    └── numpy_basics.py
├── random password  generater
├── read write file
├── recursion
├── remove duplicate
├── reverse string
├── reverse string 1
├── roman number
├── student grade system
├── student grading system
├── tiny litele clean data
├── use of df.loc
├── using encapculation
└── vowels in string find


/All Permutations:
--------------------------------------------------------------------------------
 1 | from collections.abc import Iterable
 2 | from itertools import permutations
 3 | 
 4 | def string_permutations(s: str) -> Iterable[str]:
 5 |     # your code here
 6 |     
 7 |      return sorted([''.join(i) for i in permutations(s) ])
 8 | 
 9 | 
10 | print("Example:")
11 | print(list(string_permutations("ab")))
12 | 
13 | # These "asserts" are used for self-checking
14 | assert list(string_permutations("ab")) == ["ab", "ba"]
15 | assert list(string_permutations("abc")) == ["abc", "acb", "bac", "bca", "cab", "cba"]
16 | assert list(string_permutations("a")) == ["a"]
17 | assert list(string_permutations("abcd")) == [
18 |     "abcd",
19 |     "abdc",
20 |     "acbd",
21 |     "acdb",
22 |     "adbc",
23 |     "adcb",
24 |     "bacd",
25 |     "badc",
26 |     "bcad",
27 |     "bcda",
28 |     "bdac",
29 |     "bdca",
30 |     "cabd",
31 |     "cadb",
32 |     "cbad",
33 |     "cbda",
34 |     "cdab",
35 |     "cdba",
36 |     "dabc",
37 |     "dacb",
38 |     "dbac",
39 |     "dbca",
40 |     "dcab",
41 |     "dcba",
42 | ]
43 | 
44 | print("The mission is done! Click 'Check Solution' to earn rewards!")
45 | 


--------------------------------------------------------------------------------
/Backward Each Word:
--------------------------------------------------------------------------------
 1 | def backward_string_by_word(text: str) -> str:
 2 |     # your code here
 3 |     b = [''.join(i[::-1]) for i in text.split(' ')]
 4 | 
 5 |     return ' '.join(b)
 6 | 
 7 | 
 8 | print("Example:")
 9 | print(backward_string_by_word(""))
10 | 
11 | # These "asserts" are used for self-checking
12 | assert backward_string_by_word("") == ""
13 | assert backward_string_by_word("world") == "dlrow"
14 | assert backward_string_by_word("hello world") == "olleh dlrow"
15 | assert backward_string_by_word("hello   world") == "olleh   dlrow"
16 | assert backward_string_by_word("welcome to a game") == "emoclew ot a emag"
17 | 
18 | print("The mission is done! Click 'Check Solution' to earn rewards!")
19 | 


--------------------------------------------------------------------------------
/Backward String:
--------------------------------------------------------------------------------
 1 | def backward_string(val: str) -> str:
 2 |     # your code here
 3 |     
 4 |     return val[:: -1]
 5 | 
 6 | 
 7 | print("Example:")
 8 | print(backward_string("val"))
 9 | 
10 | # These "asserts" are used for self-checking
11 | assert backward_string("val") == "lav"
12 | assert backward_string("") == ""
13 | assert backward_string("ohho") == "ohho"
14 | assert backward_string("123456789") == "987654321"
15 | 
16 | print("The mission is done! Click 'Check Solution' to earn rewards!")
17 | 


--------------------------------------------------------------------------------
/Check if a Number is Prime:
--------------------------------------------------------------------------------
 1 | class Solution(object):
 2 |     def isPrime(self, num):
 3 |         if num <= 1:
 4 |             return False
 5 |         for i in range(2, int(num**0.5) + 1):
 6 |             if num % i == 0:
 7 |                 return False
 8 |         return True
 9 | 
10 | # Example
11 | sol = Solution()
12 | print(sol.isPrime(7))   # True
13 | print(sol.isPrime(10))  # False
14 | 


--------------------------------------------------------------------------------
/Double numbers but only if odd, else square:
--------------------------------------------------------------------------------
1 | f1 = lambda nums: [x*2 if x % 2 != 0 else x**2 for x in nums]
2 | print(f1([1, 2, 3, 4, 5]))
3 | # Output: [2, 4, 6, 16, 10]
4 | 


--------------------------------------------------------------------------------
/Exception Handling:
--------------------------------------------------------------------------------
 1 | ## ⚙️ Exception Handling Example – Safe Division
 2 | 
 3 | ```python
 4 | def safe_divide(a, b):
 5 |     try:
 6 |         result = a / b
 7 |     except ZeroDivisionError:
 8 |         print("Oops! Cannot divide by zero.")
 9 |     else:
10 |         print("Good work! Result is:", result)
11 |     finally:
12 |         print("Done.")
13 | 


--------------------------------------------------------------------------------
/Filter strings starting with a vowel:
--------------------------------------------------------------------------------
1 | f2 = lambda words: [w for w in words if w[0].lower() in 'aeiou']
2 | print(f2(["apple", "banana", "Orange", "grape", "umbrella"]))
3 | # Output: ['apple', 'Orange', 'umbrella']
4 | 


--------------------------------------------------------------------------------
/Find Remainder:
--------------------------------------------------------------------------------
 1 | def find_remainder(dividend: int, divisor: int) -> int:
 2 |     # your code here
 3 |     hlw =int(dividend % divisor)
 4 |     return hlw
 5 | 
 6 | 
 7 | print("Example:")
 8 | print(find_remainder(3, 2))
 9 | 
10 | # These "asserts" are used for self-checking
11 | assert find_remainder(10, 3) == 1
12 | assert find_remainder(14, 4) == 2
13 | assert find_remainder(27, 4) == 3
14 | assert find_remainder(10, 5) == 0
15 | assert find_remainder(10, 1) == 0
16 | assert find_remainder(5, 7) == 5
17 | assert find_remainder(7, 5) == 2
18 | 
19 | print("The mission is done! Click 'Check Solution' to earn rewards!")
20 | 


--------------------------------------------------------------------------------
/Find the factorial of a number (reduce):
--------------------------------------------------------------------------------
1 | from functools import reduce
2 | f6 = lambda n: reduce(lambda a, b: a * b, range(1, n+1))
3 | print(f6(5))
4 | # Output: 120
5 | 


--------------------------------------------------------------------------------
/Find the longest word in a sentence:
--------------------------------------------------------------------------------
1 | 
2 | f9 = lambda s: max(s.split(), key=len)
3 | print(f9("Python makes you think sharper"))
4 | # Output: sharper
5 | 


--------------------------------------------------------------------------------
/First Word (simplified:
--------------------------------------------------------------------------------
 1 | def first_word(text: str) -> str:
 2 |     # your code here
 3 |    
 4 |     return text.split()[0]
 5 | 
 6 | 
 7 | print("Example:")
 8 | print(first_word("Hello world"))
 9 | 
10 | # These "asserts" are used for self-checking
11 | assert first_word("Hello world") == "Hello"
12 | assert first_word("a word") == "a"
13 | assert first_word("greeting from CheckiO Planet") == "greeting"
14 | assert first_word("hi") == "hi"
15 | 
16 | print("The mission is done! Click 'Check Solution' to earn rewards!")
17 | 


--------------------------------------------------------------------------------
/Flatten a 2D list:
--------------------------------------------------------------------------------
1 | f7 = lambda lists: [x for sublist in lists for x in sublist]
2 | print(f7([[1, 2], [3, 4], [5, 6]]))
3 | # Output: [1, 2, 3, 4, 5, 6]
4 | 


--------------------------------------------------------------------------------
/Get unique elements from list (order preserved):
--------------------------------------------------------------------------------
1 | f8 = lambda nums: list(dict.fromkeys(nums))
2 | print(f8([1, 2, 2, 3, 1, 4]))
3 | # Output: [1, 2, 3, 4]
4 | 


--------------------------------------------------------------------------------
/Integer Sign Determination:
--------------------------------------------------------------------------------
 1 | def determine_sign(num: int) -> str:
 2 |     # your code here
 3 |     if num > 0 :
 4 |       return "positive"
 5 |     elif num<0 :
 6 |       return "negative"
 7 |     else:
 8 |      return "zero"
 9 | 
10 | 
11 | print("Example:")
12 | print(determine_sign(11))
13 | 
14 | # These "asserts" are used for self-checking
15 | assert determine_sign(5) == "positive"
16 | assert determine_sign(0) == "zero"
17 | assert determine_sign(-10) == "negative"
18 | assert determine_sign(1) == "positive"
19 | assert determine_sign(-1) == "negative"
20 | assert determine_sign(999) == "positive"
21 | assert determine_sign(-1000) == "negative"
22 | assert determine_sign(123456789) == "positive"
23 | assert determine_sign(-987654321) == "negative"
24 | assert determine_sign(2) == "positive"
25 | 
26 | print("The mission is done! Click 'Check Solution' to earn rewards!")
27 | 


--------------------------------------------------------------------------------
/Is Even:
--------------------------------------------------------------------------------
 1 | def is_even(num: int) -> bool:
 2 |     # your code here
 3 |     if num%2 == 0:
 4 |      return True
 5 |     else:
 6 |      return False
 7 |     
 8 |     
 9 | 
10 | 
11 | print("Example:")
12 | print(is_even(2))
13 | 
14 | # These "asserts" are used for self-checking
15 | assert is_even(2) == True
16 | assert is_even(5) == False
17 | assert is_even(0) == True
18 | 
19 | print("The mission is done! Click 'Check Solution' to earn rewards!")
20 | 


--------------------------------------------------------------------------------
/Just Fizz!:
--------------------------------------------------------------------------------
 1 | def checkio(num: int) -> str:
 2 |     # your code here
 3 |     if num % 3 ==0:
 4 |        return "Fizz"
 5 |     else:
 6 |      return str(num)
 7 | 
 8 | 
 9 | print("Example:")
10 | print(checkio(3))
11 | 
12 | # These "asserts" are used for self-checking
13 | assert checkio(15) == "Fizz"
14 | assert checkio(6) == "Fizz"
15 | assert checkio(10) == "10"
16 | assert checkio(7) == "7"
17 | 
18 | print("The mission is done! Click 'Check Solution' to earn rewards!")
19 | 


--------------------------------------------------------------------------------
/Merge two lists into a dictionary (zip):
--------------------------------------------------------------------------------
1 | f5 = lambda keys, vals: dict(zip(keys, vals))
2 | print(f5(['name', 'age'], ['Aadarsh', 24]))
3 | # Output: {'name': 'Aadarsh', 'age': 24}
4 | 


--------------------------------------------------------------------------------
/Multiply (Intro):
--------------------------------------------------------------------------------
 1 | def mult_two(a: int, b: int) -> int:
 2 |     # your code here
 3 |     result = a * b
 4 |     return result
 5 | 
 6 | 
 7 | print("Example")
 8 | print(mult_two(1, 2))
 9 | 
10 | assert mult_two(3, 2) == 6
11 | assert mult_two(0, 1) == 0
12 | 
13 | print("The first mission is done! Click 'Check' to earn cool rewards!")
14 | 


--------------------------------------------------------------------------------
/Probability & Statistics Examples in Python:
--------------------------------------------------------------------------------
 1 | """
 2 | Probability & Statistics Examples in Python
 3 | Author: Aadarsh Tiwari
 4 | Description: Collection of 10 examples demonstrating
 5 |              probability and statistics concepts in Python.
 6 | """
 7 | 
 8 | # 1. Probability of Specific Event (Basic Rule)
 9 | favorable_outcomes = 1
10 | total_outcomes = 6
11 | probability = favorable_outcomes / total_outcomes
12 | print("1. P(rolling a 4):", probability)
13 | 
14 | # 2. Complement Rule
15 | P_heads = 0.5
16 | P_not_heads = 1 - P_heads
17 | print("2. P(Not Heads):", P_not_heads)
18 | 
19 | # 3. Addition Rule for Mutually Exclusive Events
20 | P_A = 0.3
21 | P_B = 0.4
22 | P_A_or_B = P_A + P_B
23 | print("3. P(A or B) [Mutually Exclusive]:", P_A_or_B)
24 | 
25 | # 4. Addition Rule for Non-Mutually Exclusive Events
26 | P_A = 0.5
27 | P_B = 0.6
28 | P_A_and_B = 0.3
29 | P_A_or_B = P_A + P_B - P_A_and_B
30 | print("4. P(A or B) [Non-Mutually Exclusive]:", P_A_or_B)
31 | 
32 | # 5. Multiplication Rule for Independent Events
33 | P_A = 0.4
34 | P_B = 0.5
35 | P_A_and_B = P_A * P_B
36 | print("5. P(A and B) [Independent]:", P_A_and_B)
37 | 
38 | # 6. Multiplication Rule for Dependent Events
39 | P_A = 0.5
40 | P_B_given_A = 0.3
41 | P_A_and_B = P_A * P_B_given_A
42 | print("6. P(A and B) [Dependent]:", P_A_and_B)
43 | 
44 | # 7. Conditional Probability
45 | P_A_and_B = 0.2
46 | P_B = 0.4
47 | P_A_given_B = P_A_and_B / P_B
48 | print("7. P(A|B):", P_A_given_B)
49 | 
50 | # 8. Bayes’ Theorem
51 | P_D = 0.02          # P(Disease)
52 | P_not_D = 0.98      # P(No Disease)
53 | P_Pos_given_D = 0.90        # P(Positive | Disease)
54 | P_Pos_given_not_D = 0.05    # P(Positive | No Disease)
55 | 
56 | numerator = P_Pos_given_D * P_D
57 | denominator = (P_Pos_given_D * P_D) + (P_Pos_given_not_D * P_not_D)
58 | P_D_given_Pos = numerator / denominator
59 | print("8. P(Disease | Positive):", round(P_D_given_Pos, 4))
60 | 
61 | # 9. Binomial Probability
62 | from scipy.stats import binom
63 | n = 15
64 | p = 0.3
65 | k = 5
66 | probability = binom.pmf(k, n, p)
67 | print(f"9. P(X = {k} successes in {n} trials):", probability)
68 | 
69 | # 10. Normal Distribution Probability
70 | import scipy.stats as stats
71 | mean = 50
72 | std_dev = 10
73 | x = 60
74 | z_score = (x - mean) / std_dev
75 | P_less_than_x = stats.norm.cdf(z_score)
76 | print(f"10. P(X ≤ {x}):", P_less_than_x)
77 | 


--------------------------------------------------------------------------------
/Python + Pandas – Clean and Summarize Data:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | 
 3 | # Sample diabetic patient dataset
 4 | data = {
 5 |     'Patient_ID': [1, 2, 3, 4, 5],
 6 |     'Age': [25, None, 40, 55, None],
 7 |     'Blood_Sugar': [150, 180, None, 140, 200]
 8 | }
 9 | 
10 | df = pd.DataFrame(data)
11 | 
12 | # Data Cleaning
13 | df['Age'] = df['Age'].fillna(df['Age'].mean())
14 | df['Blood_Sugar'] = df['Blood_Sugar'].fillna(df['Blood_Sugar'].median())
15 | 
16 | # Summary Statistics
17 | summary = df.describe()
18 | 
19 | print(df)
20 | print(summary)


--------------------------------------------------------------------------------
/Rectangle Perimeter:
--------------------------------------------------------------------------------
 1 | def rectangle_perimeter(length: int, width: int) -> int:
 2 |     # your code here
 3 |     result = 2*(length+width)
 4 |   
 5 |     return result
 6 | 
 7 | 
 8 | print("Example:")
 9 | print(rectangle_perimeter(3, 2))
10 | 
11 | # These "asserts" are used for self-checking
12 | assert rectangle_perimeter(2, 4) == 12
13 | assert rectangle_perimeter(3, 5) == 16
14 | assert rectangle_perimeter(10, 20) == 60
15 | assert rectangle_perimeter(7, 2) == 18
16 | assert rectangle_perimeter(1, 1) == 4
17 | assert rectangle_perimeter(1, 5) == 12
18 | assert rectangle_perimeter(4, 1) == 10
19 | assert rectangle_perimeter(100, 100) == 400
20 | assert rectangle_perimeter(0.5, 2) == 5
21 | 
22 | print("The mission is done! Click 'Check Solution' to earn rewards!")
23 | 


--------------------------------------------------------------------------------
/Reverse each word in a sentence:
--------------------------------------------------------------------------------
1 | f3 = lambda s: ' '.join([w[::-1] for w in s.split()])
2 | print(f3("Python is fun"))
3 | # Output: nohtyP si nuf
4 | 


--------------------------------------------------------------------------------
/Sample Walking Data:
--------------------------------------------------------------------------------
 1 | Mini Project: Personal Health Tracker 7-Day Walking Tracker
 2 | import pandas as pd
 3 | import matplotlib.pyplot as plt
 4 | 
 5 | # 1. Sample Walking Data
 6 | data = {
 7 |     'Date': pd.date_range(start='2025-07-24', periods=7, freq='D'),
 8 |     'Walking_Minutes': [30, 45, 20, 60, 50, 35, 40]
 9 | }
10 | 
11 | df = pd.DataFrame(data)
12 | 
13 | # 2. Set Date as Index
14 | df.set_index('Date', inplace=True)
15 | 
16 | # 3. Show Full Data
17 | print("Full Walking Data:\n", df)
18 | 
19 | # 4. Calculate Weekly Stats
20 | print("\nAverage Walk (min):", df['Walking_Minutes'].mean())
21 | print("Max Walked on:", df['Walking_Minutes'].idxmax(), "→", df['Walking_Minutes'].max(), "min")
22 | print("Min Walked on:", df['Walking_Minutes'].idxmin(), "→", df['Walking_Minutes'].min(), "min")
23 | 
24 | # 5. Add Rolling Average (3-day)
25 | df['Rolling_Avg'] = df['Walking_Minutes'].rolling(window=3).mean()
26 | 
27 | # 6. Plot the Walking Trend
28 | df.plot(figsize=(10, 5), title='7-Day Walking Tracker')
29 | plt.ylabel("Walking Minutes")
30 | plt.grid(True)
31 | plt.show()
32 | 


--------------------------------------------------------------------------------
/Sort dictionary by value in descending order:
--------------------------------------------------------------------------------
1 | f4 = lambda d: dict(sorted(d.items(), key=lambda x: x[1], reverse=True))
2 | print(f4({'a': 3, 'b': 7, 'c': 1}))
3 | # Output: {'b': 7, 'a': 3, 'c': 1}
4 | 


--------------------------------------------------------------------------------
/analysis by pd:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | 
 3 | # Example: Analyzing sales data
 4 | data = {
 5 |     'Product': ['A', 'B', 'C', 'A', 'B'],
 6 |     'Sales': [100, 200, 150, 120, 220]
 7 | }
 8 | df = pd.DataFrame(data)
 9 | 
10 | # Total Sales
11 | total_sales = df['Sales'].sum()
12 | # Average Sales
13 | avg_sales = df['Sales'].mean()
14 | # Group by Product
15 | product_summary = df.groupby('Product')['Sales'].sum()
16 | 
17 | print("Total Sales:", total_sales)
18 | print("Average Sales:", avg_sales)
19 | print("Sales by Product:\n", product_summary)
20 | 


--------------------------------------------------------------------------------
/bmi calculater:
--------------------------------------------------------------------------------
 1 | # BMI Calculator
 2 | def bmi(weight, height):
 3 |     bmi_val = weight / (height ** 2)
 4 |     if bmi_val < 18.5:
 5 |         return "Underweight"
 6 |     elif bmi_val < 25:
 7 |         return "Normal"
 8 |     elif bmi_val < 30:
 9 |         return "Overweight"
10 |     else:
11 |         return "Obese"
12 | 
13 | print(bmi(70, 1.75))  # Normal
14 | 


--------------------------------------------------------------------------------
/calculater:
--------------------------------------------------------------------------------
 1 | def add(x, y): return x + y
 2 | def subtract(x, y): return x - y
 3 | def multiply(x, y): return x * y
 4 | def divide(x, y): return x / y
 5 | 
 6 | print(add(10, 5))       # 15
 7 | print(subtract(10, 5))  # 5
 8 | print(multiply(10, 5))  # 50
 9 | print(divide(10, 5))    # 2.0
10 | 


--------------------------------------------------------------------------------
/central tendancy:
--------------------------------------------------------------------------------
 1 | import statistics
 2 | 
 3 | class Solution(object):
 4 |     def statsSummary(self, data):
 5 |         return {
 6 |             "mean": statistics.mean(data),
 7 |             "median": statistics.median(data),
 8 |             "mode": statistics.mode(data)
 9 |         }
10 | 
11 | # Example
12 | sol = Solution()
13 | print(sol.statsSummary([1, 2, 2, 3, 4]))
14 | 


--------------------------------------------------------------------------------
/class book:
--------------------------------------------------------------------------------
 1 | class Book:
 2 |     def __init__(self, title, author, pages):
 3 |         self.title = title
 4 |         self.author = author
 5 |         self.pages = pages
 6 | 
 7 |     def boss(self):
 8 |         print(f"The title of the book is {self.title}")
 9 |         print(f"The author of the book is {self.author}")
10 |         print(f"The number of pages is {self.pages}")
11 | 
12 | # Example objects
13 | book1 = Book("Python", "Aadarsh", 320)
14 | book2 = Book("SQL", "Aadarsh", 200)
15 | 
16 | book1.boss()
17 | book2.boss()
18 | 


--------------------------------------------------------------------------------
/delete,fill,see nan value , for nan value use:
--------------------------------------------------------------------------------
 1 | # 1. Check for missing values
 2 | print(df.isnull())
 3 | 
 4 | # 2. Drop rows with any NaN values
 5 | df_dropped = df.dropna()
 6 | print(df_dropped)
 7 | 
 8 | # 3. Replace all NaN values with 0
 9 | df_filled = df.fillna(0)
10 | print(df_filled)
11 | 


--------------------------------------------------------------------------------
/df.iloc use:
--------------------------------------------------------------------------------
 1 | 
 2 | import pandas as pd
 3 | 
 4 | data = {
 5 |     'Day': ['Monday', 'Tuesday', 'Wednesday'],
 6 |     'Steps': [8000, 7200, 9000],
 7 |     'Walking_Minutes': [35, None, 45]
 8 | }
 9 | 
10 | df = pd.DataFrame(data)
11 | df.iloc[0, 1]
12 | 


--------------------------------------------------------------------------------
/difference =, ==:
--------------------------------------------------------------------------------
1 | a = [1, 2, 3]
2 | b = [1, 2, 3]
3 | 
4 | print(a == b)  # True (same value)
5 | print(a is b)  # False (different objects)
6 | 


--------------------------------------------------------------------------------
/erroe handaling of  ZeroDivisionError:
--------------------------------------------------------------------------------
1 | try:
2 |     result = 10 / 0
3 | except ZeroDivisionError:
4 |     print("Cannot divide by zero!")
5 | 


--------------------------------------------------------------------------------
/factoriyal:
--------------------------------------------------------------------------------
1 | def factorial(n):
2 |     if n == 0 or n == 1:
3 |         return 1
4 |     return n * factorial(n - 1)
5 | 
6 | # Example
7 | print(factorial(5))  # 120
8 | 


--------------------------------------------------------------------------------
/filw handaling with write:
--------------------------------------------------------------------------------
1 | with open("file.txt", "w") as f:
2 |     f.write("Hello world")
3 | 


--------------------------------------------------------------------------------
/find outlier:
--------------------------------------------------------------------------------
 1 | import numpy as np
 2 | import matplotlib.pyplot as plt
 3 | 
 4 | data = [12, 15, 14, 10, 19, 100, 13, 14, 15, 16]
 5 | q1 = np.percentile(data, 25)
 6 | q3 = np.percentile(data, 75)
 7 | iqr = q3 - q1
 8 | 
 9 | lower = q1 - 1.5 * iqr
10 | upper = q3 + 1.5 * iqr
11 | outliers = [x for x in data if x < lower or x > upper]
12 | 
13 | plt.boxplot(data)
14 | plt.title("Boxplot with Outliers")
15 | plt.show()
16 | 
17 | print("Outliers:", outliers)
18 | 


--------------------------------------------------------------------------------
/for cleaning data:
--------------------------------------------------------------------------------
 1 | df.isnull()         # Shows True/False for each cell
 2 | df.isnull().sum()   # Total missing in each column
 3 | df.dropna()               # Drops rows with ANY missing value
 4 | df.dropna(axis=1)         # Drops columns with ANY missing value
 5 | df.dropna(thresh=2)       # Drops rows with less than 2 non-null values
 6 | df.fillna(0)                        # Fill all NaNs with 0
 7 | df['Age'].fillna(df['Age'].mean()) # Fill Age column NaNs with mean
 8 | df.fillna(method='ffill')          # Forward fill (copy previous)
 9 | df.fillna(method='bfill')          # Backward fill (copy next)
10 | df.groupby('Dept').mean()          #This gives average salary per Dept
11 | df.groupby('Dept')['Salary'].agg(['mean', 'max', 'min'])
12 | emp = pd.DataFrame({                             # Like SQL joins — used to combine two tables.
13 |     'EmpID': [1, 2, 3],
14 |     'Name': ['Aadarsh', 'Raj', 'Priya']
15 | })
16 | 
17 | sal = pd.DataFrame({
18 |     'EmpID': [1, 2, 4],
19 |     'Salary': [50000, 60000, 45000]
20 | })
21 | 
22 | pd.merge(emp, sal, on='EmpID')      #Merge (like INNER JOIN)
23 | pd.merge(emp, sal, on='EmpID', how='left')   # Left Join
24 | pd.merge(emp, sal, on='EmpID', how='right')  # Right Join
25 | pd.merge(emp, sal, on='EmpID', how='outer')  # Full Outer Join
26 | 
27 | 
28 | 


--------------------------------------------------------------------------------
/health data cleaning for py:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | import numpy as np
 3 | 
 4 | # Simulated health data with missing values
 5 | df = pd.DataFrame({
 6 |     'Date': pd.date_range(start='2025-08-01', periods=5),
 7 |     'Steps': [5000, np.nan, 7000, np.nan, 10000],
 8 |     'Sleep_Hours': [6.5, 7.0, np.nan, 8.0, 6.0]
 9 | })
10 | 
11 | # Fill missing steps with average
12 | df['Steps'].fillna(df['Steps'].mean(), inplace=True)
13 | # Drop rows where sleep data is missing
14 | df.dropna(subset=['Sleep_Hours'], inplace=True)
15 | 
16 | print(df)
17 | 


--------------------------------------------------------------------------------
/lambda_use:
--------------------------------------------------------------------------------
 1 | # Q1
 2 | hlw1 = lambda words: [word[::-1] for word in words]
 3 | print(hlw1(["python", "lambda"]))
 4 | 
 5 | # Q2
 6 | hlw2 = lambda a, b: [a[i] * b[i] for i in range(len(a))]
 7 | print(hlw2([2, 4, 6], [1, 2, 3]))
 8 | 
 9 | # Q3
10 | hlw3 = lambda d: {k.upper(): v for k, v in d.items()}
11 | print(hlw3({"name": "Aadarsh", "city": "Delhi"}))
12 | 
13 | # Q4
14 | hlw4 = lambda nums: [n**2 for n in nums if n % 2 != 0]
15 | print(hlw4([1, 2, 3, 4, 5]))
16 | 
17 | # Q5
18 | hlw5 = lambda words: [word[0] for word in words]
19 | print(hlw5(["Python", "Is", "Fun"]))
20 | 


--------------------------------------------------------------------------------
/largest element:
--------------------------------------------------------------------------------
 1 | def find_max(lst):
 2 |     max_val = lst[0]
 3 |     for num in lst:
 4 |         if num > max_val:
 5 |             max_val = num
 6 |     return max_val
 7 | 
 8 | # Example
 9 | print(find_max([10, 25, 78, 34]))  # 78
10 | 


--------------------------------------------------------------------------------
/list comp:
--------------------------------------------------------------------------------
1 | #  Filter names starting with 'A'
2 | 
3 | names = ["Aadarsh", "Riya", "Aman", "Sohail", "Aditi", "Neha"]
4 | 
5 | # Filter names
6 | a_names = [name for name in names if name.startswith('A')]
7 | print("Names starting with 'A':", a_names)
8 | 


--------------------------------------------------------------------------------
/list comparistions:
--------------------------------------------------------------------------------
1 | # Answer:
2 | # Shorter way to write for loops on lists.
3 | 
4 | nums = [1, 2, 3, 4]
5 | squared = [x**2 for x in nums]
6 | print("Squared:", squared)
7 | 


--------------------------------------------------------------------------------
/map(),filter():
--------------------------------------------------------------------------------
 1 | # Answer:
 2 | # map() transforms all items.
 3 | # filter() keeps only those that match a condition.
 4 | 
 5 | nums = [1, 2, 3, 4, 5]
 6 | doubled = list(map(lambda x: x*2, nums))
 7 | evens = list(filter(lambda x: x%2==0, nums))
 8 | print("Mapped:", doubled)
 9 | print("Filtered:", evens)
10 | 


--------------------------------------------------------------------------------
/max min:
--------------------------------------------------------------------------------
 1 | #  Salary list analysis - Find total, average, min, max salary
 2 | 
 3 | salaries = [38000, 42000, 50000, 47000, 39000, 56000, 61000, 48000]
 4 | 
 5 | # Total number of employees
 6 | total_employees = len(salaries)
 7 | 
 8 | # Average salary
 9 | average_salary = sum(salaries) / total_employees
10 | 
11 | # Minimum and Maximum salary
12 | min_salary = min(salaries)
13 | max_salary = max(salaries)
14 | 
15 | # Output results
16 | print("Total Employees:", total_employees)
17 | print("Average Salary:", average_salary)
18 | print("Minimum Salary:", min_salary)
19 | print("Maximum Salary:", max_salary)
20 | 


--------------------------------------------------------------------------------
/more_lambda:
--------------------------------------------------------------------------------
 1 | # Q1
 2 | hlw = lambda nums: [x + 5 for x in nums]
 3 | print(hlw([1, 2, 3, 4, 5]))
 4 | 
 5 | # Q2
 6 | hlw = lambda nums: [x.upper() for x in nums]
 7 | print(hlw(["python", "lambda", "practice"]))
 8 | 
 9 | # Q3
10 | hlw = lambda nums: [x for x in nums if x % 2 == 0]
11 | print(hlw([10, 15, 20, 25, 30]))
12 | 


--------------------------------------------------------------------------------
/num:
--------------------------------------------------------------------------------
 1 | import numpy as np
 2 | from scipy.stats import norm
 3 | 
 4 | n = 36
 5 | mean = 52
 6 | std_dev = 8
 7 | z_score = 1.96  # for 95% confidence
 8 | 
 9 | se = std_dev / np.sqrt(n)
10 | margin = z_score * se
11 | ci = (mean - margin, mean + margin)
12 | print("Confidence Interval:", ci)
13 | 


--------------------------------------------------------------------------------
/oops:
--------------------------------------------------------------------------------
1 | class Person:
2 |     def __init__(self, name):
3 |         self.name = name
4 | 
5 |     def greet(self):
6 |         return f"Hi {self.name}"
7 | 


--------------------------------------------------------------------------------
/palindrome:
--------------------------------------------------------------------------------
1 | # Check if a string is palindrome
2 | def is_palindrome(s):
3 |     return s == s[::-1]
4 | 
5 | print(is_palindrome("radar"))  # True
6 | print(is_palindrome("apple"))  # False
7 | 


--------------------------------------------------------------------------------
/pd 1:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | 
 3 | data = {
 4 |     'Day': ['Monday', 'Tuesday', 'Wednesday'],
 5 |     'Steps': [8000, 7200, 9000],
 6 |     'Walking_Minutes': [35, None, 45]
 7 | }
 8 | 
 9 | df = pd.DataFrame(data)
10 | 
11 | # Fill missing values with 30
12 | df['Walking_Minutes'] = df['Walking_Minutes'].fillna(30)
13 | 
14 | # Access only the 'Steps' column
15 | steps_column = df['Steps']
16 | 
17 | print(df)
18 | print("Steps column:")
19 | print(steps_column)
20 | 


--------------------------------------------------------------------------------
/pd for data analysis:
--------------------------------------------------------------------------------
1 | import pandas as pd
2 | df = pd.read_csv("data.csv")
3 | print(df.head())
4 | 


--------------------------------------------------------------------------------
/prime:
--------------------------------------------------------------------------------
 1 | def is_prime(n):
 2 |     if n <= 1:
 3 |         return False
 4 |     for i in range(2, int(n**0.5)+1):
 5 |         if n % i == 0:
 6 |             return False
 7 |     return True
 8 | 
 9 | # Example
10 | print(is_prime(7))   # True
11 | print(is_prime(10))  # False
12 | 


--------------------------------------------------------------------------------
/prime nu:
--------------------------------------------------------------------------------
1 | # Program to find all prime numbers from 1 to 100
2 | for num in range(2, 101):
3 |     for i in range(2, num):
4 |         if num % i == 0:
5 |             break
6 |     else:
7 |         print(num, end=' ')
8 | 


--------------------------------------------------------------------------------
/python-basics/README.md:
--------------------------------------------------------------------------------
https://raw.githubusercontent.com/aadarsh3419/python/e99de4d764149c67b761a79229ba17387d71f821/python-basics/README.md


--------------------------------------------------------------------------------
/python-basics/array_operations.py:
--------------------------------------------------------------------------------
https://raw.githubusercontent.com/aadarsh3419/python/e99de4d764149c67b761a79229ba17387d71f821/python-basics/array_operations.py


--------------------------------------------------------------------------------
/python-basics/numpy_basics.py:
--------------------------------------------------------------------------------
https://raw.githubusercontent.com/aadarsh3419/python/e99de4d764149c67b761a79229ba17387d71f821/python-basics/numpy_basics.py


--------------------------------------------------------------------------------
/random password  generater:
--------------------------------------------------------------------------------
1 | import random
2 | import string
3 | 
4 | def generate_password(length=12):
5 |     chars = string.ascii_letters + string.digits + string.punctuation
6 |     return ''.join(random.choice(chars) for _ in range(length))
7 | 
8 | print("Generated Password:", generate_password())
9 | 


--------------------------------------------------------------------------------
/read write file:
--------------------------------------------------------------------------------
 1 | # Answer:
 2 | # Writing
 3 | with open("sample.txt", "w") as f:
 4 |     f.write("Hello, GitHub!")
 5 | 
 6 | # Reading
 7 | with open("sample.txt", "r") as f:
 8 |     content = f.read()
 9 |     print(content)
10 | 


--------------------------------------------------------------------------------
/recursion:
--------------------------------------------------------------------------------
1 | def factorial(n):
2 |     if n == 0:
3 |         return 1
4 |     return n * factorial(n - 1)
5 | 
6 | print(factorial(5))  # Output: 120
7 | 


--------------------------------------------------------------------------------
/remove duplicate:
--------------------------------------------------------------------------------
1 | def remove_duplicates(lst):
2 |     return list(set(lst))
3 | 
4 | # Example
5 | print(remove_duplicates([1, 2, 2, 3, 4, 4, 5]))  # [1, 2, 3, 4, 5]
6 | 


--------------------------------------------------------------------------------
/reverse string:
--------------------------------------------------------------------------------
1 | def reverse_string(s):
2 |     return s[::-1]
3 | 
4 | # Example
5 | print(reverse_string("DataScience"))  # ecneicSataD
6 | 


--------------------------------------------------------------------------------
/reverse string 1:
--------------------------------------------------------------------------------
1 | class Solution(object):
2 |     def reverseString(self, s):
3 |         return s[::-1]
4 | 
5 | # Example
6 | sol = Solution()
7 | print(sol.reverseString("Aadarsh"))  # hsradaa
8 | 


--------------------------------------------------------------------------------
/roman number:
--------------------------------------------------------------------------------
 1 | # Intuition
 2 | <!-- Describe your first thoughts on how to solve this problem. -->
 3 | 
 4 | # Approach
 5 | <!-- Describe your approach to solving the problem. -->
 6 | 
 7 | # Complexity
 8 | - Time complexity:
 9 | <!-- Add your time complexity here, e.g. $O(n)$ -->
10 | 
11 | - Space complexity:
12 | <!-- Add your space complexity here, e.g. $O(n)$ -->
13 | 
14 | # Code
15 | ```python []
16 | class Solution(object):
17 |     def romanToInt(self, s):
18 |         values = {
19 |             "I": 1,
20 |             "V": 5,
21 |             "X": 10,
22 |             "L": 50,
23 |             "C": 100,
24 |             "D": 500,
25 |             "M": 1000
26 |         }
27 |         
28 |         total = 0
29 |         prev = 0
30 |         
31 |         for char in reversed(s):
32 |             val = values[char]
33 |             if val < prev:
34 |                 total -= val
35 |             else:
36 |                 total += val
37 |             prev = val
38 |         
39 |         return total
40 | 
41 | ```
42 | 


--------------------------------------------------------------------------------
/student grade system:
--------------------------------------------------------------------------------
 1 | # Calculate grade of student
 2 | def grade_calculator(marks):
 3 |     avg = sum(marks) / len(marks)
 4 |     if avg >= 90:
 5 |         return "A"
 6 |     elif avg >= 75:
 7 |         return "B"
 8 |     elif avg >= 60:
 9 |         return "C"
10 |     elif avg >= 40:
11 |         return "D"
12 |     else:
13 |         return "F"
14 | 
15 | print(grade_calculator([88, 76, 92, 85]))
16 | 


--------------------------------------------------------------------------------
/student grading system:
--------------------------------------------------------------------------------
 1 | This Python class simulates a student grading system.
 2 | 
 3 | __init__: Initializes student name and marks.
 4 | 
 5 | grade(): Prints the student's name, marks, and whether they Passed ✅ or Failed ❌ based on a passing mark of 40.
 6 | 
 7 | Two students (Aalok and Aadarsh) are created with different marks.
 8 | 
 9 | The result is printed for each student.
10 | 
11 | 📌 Logic:
12 | If a student's marks are ≥ 40, they pass.
13 | If marks are < 40, they fail.
14 | 
15 | class Student: 
16 |     def __init__(self, name, marks):
17 |         self.name = name
18 |         self.marks = marks
19 | 
20 |     def grade(self):
21 |         print(f"Marks of {self.name} is {self.marks}")
22 |         if self.marks >= 40:
23 |             print("Result: Passed ✅\n")
24 |         else:
25 |             print("Result: Failed ❌\n")
26 | 
27 | # Create students with numeric marks
28 | student1 = Student("Aalok", 38)
29 | student2 = Student("Aadarsh", 89)
30 | 
31 | student1.grade()
32 | student2.grade()
33 | 


--------------------------------------------------------------------------------
/tiny litele clean data:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | 
 3 | data = {
 4 |     'Name': ['Aadarsh', 'Ravi', 'Priya', None],
 5 |     'Steps': [7000, 8500, None, 9000],
 6 |     'Walking_Minutes': [30, 40, 25, None]
 7 | }
 8 | 
 9 | df = pd.DataFrame(data)
10 | 
11 | df_cleaned = df.dropna()     # Removed rows with missing values
12 | print(df_cleaned)
13 | 


--------------------------------------------------------------------------------
/use of df.loc:
--------------------------------------------------------------------------------
 1 | import pandas as pd
 2 | 
 3 | data = {
 4 |     'Day': ['Monday', 'Tuesday', 'Wednesday'],
 5 |     'Steps': [8000, 7200, 9000],
 6 |     'Walking_Minutes': [35, None, 45]
 7 | }
 8 | 
 9 | df = pd.DataFrame(data)
10 | df.loc[df['Day'] == 'Wednesday', 'Steps'].values[0]
11 | 


--------------------------------------------------------------------------------
/using encapculation:
--------------------------------------------------------------------------------
 1 | class Car:
 2 |     def __init__(self):
 3 |         self.__speed = 0  # Private attribute to store speed
 4 | 
 5 |     def accelerate(self, amount):
 6 |         if amount > 0:
 7 |             self.__speed += amount
 8 |             print(f"Accelerated by {amount}. Current speed: {self.__speed} km/h")
 9 |         else:
10 |             print("Speed increase must be positive!")
11 | 
12 |     def brake(self, amount):
13 |         if amount > 0:
14 |             self.__speed = max(0, self.__speed - amount)
15 |             print(f"Braked by {amount}. Current speed: {self.__speed} km/h")
16 |         else:
17 |             print("Brake amount must be positive!")
18 | 
19 |     def get_speed(self):
20 |         return self.__speed
21 | 
22 | 
23 | # Example usage
24 | my_car = Car()
25 | my_car.accelerate(50)
26 | my_car.brake(20)
27 | print("Final Speed:", my_car.get_speed(), "km/h")
28 | 


--------------------------------------------------------------------------------
/vowels in string find:
--------------------------------------------------------------------------------
1 | def count_vowels(s):
2 |     vowels = "aeiouAEIOU"
3 |     return sum(1 for char in s if char in vowels)
4 | 
5 | # Example
6 | print(count_vowels("Aadarsh Tiwari"))  # 6
7 | 


--------------------------------------------------------------------------------
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




import pandas as pd
import matplotlib.pyplot as plt

# 1. Sample Walking Data
data = {
    'Date': pd.date_range(start='2025-07-24', periods=7, freq='D'),
    'Walking_Minutes': [30, 45, 20, 60, 50, 35, 40]
}

df = pd.DataFrame(data)

# 2. Set Date as Index
df.set_index('Date', inplace=True)

# 3. Show Full Data
print("Full Walking Data:\n", df)

# 4. Calculate Weekly Stats
print("\nAverage Walk (min):", df['Walking_Minutes'].mean())
print("Max Walked on:", df['Walking_Minutes'].idxmax(), "→", df['Walking_Minutes'].max(), "min")
print("Min Walked on:", df['Walking_Minutes'].idxmin(), "→", df['Walking_Minutes'].min(), "min")

# 5. Add Rolling Average (3-day)
df['Rolling_Avg'] = df['Walking_Minutes'].rolling(window=3).mean()

# 6. Plot the Walking Trend
df.plot(figsize=(10, 5), title='7-Day Walking Tracker')
plt.ylabel("Walking Minutes")
plt.grid(True)
plt.show()


