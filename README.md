<div align="center">

# 🌸 Rue Learns Python 🌸



![Python](https://img.shields.io/badge/Python-3.x-ffb6c1?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-f7c6d9?style=for-the-badge&logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-dcc6f7?style=for-the-badge&logo=pandas&logoColor=white)


</div>

---

## Overview

The notebook is a series of short, self-contained cells. Each one introduces a single concept with a minimal working example. The material moves from syntax and data types through control flow and data structures, then to file input/output, and finally to tabular analysis with pandas. It is, in effect, a lab notebook. The experiments are small, the results are reproducible, and the occasional comment was clearly written late at night.

## Contents

### 1. Python Foundations
- Program output, indentation and comments
- Numeric types (`int`, `float`, `complex`) and explicit type conversion
- String operations: length, slicing, case conversion, replacement, concatenation and formatting
- Arithmetic operators: addition, subtraction, multiplication, division and exponentiation

### 2. Data Structures
- **Lists:** slicing, step and negative indexing, and modification with `append`, `insert`, `remove`, `pop` and `clear`
- **Tuples:** construction, immutability, and the single-element tuple, whose trailing comma separates a tuple from a string in parentheses
- **Sets:** uniqueness, iteration, and the `add`, `update` and `pop` methods. Duplicate pineapples are quietly discarded.
- **Dictionaries:** key–value access, `keys()` and `values()` views, `update`, `pop`, `popitem`, `del` and `copy`

### 3. Control Flow
- Conditional statements: `if`, `elif`, `else`, conditional expressions and nested conditions
- Logical operators: `and`, `or`
- Iteration with `for` and `while` loops, `range()`, nested loops and the often-overlooked loop `else` clause
- Loop control with `break`, `continue` and `pass`, which is Python's way of saying "nothing to see here"

### 4. Applied Exercises
- Sum of two user-supplied numbers
- Euclidean distance between two points
- Parity checks for integers and string lengths
- Variable swapping with a temporary variable
- Factorial computation (12! = 479,001,600, which escalates quickly)
- Sum of the first *n* natural numbers
- Linear search with `while`–`else`
- Grade classification

### 5. File Handling
- Opening, reading, partially reading and appending to text files
- Reading individual lines with `readline()`

The sample text file is a candid record of the author's state of mind at the time, preserved for scientific accuracy.

### 6. Data Analysis with pandas
Analysis of `DSA1080_Pandas_Student_Data.csv`, a dataset of 40 student records with the attributes `StudentID`, `Name`, `Course`, `Age`, `Score`, `Attendance`, `StudyHours` and `City`.

- **Inspection:** `head()`, `shape`, `info()`, `describe()` and missing-value counts
- **Selection:** column selection, label-based indexing (`loc`) and positional indexing (`iloc`)
- **Filtering:** single and compound boolean conditions, such as students scoring above 70 *and* studying at least 10 hours
- **Sorting:** ranking students by score
- **Feature engineering:** a derived `Total` column
- **Data cleaning:** median imputation for missing scores, placeholder imputation for missing cities, duplicate detection and range validation
- **Descriptive statistics:** mean, median, standard deviation, minimum, maximum and frequency distributions

## Key Findings

After cleaning, the dataset had the following properties:

| Metric | Value |
|:--|--:|
| Records | 40 |
| Courses represented | 4 |
| Mean score | 70.4 |
| Median score | 70.0 |
| Standard deviation | 15.11 |
| Score range | 44 – 97 |

Students were split evenly across the four courses (IT, Business Analytics, Computer Science and Data Science), with 10 in each, which is suspiciously tidy for real-world data. Three missing `Score` values were imputed with the median, and two students whose city went unrecorded were assigned to `Unknown`. No duplicate records were found.

## Requirements

- Python 3.x
- Jupyter Notebook
- pandas

```bash
pip install notebook pandas
```

## Usage

```bash
git clone https://github.com/<username>/<repository>.git
cd <repository>
jupyter notebook work.ipynb
```

**Notes:**
- Several cells use `input()` and will wait patiently for you to type something.
- The file-handling section expects a `file.txt` in the working directory.
- The pandas section expects `DSA1080_Pandas_Student_Data.csv` in the working directory.

## Author

**Ruvarashe Jo-Ann Mandima**

> `"RUE IS COOL".lower()` returns `'rue is cool'`. The value is unchanged. Only the volume is lower.
