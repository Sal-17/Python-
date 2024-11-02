
1.  Find the type of the following variables.
   1. `x = 2`
   2. `x = 2.0`
   3. `x = "2.0"`
   4. `x = 2 + 0j`
   5.  `x = "2 + 0j"`
   6.  `x = math.pi` \# import math module first!
x = 2
type(x)
x = 2.0
type(x)
x = "2.0"
type(x)
x = 2 + 0j
type(x)
x = "2 + 0j"
type(x)
import math
x = math.pi 
type(x)
2.  Generate the following string variable `s = "Python has a nice syntax."`
   1.  Compute the number of characters in `s`.
   2.  Slice `s` to obtain the substring `"syntax"`.
   3.  Find the first occurrence of `"a"` in `s`.
   4.  Replace all occurrences of `"a"` in `s` to `"A"`.
   5.  Add the following string to `s`, `"But, Stata's is counter-intuitive"`.
len(s)
 s[-7:-1]
s.find("a")
s.replace("a", "A")
s + " But, Stata's is counter-intuitive."
3.  Generate the following list, `y = [[1,math.pi,0,7,8], ["abc", bool(0), -3, 12]]`.
   1.  Reverse the first list in `y` using a reverse method.
   2.  Replace `bool(0)` to `bool(1)` in the second list in `y`.
   3.  Drop `pi` from the first list in `y`.
   4.  Add `[math.pi, math.e, 3-1j, False]` to `y`.
y[0].reverse()
y
y[1][1] = bool(1)
y
y[0].remove(math.pi)
y
y.append([math.pi, math.e, 3-1j, False])
y
4. (15 pts) Let `z` be equal to `y` in 3.D, `z = y`.
   1. Replace `z[2][0]` to `True`. What happened to `y`? Did it change also?
   2. How should we generate `z` so that the definition of `y` remains unaffected? Note that `copy` method will not work here.
z = y
z
z[2][0] = True
z
Since z and y point to the same list, any changes made to z[2][0] also affect y[2][0].
5.  Generate a dictionary named `student` with the following keys: `"name"`, `"age"`, `"courses"`, `"phone"` and corresponding values `"Jane"`, `22`, `["MATH131", "ANTH201"]`, `"555-788-5544"`.
   1. Print student's phone.
   2. Update student's `age` to `24` and `courses` to `["MATH131", "ANTH201", "ECO387"]`.
   3. Drop the phone number from the dictionary.
   4. Generate a new string variable named `courses` from the values in `courses` such that course names are separated by `"-"`. Then, print it.
student = {
    "name": "Jane",
    "age": 22,
    "courses": ["MATH131", "ANTH201"],
    "phone": "555-788-5544"
}
print(student["phone"])
student["age"] = 24
student["courses"] = ["MATH131", "ANTH201", "ECO387"]
student
student.pop("phone")
courses = "-".join(student["courses"])
print(courses)
6.  Generate an empty set named `w1`.
   1. Add the following elements to `w1: {2,4,6,...,100}`.
   2. Find the number of elements in the intersection of `w1` and `w2`.
   3. Find the number of elements in the set difference between `w2` and `w1`.
w1 = set()
w1 = {i for i in range(2, 101, 2)}
w2 = {i for i in range(1, 51)}  # Example w2 set

intersection_count = len(w1.intersection(w2))
difference_count = len(w2.difference(w1))
intersection_count 
difference_count# Python-
Python Fundamentals and Data Manipulation Exercises with Lists, Strings, Dictionaries, and Sets
