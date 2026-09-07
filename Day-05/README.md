# Day 05 — NumPy Fundamentals

## 🎯 Goal

Learn the basics of NumPy and understand how NumPy arrays are used for numerical operations and data handling in AI and Machine Learning.

---

# 1. What is NumPy?

NumPy stands for **Numerical Python**.

It is a Python library used for working with:

- Numerical data
- Arrays
- Matrices
- Mathematical operations

NumPy is very important for AI and Machine Learning because ML involves working with large amounts of numerical data.

---

# 2. Creating a NumPy Array

First, import NumPy:

    import numpy as np

Create an array:

    numbers = np.array([10, 20, 30, 40])

Print the array:

    print(numbers)

Output:

    [10 20 30 40]

A NumPy array is different from a normal Python list and is designed for efficient numerical operations.

---

# 3. Element-wise Operations

One important feature of NumPy arrays is that mathematical operations can be performed on every element.

Example:

    numbers = np.array([10, 20, 30, 40])

    print(numbers + 10)

Output:

    [20 30 40 50]

NumPy adds `10` to every element.

Other examples:

    numbers = np.array([10, 20, 30, 40])

    print(numbers * 2)
    print(numbers - 5)
    print(numbers / 10)

Output:

    [20 40 60 80]
    [ 5 15 25 35]
    [1. 2. 3. 4.]

This is called an **element-wise operation**.

---

# 4. NumPy Indexing

NumPy array indexing works similarly to Python lists.

Example:

    numbers = np.array([10, 20, 30, 40, 50])

    print(numbers[0])
    print(numbers[-1])
    print(numbers[1:4])

Output:

    10
    50
    [20 30 40]

Important:

- `numbers[0]` → first element
- `numbers[-1]` → last element
- `numbers[1:4]` → elements from index 1 up to, but not including, index 4

---

# 5. Shape of an Array

The `shape` property tells us the size of each dimension of an array.

Example:

    numbers = np.array([10, 20, 30, 40, 50])

    print(numbers.shape)

Output:

    (5,)

This is a one-dimensional array containing 5 elements.

---

# 6. Number of Dimensions

The `ndim` property tells us the number of dimensions in an array.

Example:

    numbers = np.array([10, 20, 30, 40, 50])

    print(numbers.ndim)

Output:

    1

Therefore:

    shape → (5,)
    ndim  → 1

---

# 7. Two-Dimensional NumPy Arrays

A 2D array can be represented like a matrix.

Example:

    matrix = np.array([
        [1, 2, 3],
        [4, 5, 6]
    ])

This matrix has:

- 2 rows
- 3 columns

Therefore:

    print(matrix.shape)

Output:

    (2, 3)

And:

    print(matrix.ndim)

Output:

    2

Important:

    shape = (rows, columns)

So:

    (2, 3)

means:

    2 rows × 3 columns

---

# 8. 2D Array Indexing

Consider:

    matrix = np.array([
        [1, 2, 3],
        [4, 5, 6]
    ])

The indexes are:

            0  1  2
           ---------
    row 0  [1  2  3]
    row 1  [4  5  6]

Access the first row:

    print(matrix[0])

Output:

    [1 2 3]

Access the value at row 1, column 2:

    print(matrix[1][2])

Output:

    6

Remember that indexing starts from `0`.

---

# 9. 2D Array Slicing

Example:

    print(matrix[0:2, 1:3])

The first part selects rows:

    0:2

The second part selects columns:

    1:3

The result is:

    [[2 3]
     [5 6]]

Important slicing rule:

    start:end

means:

    start is included
    end is excluded

---

# 10. Selecting a Column

The `:` means all rows.

Example:

    print(matrix[:, 1])

This selects column index `1` from every row.

Output:

    [2 5]

So:

    matrix[:, 1]

means:

    all rows
    column 1

---

# 11. NumPy Mathematical Operations

NumPy provides useful functions for numerical data.

Example:

    numbers = np.array([10, 20, 30, 40, 50])

    print(numbers.sum())
    print(numbers.mean())
    print(numbers.max())
    print(numbers.min())

Output:

    150
    30.0
    50
    10

## sum()

Returns the total:

    numbers.sum()

Output:

    150

## mean()

Returns the average:

    numbers.mean()

Output:

    30.0

## max()

Returns the largest value:

    numbers.max()

Output:

    50

## min()

Returns the smallest value:

    numbers.min()

Output:

    10

---

# 12. Practical Task Completed

I created a NumPy array and performed different operations on it.

    import numpy as np

    number = np.array([10, 20, 30, 40, 50])

    print(number.sum())
    print(number.mean())
    print(number.max())
    print(number.min())
    print(number * 2)

Output:

    150
    30.0
    50
    10
    [20 40 60 80 100]

---

# 🧪 Practice Completed

During Day 05, I practiced:

- Creating NumPy arrays
- Importing NumPy
- Element-wise addition
- Element-wise subtraction
- Element-wise multiplication
- Element-wise division
- Array indexing
- Array slicing
- Understanding `shape`
- Understanding `ndim`
- Creating 2D arrays
- 2D array indexing
- 2D array slicing
- Selecting rows and columns
- Calculating sum
- Calculating mean
- Finding maximum
- Finding minimum

---

# 🧠 Important Concepts

## NumPy Array

A NumPy array is a data structure designed for efficient numerical operations.

## Element-wise Operation

An operation is performed separately on each element of the array.

Example:

    [10 20 30] + 10

Result:

    [20 30 40]

## Shape

Tells us the size of each dimension.

Example:

    (2, 3)

means:

    2 rows × 3 columns

## ndim

Tells us the number of dimensions.

Example:

    ndim = 2

means the array is two-dimensional.

---

# 🎯 Key Takeaways

Today I learned that NumPy is an important Python library for numerical computing.

The most important concepts I learned are:

    np.array()
    element-wise operations
    indexing
    slicing
    shape
    ndim
    sum()
    mean()
    max()
    min()

I also learned how to work with both one-dimensional and two-dimensional arrays.

---

# 💡 Why NumPy Matters for AI

AI and Machine Learning involve a lot of numerical data.

NumPy provides efficient ways to:

- Store numerical data
- Perform mathematical operations
- Work with vectors
- Work with matrices
- Process arrays

These concepts will be useful later when learning:

    Pandas
    Machine Learning
    Linear Algebra
    Neural Networks
    Deep Learning

---

# ✅ Day 05 Completed

Learn → Practice → Build → Explain → Document → GitHub