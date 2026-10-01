# Day 12 – NumPy Array Operations

## 📌 Overview

This project is part of my **45-Day AI & ML Internship**.

The objective of Day 12 is to understand **NumPy arrays** and perform basic mathematical operations using **vectorized operations** in Python.

In this task, two NumPy arrays are created and the following operations are performed:

* Addition
* Subtraction
* Multiplication
* Division

The task also demonstrates the concept of **vectorization** and compares NumPy vectorized operations with a traditional Python loop.

---

## 🎯 Objectives

* Understand how to create NumPy arrays.
* Learn how to perform mathematical operations on NumPy arrays.
* Check the shape of NumPy arrays.
* Understand NumPy vectorization.
* Compare vectorized operations with traditional Python loops.
* Gain practical experience using NumPy in Jupyter Notebook.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Jupyter Notebook**

---

## 📊 Arrays Used

Two one-dimensional NumPy arrays were created:

```python
Array 1 = [10, 20, 30, 40, 50]
Array 2 = [2, 4, 5, 8, 10]
```

Both arrays contain **5 elements**.

Their shapes are:

```text
Array 1: (5,)
Array 2: (5,)
```

---

## ➕ Addition

The corresponding elements of both arrays are added.

```python
array1 + array2
```

### Result

```text
[12 24 35 48 60]
```

---

## ➖ Subtraction

The corresponding elements of the second array are subtracted from the first array.

```python
array1 - array2
```

### Result

```text
[ 8 16 25 32 40]
```

---

## ✖️ Multiplication

The corresponding elements of both arrays are multiplied.

```python
array1 * array2
```

### Result

```text
[ 20  80 150 320 500]
```

---

## ➗ Division

The corresponding elements of the first array are divided by the corresponding elements of the second array.

```python
array1 / array2
```

### Result

```text
[5. 5. 6. 5. 5.]
```

---

## ⚡ Vectorization

**Vectorization** allows mathematical operations to be performed on an entire NumPy array without explicitly writing a Python `for` loop.

For example:

```python
array1 + array2
```

automatically performs:

```text
10 + 2  = 12
20 + 4  = 24
30 + 5  = 35
40 + 8  = 48
50 + 10 = 60
```

This makes numerical operations concise and efficient.

---

## 🔄 Vectorization vs Python Loop

The same addition can also be performed using a traditional Python loop:

```python
result_loop = []

for i in range(len(array1)):
    result_loop.append(array1[i] + array2[i])
```

Using NumPy vectorization:

```python
result = array1 + array2
```

The NumPy approach allows the operation to be expressed directly on the arrays and is generally more efficient for numerical workloads.

---

## 📋 Operations Summary

| Operation      | NumPy Expression  | Result                |
| -------------- | ----------------- | --------------------- |
| Addition       | `array1 + array2` | `[12 24 35 48 60]`    |
| Subtraction    | `array1 - array2` | `[8 16 25 32 40]`     |
| Multiplication | `array1 * array2` | `[20 80 150 320 500]` |
| Division       | `array1 / array2` | `[5. 5. 6. 5. 5.]`    |

---

## 💻 Complete Code

```python
import numpy as np

# Create two NumPy arrays
array1 = np.array([10, 20, 30, 40, 50])
array2 = np.array([2, 4, 5, 8, 10])

# Display arrays
print("Array 1:", array1)
print("Array 2:", array2)

# Check shapes
print("\nShape of Array 1:", array1.shape)
print("Shape of Array 2:", array2.shape)

# Mathematical operations
addition = array1 + array2
subtraction = array1 - array2
multiplication = array1 * array2
division = array1 / array2

# Display results
print("\nAddition:", addition)
print("Subtraction:", subtraction)
print("Multiplication:", multiplication)
print("Division:", division)

# Vectorized operation
result = array1 + array2
print("\nVectorized Addition:", result)

# Comparison with Python loop
result_loop = []

for i in range(len(array1)):
    result_loop.append(array1[i] + array2[i])

print("\nUsing Python loop:", result_loop)
print("Using NumPy vectorization:", array1 + array2)
```

---

## 🎓 Interview Questions

### 1. What is NumPy?

NumPy is a Python library used for numerical computing. It provides multidimensional arrays and efficient mathematical operations.

### 2. What is vectorization?

Vectorization is the process of performing operations on an entire array without explicitly using Python loops.

### 3. What happens when two NumPy arrays are added?

Corresponding elements of the arrays are added.

Example:

```python
np.array([1, 2, 3]) + np.array([4, 5, 6])
```

Output:

```text
[5 7 9]
```

### 4. What is the shape of a one-dimensional NumPy array containing five elements?

```text
(5,)
```

### 5. Why is NumPy useful for numerical operations?

NumPy provides efficient array-based operations and optimized numerical routines, making it well suited for scientific computing, data analysis, and machine learning.

### 6. What happens if two NumPy arrays have incompatible shapes?

NumPy attempts to apply its **broadcasting rules**. If the shapes cannot be broadcast together, a `ValueError` is raised.

---

## 📁 Project Structure

```text
Day-12-NumPy-Array-Operations/
│
├── Day-12-NumPy-Array-Operations.ipynb
└── README.md
```

---

## 📚 Learning Outcomes

After completing this task, I learned how to:

* Import NumPy in Python.
* Create NumPy arrays using `np.array()`.
* Check array shapes using `.shape`.
* Perform addition, subtraction, multiplication, and division.
* Understand vectorized operations.
* Compare NumPy operations with Python loops.
* Use Jupyter Notebook for numerical computing.

---

## ✅ Conclusion

This task provided practical experience with **NumPy array operations and vectorization**. Two numerical arrays were created and used to perform basic mathematical operations. The task also demonstrated how NumPy allows operations to be applied directly to arrays, providing a convenient approach for numerical computation.

---

## 👨‍💻 Author

**Divakar R**
B.E. Electronics and Communication Engineering
Adithya Institute of Technology, Coimbatore

**AI & ML Internship – Day 12 of 45**
