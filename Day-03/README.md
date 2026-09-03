# Day 03 — Python Fundamentals

## 📌 Topic

- Variables
- Arithmetic Operators
- Comparison Operators
- Logical Operators
- If / Elif / Else
- For Loops
- range()
- Lists
- List Indexing
- append()
- remove()
- len()
- Finding Largest and Smallest Numbers
- Working with Even and Odd Numbers
- Calculating Sums

---

## 1. Variables

A variable is a name used to store a value.

Example:

    name = "Yashaswini"
    age = 21

    print(name)
    print(age)

Output:

    Yashaswini
    21

---

## 2. Arithmetic Operators

Python supports common arithmetic operators.

    x = 10
    y = 5

    print(x + y)
    print(x - y)
    print(x * y)

Output:

    15
    5
    50

### Division Operators

    x = 10
    y = 3

    print(x / y)
    print(x // y)
    print(x % y)

Output:

    3.3333333333333335
    3
    1

| Operator | Meaning |
|---|---|
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Normal division |
| `//` | Floor division |
| `%` | Remainder |

---

## 3. Comparison Operators

Comparison operators compare two values and return True or False.

    a = 10
    b = 5

    print(a > b)
    print(a < b)
    print(a == b)
    print(a != b)

Output:

    True
    False
    False
    True

| Operator | Meaning |
|---|---|
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater than or equal to |
| `<=` | Less than or equal to |
| `==` | Equal to |
| `!=` | Not equal to |

---

## 4. Assignment vs Comparison

`=` means assignment.

    a = 10

It assigns 10 to `a`.

`==` means comparison.

    a == 10

It checks whether `a` is equal to 10.

---

## 5. Logical Operators

Logical operators are used to combine conditions.

    marks = 85
    attendance = 72

    print(marks >= 80)
    print(attendance >= 75)
    print(marks >= 80 and attendance >= 75)

Output:

    True
    False
    False

| Operator | Meaning |
|---|---|
| `and` | Both conditions must be True |
| `or` | At least one condition must be True |
| `not` | Reverses True/False |

---

## 6. If / Else

Conditional statements allow a program to make decisions.

    marks = 65

    if marks >= 70:
        print("Pass")
    else:
        print("Fail")

Output:

    Fail

Python uses indentation to identify the code belonging to a condition.

---

## 7. If / Elif / Else

Multiple conditions can be checked using `if`, `elif`, and `else`.

    marks = 85

    if marks >= 90:
        print("Excellent")
    elif marks >= 70:
        print("Good")
    else:
        print("Needs Improvement")

Output:

    Good

Python checks the conditions from top to bottom.

Once a condition is True, its block is executed.

---

## 8. Student Classification

I practiced multiple conditions using marks.

    marks = 85

    if marks >= 90:
        print("Excellent")
    elif marks >= 70:
        print("Good")
    elif marks >= 50:
        print("Average")
    else:
        print("Fail")

---

## 9. For Loop

A `for` loop is used to repeat an operation for multiple values.

    for i in range(5):
        print(i)

Output:

    0
    1
    2
    3
    4

### Important Rule

`range(5)` starts from 0 and stops before 5.

    range(5)
    → 0, 1, 2, 3, 4

---

## 10. range(start, stop)

    for i in range(2, 7):
        print(i)

Output:

    2
    3
    4
    5
    6

The start value is included, but the stop value is excluded.

---

## 11. range(start, stop, step)

    for i in range(2, 11, 2):
        print(i)

Output:

    2
    4
    6
    8
    10

The third value represents the step.

---

## 12. Negative Step

A negative step allows us to count backwards.

    for i in range(10, 0, -2):
        print(i)

Output:

    10
    8
    6
    4
    2

---

## 13. Finding Even Numbers

I combined a `for` loop with the remainder operator.

    for i in range(2, 11):
        if i % 2 == 0:
            print(i)

Output:

    2
    4
    6
    8
    10

The expression `i % 2 == 0` checks whether a number is even.

---

## 14. Even and Odd Numbers

    for i in range(1, 11):
        if i % 2 == 0:
            print(i, "Even")
        else:
            print(i, "Odd")

Output:

    1 Odd
    2 Even
    3 Odd
    4 Even
    5 Odd
    6 Even
    7 Odd
    8 Even
    9 Odd
    10 Even

---

## 15. Calculating a Sum Using a Loop

I learned how to use an accumulator variable.

    total = 0

    for i in range(1, 11):
        total = total + i

    print(total)

Output:

    55

The `total` variable is updated during every iteration.

---

## 16. Lists

A list stores multiple values in a single variable.

    numbers = [10, 25, 7, 42, 18]

---

## 17. List Indexing

Python list indexing starts from 0.

    numbers = [10, 25, 7, 42, 18]

    print(numbers[0])
    print(numbers[2])
    print(numbers[-1])

Output:

    10
    7
    18

Index positions:

    Index:    0    1   2    3   4
    Value:   10   25   7   42  18

Negative indexing starts from the end:

    Index:   -5   -4   -3   -2   -1
    Value:   10   25    7   42   18

---

## 18. append()

`append()` adds an element to the end of a list.

    numbers = [10, 20, 30]

    numbers.append(40)

    print(numbers)

Output:

    [10, 20, 30, 40]

---

## 19. remove()

`remove()` removes an element from a list using its value.

    numbers = [10, 20, 30, 40]

    numbers.remove(30)

    print(numbers)

Output:

    [10, 20, 40]

---

## 20. len()

`len()` returns the number of elements in a list.

    numbers = [10, 20, 30, 40, 50]

    print(len(numbers))

Output:

    5

---

## 21. Finding the Largest Number

I practiced finding the largest number without using the built-in `max()` function.

    numbers = [10, 25, 7, 42, 18]

    temp = numbers[0]

    for number in numbers:
        if number > temp:
            temp = number

    print(temp)

Output:

    42

### Logic

I initially assume the first number is the largest.

Then I compare every number with the current largest value.

If a bigger number is found, I update the value.

---

## 22. Finding the Smallest Number

I used the same idea to find the smallest number.

    numbers = [10, 25, 7, 42, 18]

    temp = numbers[0]

    for number in numbers:
        if number < temp:
            temp = number

    print(temp)

Output:

    7

The main difference is:

    number > temp

is used for finding the largest number.

    number < temp

is used for finding the smallest number.

---

## 23. Finding Both Smallest and Largest

    numbers = [10, 25, 7, 42, 18]

    # Find smallest
    temp = numbers[0]

    for number in numbers:
        if number < temp:
            temp = number

    print(temp)

    # Find largest
    temp = numbers[0]

    for number in numbers:
        if number > temp:
            temp = number

    print(temp)

Output:

    7
    42

---

## 24. Sum of Only Even Numbers

I combined lists, loops, conditions, and the `%` operator.

    numbers = [10, 15, 20, 25, 30]

    total = 0

    for number in numbers:
        if number % 2 == 0:
            total = total + number

    print(total)

Output:

    60

Calculation:

    10 + 20 + 30 = 60

---

## 🧠 What I Learned

- Variables
- Arithmetic operators
- Comparison operators
- Logical operators
- `if / elif / else`
- `for` loops
- `range()`
- Lists
- List indexing
- `append()`
- `remove()`
- `len()`
- Accumulator variables
- Finding minimum and maximum values
- Working with even and odd numbers
- Combining loops and conditions

---

## 🛠️ Practice Completed

I practiced:

1. Arithmetic operations
2. Comparison operations
3. Logical conditions
4. Student marks classification
5. Printing numbers using loops
6. Printing even numbers
7. Printing even and odd numbers
8. Calculating a sum
9. Finding the largest number
10. Finding the smallest number
11. Finding both minimum and maximum
12. Calculating the sum of even numbers

---

## 🎯 Key Takeaway

> Programming is not only about syntax. The important part is understanding the logic and solving a problem step-by-step.

I practiced writing the logic myself instead of simply copying code.

---

## 📅 Progress

**Day 03 — Completed ✅**

### Learning Workflow

**Learn → Practice → Build → Explain → Document → GitHub**

Next: **Continue Python Fundamentals → NumPy/Pandas → SQL → Machine Learning → Deep Learning → Transformers → LLMs → GenAI → RAG → Vector Databases → LangChain → LangGraph → AI Agents → MCP → FastAPI → Docker → AWS → Projects**