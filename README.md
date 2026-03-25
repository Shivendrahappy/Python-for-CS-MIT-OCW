#MITOCW6.0001  fall 2016  Python-for-CS-MIT-OCW 6.00001 Fall 2015,
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
Date 20 march 2026
1. What is a Python Program?

👉 A program is simply:

A set of instructions written to make the computer do something.

Example:
x=5
y=6
print(x+y)
...11

This is a Python program (even 1 line counts).

🔹 Think like this:

You → give instructions

Computer → follows them step by step

🧾 2. What are Commands?

👉 A command is a single instruction inside a program.

Example:
x=5
y=6
print(x+y)


Each line = a command

🔹 Types of commands:

Output → print()

Assignment → x = 5

Calculation → x + 2

🧠 3. What is an Interpreter?

This is the MOST IMPORTANT concept.

👉 Python uses an interpreter, not a compiler.

Definition:

Interpreter = program that reads your code and executes it line-by-line.

How it works:

You write:

print(5 + 2)

Interpreter does:

Reads line

Understands it

Executes it

Shows result

👉 Output:

7
🔥 Key point:

If there is an error:

Interpreter stops immediately

Shows error
21 March 2026
🖥️ 4. What is a Shell?

👉 Shell = place where you directly talk to Python

Also called:

Python shell
Interactive mode
Example:

You open Python and type:

 5 + 3

👉 Output:

8
🔹 Why called “interactive”?

Because:

You type → get instant answer
No need to save file
🧾 5. Difference: Shell vs Program File
Shell (Interactive)
One line at a time
Immediate result
Good for testing
Program File (.py)
Many lines
Saved as file
Run all together

Example file:

x = 5
y = 10
print(x + y)
⚙️ 6. Full Flow (VERY IMPORTANT)

This is what you asked: how everything works together

Step 1: You write code

In:

Notepad / VS Code / IDLE
Step 2: Python Interpreter runs it

Command:

python file.py
Step 3: Interpreter reads line-by-line
Step 4: Output is shown
🔄 Example Flow

You write:

x = 3
y = 4
print(x + y)
Internally:
x = 3 → stored
y = 4 → stored
print(x+y) → calculates → prints 7
🎯 Real-life analogy (important)
Concept	Real life
Program	Recipe
Command	Step in recipe
Interpreter	Chef
Shell	Talking directly to chef
Output	Final dish


 remember:

👉 Program = instructions
👉 Commands = steps
👉 Interpreter = executor
👉 Shell = direct interactio

DATE 23 MARCH 2026

(Scalar Objects — full meaning)
🔴 Core idea:

Scalar objects = simple values (cannot be broken further)

🔹 Types from your slide
1️⃣ int (integers)
Whole numbers
Examples:
5
-2
100
2️⃣ float (real numbers)
Numbers with decimal
3.14
2.0
-0.5
3️⃣ bool (Boolean)
Only 2 values:
True
False
4️⃣ NoneType
Special value:
None

👉 Means: “no value / empty”

🔹 Important line (from slide)

type() tells type of object

Example:
type(5)      # int
type(3.0)    # float
type(True)   # bool
type(None)   # NoneType
x = 5
print(float(x))   # 5.0

y = 3.7
print(int(y))     # 3

print(str(10))    # "10"
Important concept (VERY IMPORTANT)

Python does NOT always convert automatically.

❌ This gives error:
5 + "3"

👉 because:

int + string ❌
✅ Fix using conversion:
5 + int("3")

👉 Output:

8



March -25- 2026
1. “Why give names to values?”

👉 Answer:

To store values and reuse them easily

Instead of writing numbers again and again, we use variables (names).

Example from your notes:
pi = 3.14159
radius = 2.2
area = pi * (radius ** 2)

👉 Meaning:

pi, radius, and area are variables
They store values
