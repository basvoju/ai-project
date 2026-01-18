# Practice Sheet — Python Basics + Data Structures + OOP (30 Programs)

Use this sheet for in-class practice. Students should write clean code, test with multiple inputs, and be ready to explain their approach.

## Ground rules
- Don’t use external libraries unless a problem explicitly allows it.
- Prefer writing small helper functions.
- Handle edge cases (empty input, negative numbers, duplicates, etc.).
- For each problem: write **inputs**, **process**, **outputs** clearly.

---

## A) Warm-up (Data types + conditionals) — Programs 1–6

### Program 1 (Easy): Type inspector
Write a program that takes 5 variables (you choose values) and prints each value with its `type`.

### Program 2 (Easy): Even or odd
Input an integer and print whether it is even or odd.

### Program 3 (Easy): Absolute difference
Input two integers `a` and `b`. Print `abs(a - b)` **without** using `abs()`.

### Program 4 (Easy): Largest of three
Input three numbers and print the largest.

### Program 5 (Easy): Leap year checker
Input a year. Print whether it is a leap year.
- Leap year rule: divisible by 4, except divisible by 100 unless also divisible by 400.

### Program 6 (Medium): Simple calculator
Input two numbers and an operator (`+ - * / // % **`). Perform the operation and print the result.
- Handle division by zero gracefully.

---

## B) Loops — Programs 7–12

### Program 7 (Easy): Sum of first N numbers
Input `n`. Print `1 + 2 + ... + n`.

### Program 8 (Easy): Factorial
Input `n`. Print `n!` using a loop (no recursion).

### Program 9 (Medium): Prime checker
Input `n`. Print whether `n` is prime.
- Constraint: do it efficiently (check up to `sqrt(n)`).

### Program 10 (Medium): Print primes in a range
Input two integers `L` and `R`. Print all prime numbers between them (inclusive).

### Program 11 (Medium): Fibonacci series
Input `n`. Print the first `n` Fibonacci numbers.

### Program 12 (Medium): Count digits
Input an integer `n` (can be negative). Count how many digits it has.
- Example: `-1205` has 4 digits.

---

## C) Strings — Programs 13–17

### Program 13 (Easy): Reverse a string
Input a string and print it reversed (use slicing or a loop).

### Program 14 (Easy): Vowel and consonant count
Input a string. Count vowels and consonants (ignore spaces and punctuation).

### Program 15 (Medium): Palindrome check
Input a string and check if it’s a palindrome.
- Ignore spaces and case.
- Example: `"Never odd or even"` → palindrome.

### Program 16 (Medium): Character frequency
Input a string and build a dictionary of character counts (ignore spaces).
- Output format suggestion: print the dict.

### Program 17 (Medium): Longest word
Input a sentence. Print the longest word and its length.
- If tie, print the first occurring longest word.

---

## D) Lists + Tuples — Programs 18–22

### Program 18 (Easy): Remove duplicates (preserve order)
Input a list of integers (hardcode or take input). Output a new list with duplicates removed, preserving first occurrences.
- Example: `[1,2,2,3,1]` → `[1,2,3]`

### Program 19 (Easy): Second largest number
Given a list of integers, find the second largest **distinct** number.
- Handle cases where it doesn’t exist.

### Program 20 (Medium): Rotate list
Given a list and integer `k`, rotate the list to the right by `k`.
- Example: `[1,2,3,4,5]`, `k=2` → `[4,5,1,2,3]`

### Program 21 (Medium): Pair sum
Given a list and a target `T`, find if any two numbers sum to `T`.
- Print the pair if found, else print “Not found”.
- Bonus: do it in O(n) using a set.

### Program 22 (Medium): Tuple unpacking practice
Given a list of tuples `[(name, marks), ...]`, print names of students scoring >= 90.
- Example: `[("A", 91), ("B", 88)]` → `A`

---

## E) Sets — Programs 23–24

### Program 23 (Easy): Common elements
Given two lists, print the common unique elements using sets.

### Program 24 (Medium): Unique words across sentences
Input two sentences. Print the set of unique words across both (case-insensitive).
- Example: `"AI is fun"`, `"AI is powerful"` → `{"ai","is","fun","powerful"}`

---

## F) Dictionaries — Programs 25–27

### Program 25 (Easy): Word frequency
Input a sentence. Print a dictionary of word counts.
- Normalize case and remove extra spaces.

### Program 26 (Medium): Invert a dictionary (values become keys)
Given a dict like `{"a": 1, "b": 2}`, invert it into `{1: "a", 2: "b"}`.
- Assume values are unique.

### Program 27 (Medium): Student gradebook
Maintain a gradebook dict of `{name: [marks...]}`.
Implement functions:
- `add_mark(name, mark)`
- `average(name)`
- `topper()` returns name with highest average

---

## G) Functions + error handling — Programs 28–29

### Program 28 (Medium): Safe integer parser
Write a function `safe_int(s, default=0)` that:
- returns `int(s)` if possible
- otherwise returns `default`
Test it on values like `"12"`, `" 7 "`, `"3.5"`, `"abc"`.

### Program 29 (Medium): Mini stats
Write functions `mean(nums)`, `median(nums)`, `mode(nums)` for a list of integers.
- Do not use statistics module.
- For mode: if multiple modes, return all of them (as a list).

---

## H) OOP — Programs 30–30

### Program 30 (Medium/Hard): Bank account system (OOP)
Design a `BankAccount` class with:
- attributes: `name`, `_balance`
- methods: `deposit(amount)`, `withdraw(amount)`, `get_balance()`
- validation: no negative deposits, no overdraft

Then add:
- a `SavingsAccount(BankAccount)` that adds an `interest_rate` and method `apply_interest()`
- `__repr__` so objects print nicely
- a small demo that creates 2 accounts and performs operations

---

## Optional extension problems (if time permits)
- Build a `TodoList` class that supports `add_task`, `complete_task`, `pending_tasks`.
- Build a `Library` system with `Book`, `Member`, and `Library` using composition.

