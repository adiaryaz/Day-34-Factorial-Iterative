# Day-34-Factorial-Iterative

Day 34/100 - Python Program to Find the Factorial of a Number Without Recursion

# Find the Factorial of a Number (Iterative)

A program to compute the mathematical factorial of a given integer utilizing a straightforward iterative loop instead of recursion.

## 📝 Description

This program calculates the **factorial** of a user-inputted number. In mathematics, the factorial of a non-negative integer $n$, denoted by $n!$, is the product of all positive integers less than or equal to $n$.

Unlike the recursive method which consumes stack memory by calling itself, this script uses an **iterative approach**. It sets an initial `factorial` variable to `1` and uses a `for` loop paired with Python's `range()` function to iterate from 1 up to the inputted number. In each step, it multiplies the running total by the current loop iterator (`i`), effectively building the factorial product step-by-step from the bottom up.

---

## 🎯 Problem Statement

### Input:

* **Input 1:** A single integer value representing the number to be processed.

### Output:

* A formatted string stating: "The factorial of [num] is: [factorial]"

### Rules:

1. The program must accept an integer input from the user.
2. The program must declare a variable (e.g., `factorial`) and initialize it to `1` (since multiplying by 0 would clear the entire result).
3. The program must use a `for` loop iterating from `1` to `num + 1` (inclusive of the target number).
4. Inside the loop, multiply the current `factorial` value by the iterator `i` (`factorial *= i`).
5. Print the final calculated product after the loop completes.

---

## 💡 Examples

### Example 1 (Standard Factorial)

**Input:**

```
5


```

**Output:**

```
The factorial of 5 is: 120


```

**Explanation:** The loop iterates from 1 to 5.

* `i = 1`: `factorial` becomes $1 \times 1 = 1$
* `i = 2`: `factorial` becomes $1 \times 2 = 2$
* `i = 3`: `factorial` becomes $2 \times 3 = 6$
* `i = 4`: `factorial` becomes $6 \times 4 = 24$
* `i = 5`: `factorial` becomes $24 \times 5 = 120$

### Example 2 (The Zero Factorial)

**Input:**

```
0


```

**Output:**

```
The factorial of 0 is: 1


```

**Explanation:** Mathematically, $0! = 1$. In the code, the loop `range(1, 1)` is empty and does not execute. The program simply prints the initial value of the `factorial` variable, which is naturally set to 1.

### Example 3 (Larger Number)

**Input:**

```
7


```

**Output:**

```
The factorial of 7 is: 5040


```

**Explanation:** The program efficiently calculates $1 \times 2 \times 3 \times 4 \times 5 \times 6 \times 7 = 5040$ without adding overhead to the call stack.

### Example 4 (Edge Case limitation: Negative Numbers)

**Input:**

```
-3


```

**Output:**

```
The factorial of -3 is: 1


```

**Explanation:** *Note on current implementation:* Factorials are undefined for negative numbers. Because the provided script lacks an explicit negative-number check (like an `if num < 0:` statement), the `range(1, -2)` evaluates as empty. The loop is skipped, and it returns the default `1`.

---

## 🚀 How to Use

1. **Clone this repository** (or save the script)

```bash
git clone https://github.com/adiaryaz/Day-34-Factorial-Iterative.git
cd factorial-iterative


```

2. **Run the program**:

```bash
python main.py


```

Enter a non-negative integer when prompted to calculate its mathematical factorial iteratively.
