[README.md](https://github.com/user-attachments/files/34969559/README.md)
# Python Assignment 1: Data Structures – Strings & Tuples

**Author:** Aiswarya Krishna G
**Tools:** Python 3, Jupyter Notebook

## Overview

This assignment covers the basics of two core Python data structures: **strings** and **tuples**. It includes string concatenation, indexing and slicing, built-in string methods, and tuple creation, concatenation, repetition and access.

## Concepts Covered

- String concatenation using `+` and user input with `input()`
- String indexing and slicing (including negative indices and reversing with `[::-1]`)
- String methods: `upper()`, `lower()`, `capitalize()`, `count()`, `replace()`, `index()`
- Tuple creation, concatenation (`+`), repetition (`*`), indexing and slicing
- Immutability of strings and tuples

---

## Part 1: Strings

### 1. String Concatenation

```python
string1 = "Hello "
string2 = input("Enter your Name: ")
greeting = string1 + string2
print(greeting)

string3 = ", welcome to Python programming"
greeting = greeting + string3
print(greeting)
```

**Sample Output**
```
Enter your Name: Zara
Hello Zara
Hello Zara, welcome to Python programming
```

### 2. String Slicing and Indexing

```python
text = greeting

print(text[0])                 # a. first character
print(text[-1])                # b. last character
print(text[:5])                # c. first 5 characters
print(text[-11:])              # d. last 11 characters
print(text[::-1])              # e. reversed string

start = text.index("Python")
print(text[start:start + 6])   # f. the word "Python"
```

**Output**
```
H
g
Hello
programming
gnimmargorp nohtyP ot emoclew ,araZ olleH
Python
```

### 3. String Methods

```python
strM = "Python beginner tutorial"

print(strM.upper())                         # a. uppercase
print(strM.lower())                         # b. lowercase
print(strM.lower().capitalize())            # c. back to original form
print(strM.count("t"))                      # d. occurrences of 't'
print(strM.replace("Python", "Machine Learning"))  # e. replace
```

**Output**
```
PYTHON BEGINNER TUTORIAL
python beginner tutorial
Python beginner tutorial
3
Machine Learning beginner tutorial
```

---

## Part 2: Tuples

```python
tuple1 = (10, 20, 30)
tuple2 = (40, 50, 60)

t_combine = tuple1 + tuple2      # a. concatenate
print(t_combine)

print(t_combine * 3)             # b. repeat 3 times
print(t_combine[2])              # c. 3rd element
print(t_combine[:3])             # d. first three elements
print(t_combine[-3:])            # e. last three elements
```

**Output**
```
(10, 20, 30, 40, 50, 60)
(10, 20, 30, 40, 50, 60, 10, 20, 30, 40, 50, 60, 10, 20, 30, 40, 50, 60)
30
(10, 20, 30)
(40, 50, 60)
```

---

## Key Takeaways

- Strings and tuples are **immutable**: operations like concatenation, `replace()` and repetition create new objects instead of changing the original.
- Indexing starts at `0`; negative indices count from the end.
- Slicing follows `[start:stop:step]`, where `stop` is excluded.
- `count()` is case-sensitive.

## How to Run

1. Open the notebook in Jupyter Notebook.
2. Run the cells in order (**Shift + Enter**), or use **Kernel → Restart & Run All**.
3. Enter a name when prompted in the first cell.
