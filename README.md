# 🚀 SmartArray OOP Project<br>
 📖 Overview

This project demonstrates key **Object-Oriented Programming (OOP)** concepts using a custom **SmartArray** class built on top of NumPy's `ndarray`.

The project extends NumPy arrays with additional functionality while showcasing **Inheritance** and **Polymorphism**.

---

## 📂 Project Structure

```text
Project/
│
├── smart_array_base.py
└── polymorphism_mixin.py
```

---

## 🔹 smart_array_base.py

### Purpose

Defines the `SmartArray` class that inherits from `numpy.ndarray`.

### OOP Concept: Inheritance

* SmartArray is a child class of `numpy.ndarray`
* Inherits built-in NumPy attributes and methods
* Uses `__new__()` for object creation
* Uses `__array_finalize__()` for NumPy subclass compatibility

### Features

✅ Custom NumPy subclass
✅ Automatic access to ndarray methods
✅ Reusable base class

---

## 🔹 polymorphism_mixin.py

### Purpose

Adds additional functionality to `SmartArray`.

### OOP Concept: Polymorphism

* Overrides the `__str__()` method
* Provides custom display output
* Adds `is_symmetric()` method for matrix validation

### Features

✅ Method Overriding
✅ Custom String Representation
✅ Symmetric Matrix Check

---

## ✨ Example Usage

```python
from smart_array_base import SmartArray

arr = SmartArray([[1, 2],
                  [2, 1]])

print(arr)
```

### Output

```text
SmartArray(shape=(2, 2), dtype=int64)
[[1 2]
 [2 1]]
```

---

## 🛠 Requirements

Install NumPy before running the project:

```bash
pip install numpy
```

---

## 🎯 OOP Concepts Demonstrated

| Concept           | Description                            |
| ----------------- | -------------------------------------- |
| Inheritance       | SmartArray inherits from NumPy ndarray |
| Polymorphism      | Custom implementation of **str**()     |
| Method Overriding | Replaces default ndarray behavior      |
| Code Reusability  | Uses existing NumPy functionality      |

---

## 📌 Conclusion

This project demonstrates how NumPy arrays can be extended using OOP principles to create more powerful and user-friendly data structures while maintaining compatibility with the original NumPy framework.
