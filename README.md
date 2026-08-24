# 🔍 Contains Duplicate

## 📌 Problem Description

Given an array of integers, determine whether the array contains any duplicate values.

Return:

* `True` if any value appears more than once.
* `False` if every value appears only once.

This problem demonstrates the use of a **Hash Set** for efficient duplicate detection.

---

## 💡 Example

### Input

```text
1 2 3 1
```

### Output

```text
Array contains duplicate values
```

### Explanation

The number `1` appears more than once, so the array contains a duplicate.

---

## 🛠️ Technology Used

* Python 3
* Lists
* Sets
* Functions
* Hashing
* Algorithm Optimization

---

## 💻 Source Code

```python
# Contains Duplicate
# Check whether an array contains any duplicate values.

def contains_duplicate(nums):
    seen = set()

    for num in nums:
        if num in seen:
            return True

        seen.add(num)

    return False


nums = list(map(int, input("Enter numbers: ").split()))

if contains_duplicate(nums):
    print("Array contains duplicate values")
else:
    print("Array does not contain duplicate values")
```

---

## ▶️ How to Run

Save the program as:

```text
contains_duplicate.py
```

Run it using:

```bash
python contains_duplicate.py
```

---

## 📥 Sample Input

```text
Enter numbers: 1 2 3 1
```

## 📤 Sample Output

```text
Array contains duplicate values
```

---

## 📥 Sample Input 2

```text
Enter numbers: 1 2 3 4
```

## 📤 Sample Output 2

```text
Array does not contain duplicate values
```

---

## 🧠 Approach

The solution uses a **set** called `seen`.

### Algorithm

1. Create an empty set.
2. Traverse each number in the array.
3. Check whether the number already exists in the set.
4. If it exists, a duplicate has been found.
5. Otherwise, add the number to the set.
6. If the complete array is processed without finding a duplicate, return `False`.

---

## ⚡ Why Use a Set?

A simple nested-loop solution would compare every pair of elements and require:

```text
O(n²)
```

Using a set allows duplicate checking in approximately:

```text
O(1)
```

for each lookup.

Therefore, the complete solution runs in:

```text
O(n)
```

---

## ⏱️ Complexity Analysis

| Complexity       | Value  |
| ---------------- | ------ |
| Time Complexity  | `O(n)` |
| Space Complexity | `O(n)` |

Where `n` represents the number of elements in the array.

---

## 📂 Project Structure

```text
Python-DSA-Coding-Journey/
│
├── Arrays/
│   ├── two_sum.py
│   ├── best_time_to_buy_sell_stock.py
│   └── contains_duplicate.py
│
├── Basics/
│   ├── prime_number.py
│   ├── factorial.py
│   ├── fibonacci.py
│   ├── palindrome.py
│   ├── reverse_number.py
│   ├── armstrong_number.py
│   ├── sum_of_digits.py
│   ├── even_odd.py
│   └── largest_of_three.py
│
├── Strings/
├── LinkedList/
├── Stack/
├── Queue/
├── Trees/
├── Graphs/
├── Backtracking/
└── DynamicProgramming/
```

---

## 🎯 Learning Objectives

This problem helps develop:

* Array processing
* Set data structures
* Hashing concepts
* Efficient searching
* Algorithm optimization
* Time and space complexity analysis
* Technical interview skills

---

## 👩‍💻 Author

**Yogasrii Deenathayalan**

M.Sc. Computer Science

Interested in:

* Python
* Data Structures & Algorithms
* Artificial Intelligence
* Machine Learning
* Deep Learning

---

⭐ **If you find this solution useful, consider starring the repository!**
