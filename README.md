#MITOCW6.0001  fall 2016  Python-for-CS-MIT-OCW
Guttag, John. Introduction to Computation and Programming Using Python: With Application to Understanding Data, Second Edition. MIT Press, 2016 und Proff. Ana Bell MITOCW videos and lecture slides. 
Chapter 1- Getting started
# MIT OCW – Introduction to Python

## Chapter 1: Getting Started

> These notes are written for **beginner understanding** and **GitHub documentation**.

---

## 1. What Does a Computer Do?

A computer does **only two things**, but does them extremely well:

1. **Performs calculations**
2. **Remembers results (memory/storage)**

### Speed of Computation

* A modern computer can perform **billions of calculations per second**.
* Example: Before a ball dropped from 1 meter hits the ground, a computer may execute **over a billion instructions**.

### Memory Capacity

* Computers can store **hundreds of gigabytes (GB)** of data.
* 1 byte = typically **8 bits**, used to store one character.
* If 1 byte weighed 1 gram, then:

  * **100 GB ≈ 10,000 metric tons**
  * Roughly equal to **15,000 African elephants** 🐘

---

## 2. Why Computers Matter

* For most of human history:

  * Calculations were limited by **human brain speed**
  * Recording results depended on **hand writing**
* Only **small problems** could be solved computationally
* Today:

  * Many complex problems can be solved using computation
  * Some problems (e.g., **climate change**) are still extremely difficult

👉 Goal of this course: **Teach you to use computational thinking to solve problems in study, work, and daily life.**

---

## 3. Computational Thinking

All knowledge can be divided into **two types**:

### A. Declarative Knowledge ("What is true")

* Statements of fact
* Example:

  > "The square root of x is a number y such that y*y = x"
* ❌ Problem: Does **not** tell us *how* to find the square root

### B. Imperative Knowledge ("How to do")

* Step-by-step methods or recipes
* Tells us **how to compute something**

---

## 4. Algorithms

### Definition

An **algorithm** is:

* A **finite list of instructions**
* That describes a computation
* Proceeds through **well-defined steps**
* Produces an **output** from given inputs

📌 Algorithms are like **recipes** in cooking.

### Cooking Analogy

Example recipe logic:

1. Heat custard
2. Stir
3. Test with spoon
4. If done → stop
5. Else → repeat

➡ Includes:

* Order of steps
* Conditions (tests)
* Repetition (loops)

---

## 5. Example Algorithm: Finding Square Root (Heron’s Method)

Heron of Alexandria described an early algorithm to compute square roots.

### Problem

Find the square root of a number **x**

### Heron’s Algorithm (Guess-and-Check)

1. Start with a **guess (g)**
2. If **g × g** is close enough to **x**, stop
3. Else, update guess:

   g = (g + x/g) / 2
4. Repeat until accurate enough

---

## 6. Example: Square Root of 25

1. Initial guess: g = 3

   * 3 × 3 = 9 ❌ (not close)
2. New guess:

   g = (3 + 25/3) / 2 = 5.67

   * 5.67 × 5.67 = 32.15 ❌
3. New guess:

   g = (5.67 + 25/5.67) / 2 = 5.04

   * 5.04 × 5.04 ≈ 25.4 ✅ (close enough)

✔ Result: **Square root of 25 ≈ 5.04**

---

## 7. Guess-and-Check Algorithms

Characteristics:

* Easy to **verify correctness** of a guess
* Improve guesses step by step
* Stop when result is "good enough"

Used widely in:

* Numerical methods
* Optimization
* Machine learning

---

## 8. Key Takeaways

* Computers are powerful because of **speed + memory**
* Computational thinking = solving problems using **algorithms**
* Algorithms are:

  * Finite
  * Step-based
  * Logical
  * Repeatable
* Programming is about converting **imperative knowledge** into code

---

## 9. Important Term

**Algorithm**

* Word comes from Persian mathematician:
  **Muhammad ibn Musa al-Khwarizmi**

---

📌 *These notes are suitable for beginners and can be directly used in a GitHub repository.*
Date 18 March 2026
How a Computer Works (Based on My Notes)
1. Basic Idea

A computer executes a sequence of instructions stored in memory.

These instructions tell the computer:

what to do

in what order

on which data

2. Main Components of a Computer
🔹 1. Memory

Stores:

Data (numbers, inputs)

Instructions (program code)

Acts like a storage area

🔹 2. Arithmetic Logic Unit (ALU)

Performs operations such as:

Arithmetic → +, −, ×, ÷

Logic → comparisons (>, <, ==)

👉 Example:

Adding two numbers

Checking if a guess is correct

🔹 3. Control Unit

Directs the entire process

Decides:

which instruction to execute

when to execute

👉 It acts like a manager

3. Program Execution Process
Step-by-step flow:

Instruction stored in memory

Control unit reads instruction

Instruction sent to ALU

ALU performs operation

Result stored back in memory or output

4. Program Counter (Very Important)

Special component in control unit

Keeps track of:
👉 “Which instruction to execute next”

How it works:

Starts from first instruction

After execution → moves to next

Continues step-by-step

👉 This is why programs run in sequence

5. Types of Primitive Instructions

Computer understands only simple instructions:

Arithmetic operations

Logical comparisons

Moving data (load/store)

👉 Complex programs = combination of these simple steps

6. Stored Program Concept

A program is stored in memory

Executed step-by-step

👉 This means:

Computer doesn’t think—it just follows instructions

🔁 Connecting This to the Square Root (Guessing) Example

Now let’s connect this to your example:

Problem:

Find √16 using guessing

Step 1: Initial Guess

Let:

x = 16

guess = 3

Step 2: Check Guess

Computer does:

👉 guess × guess = 9

Compare with 16

Result → not correct

Step 3: Improve Guess

Use formula:

👉 new_guess = (guess + x/guess) / 2

This improves the approximation.

Step 4: Repeat (Loop)

Computer repeats:

Take guess

Calculate new guess

Check error

Continue until close enough

7. How Computer Executes This (Link to Diagram)

Let’s connect each step to components:

🔹 Memory

Stores:

x = 16

guess = 3

instructions (formula, loop)

🔹 Control Unit

Reads instruction:

“calculate guess × guess”

“compare with 16”

“update guess”

🔹 ALU

Performs:

multiplication → guess²

division → x/guess

addition → guess + (x/guess)

comparison

🔹 Program Counter

Controls flow:

Step 1 → initialize guess

Step 2 → compute square

Step 3 → check condition

Step 4 → update guess

Step 5 → repeat

8. Full Process (Combined View)

Program is stored in memory

Control unit fetches instruction

ALU performs calculation

Result stored

Program counter moves forward

Loop continues until condition satisfied

9. Key Insight

👉 Computer does NOT directly know √16 = 4

Instead:

It guesses

Improves guess step-by-step

Uses simple operations repeatedly

10. Why This Is Important

This concept teaches:

How programs execute step-by-step

How loops work

How approximation works

How logic + math combine

💻 Simple Python Version
x = 16
guess = 3

while abs(guess*guess - x) > 0.01:
    guess = (guess + x/guess) / 2

print(guess)
🔥 Final Understanding

👉 Your diagram is not just theory

It explains:

how Python runs

how algorithms work

how computers “think”

