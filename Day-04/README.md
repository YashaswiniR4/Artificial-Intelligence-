# Day 04 — Python Data Structures & Strings

## 🎯 Goal

Learn the fundamental Python data structures and strings:

- Strings
- Tuples
- Sets
- Dictionaries
- Loops with dictionaries
- Combining multiple data structures

---

# 1. Strings

A string is a sequence of characters.

Example:

    name = "Yashaswini"

## Indexing

Each character has an index starting from `0`.

    name = "Yashaswini"

    print(name[0])    # Y
    print(name[1])    # a
    print(name[-1])   # i

Positive indexing starts from the beginning, while negative indexing starts from the end.

## Slicing

Slicing extracts a part of a string.

    name = "Yashaswini"

    print(name[0:4])

Output:

    Yash

The ending index is not included.

## Slicing with Step

    name[0:10:2]

Output:

    Ysawn

The third value specifies the step.

## Reverse a String

    name[::-1]

Output:

    iniwsahsaY

---

# 2. String Methods

## upper()

Converts all characters to uppercase.

    name = "yashaswini"
    print(name.upper())

Output:

    YASHASWINI

## lower()

Converts all characters to lowercase.

    print(name.lower())

## capitalize()

Capitalizes the first character.

    print(name.capitalize())

Output:

    Yashaswini

## replace()

Replaces part of a string.

    name = "yashaswini"
    print(name.replace("y", "Y"))

Output:

    Yashaswini

## strip()

Removes spaces from the beginning and end.

    name = "   Yashaswini   "
    print(name.strip())

Output:

    Yashaswini

## startswith()

Checks whether a string starts with specific characters.

    name = "Yashaswini"
    print(name.startswith("Y"))

Output:

    True

## endswith()

Checks whether a string ends with specific characters.

    print(name.endswith("i"))

Output:

    True

## in

Checks whether some text exists inside a string.

    print("sha" in name)

Output:

    True

## len()

Returns the total number of characters.

    name = "Yashaswini"
    print(len(name))

Output:

    10

Important:

    Last index = 9
    Length = 10

## count()

Counts how many times a character or substring appears.

    print(name.count("a"))
    print(name.count("i"))

Output:

    2
    2

---

# 3. Tuples

A tuple is an ordered collection of values that cannot be changed after creation.

Example:

    student = ("Yashaswini", 21, "AI")

## Accessing Tuple Elements

    print(student[0])
    print(student[1])

Output:

    Yashaswini
    21

## Negative Indexing

    print(student[-1])

Output:

    AI

## Tuple Length

    print(len(student))

Output:

    3

## Tuple Slicing

    student[0:2]

Output:

    ("Yashaswini", 21)

    student[-2:]

Output:

    (21, "AI")

Other examples:

    student[1:]

Output:

    (21, "AI")

    student[:2]

Output:

    ("Yashaswini", 21)

## Important

Tuples are immutable.

This will produce an error:

    student[0] = "Anu"

Difference:

    List  → changeable
    Tuple → fixed

---

# 4. Sets

A set is a collection of unique values.

Duplicates are automatically removed.

Example:

    numbers = {10, 20, 30, 20, 10, 40}

The set contains:

    {10, 20, 30, 40}

Length:

    len(numbers)

Output:

    4

## Important

Sets are unordered, so we should not depend on the order in which elements are printed.

## add()

Adds an element to a set.

    numbers = {10, 20, 30}

    numbers.add(40)
    numbers.add(20)

Since `20` already exists, it is not added again.

Final set:

    {10, 20, 30, 40}

## remove()

Removes an element.

    numbers = {10, 20, 30, 40}

    numbers.remove(20)

Final set:

    {10, 30, 40}

---

# 5. Dictionaries

A dictionary stores data using key-value pairs.

Example:

    student = {
        "name": "Yashaswini",
        "age": 21,
        "course": "AI"
    }

Think of it as:

    name   → Yashaswini
    age    → 21
    course → AI

## Accessing Values

    print(student["name"])
    print(student["age"])

Output:

    Yashaswini
    21

## Adding a New Key-Value Pair

    student["course"] = "AI"

## Updating a Value

    student["age"] = 22

If the key already exists, its value is updated.

## Removing a Key-Value Pair

    student.pop("age")

This removes the `age` key and its value.

---

# 6. Dictionary keys() and values()

## keys()

Returns all keys.

    print(student.keys())

Example output:

    dict_keys(['name', 'age', 'course'])

## values()

Returns all values.

    print(student.values())

Example output:

    dict_values(['Yashaswini', 22, 'AI'])

---

# 7. Dictionary Loops

When directly looping through a dictionary, we get the keys.

    student = {
        "name": "Yashaswini",
        "age": 23,
        "course": "AI"
    }

    for key in student:
        print(key)

Output:

    name
    age
    course

## Loop Through Values

    for value in student.values():
        print(value)

Output:

    Yashaswini
    23
    AI

## Loop Through Keys and Values

The `items()` method gives both key and value.

    for key, value in student.items():
        print(key, value)

Output:

    name Yashaswini
    age 23
    course AI

---

# 8. Combining Data Structures

We can use lists, dictionaries, sets, and loops together.

Example:

    students = [
        {"name": "Yashaswini", "course": "AI"},
        {"name": "Rahul", "course": "Java"},
        {"name": "Anu", "course": "AI"}
    ]

    courses = set()

    for student in students:
        courses.add(student["course"])

    print(courses)
    print(len(courses))

The set contains only unique courses:

    AI
    Java

Length:

    2

This example combines:

    List       → stores multiple students
    Dictionary → stores each student's information
    Loop       → processes each student
    Set        → stores unique courses

---

# 🧪 Practice Completed

During Day 04, I practiced:

- String indexing
- String slicing
- String reversal
- String methods
- Finding string length
- Counting characters
- Tuple indexing
- Tuple slicing
- Understanding immutable tuples
- Creating sets
- Removing duplicate values
- Adding and removing set elements
- Creating dictionaries
- Accessing dictionary values
- Adding and updating dictionary values
- Removing dictionary values
- Using `keys()`, `values()`, and `items()`
- Looping through dictionaries
- Combining lists, dictionaries, sets, and loops

---

# 🧠 Key Takeaways

### String

A sequence of characters.

### List

Ordered and changeable collection.

### Tuple

Ordered but immutable collection.

### Set

Collection of unique values.

### Dictionary

Stores data as key-value pairs.

---

# 🎯 Day 04 Final Learning

Today I learned how Python data structures work and how they can be combined.

The most important concepts I learned are:

    List  → Ordered + Changeable
    Tuple → Ordered + Fixed
    Set   → Unique Values
    Dict  → Key → Value

I also learned that choosing the correct data structure depends on the type of data and the operation I need to perform.

---

# 💡 Final Takeaway

Python data structures are the foundation for working with data in AI and Machine Learning.

Before moving into NumPy, Pandas, Machine Learning, and AI projects, I need to be comfortable working with:

    Strings
    Lists
    Tuples
    Sets
    Dictionaries
    Loops

## ✅ Day 04 Completed

Learn → Practice → Build → Explain → Document → GitHub