# Python-Interview-Questions-
# 🐍 Python Interview Questions

A collection of frequently asked Python interview questions with brief answers and examples. Great for beginners and intermediate developers preparing for interviews.

---

## 📘 Questions & Answers

### 1. What is the difference between List and Tuple in Python?
- **List**: Mutable, uses `[]`, slower, more flexible.
- **Tuple**: Immutable, uses `()`, faster, safer.

---

### 2. How do sets help in removing duplicates?
Using `set(list)` removes duplicates because sets only store unique values.

```python
my_list = [1, 2, 2, 3]
unique = list(set(my_list))  # [1, 2, 3]

---

### 3. Why are dictionaries faster than lists for lookups?

- **Dictionaries** use **hashing** to store keys, which allows fast O(1) average lookup time.
- **Lists** use **sequential search**, which takes O(n) time in the worst case.



