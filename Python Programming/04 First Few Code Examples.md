# 🧮 Getting started with simple arithmetic programs in Python

### 👋 Welcome !

As someone just starting out with Python, you might be wondering:

> “What can I actually do with Python now that I’ve just begun my journey?”

That’s a very valid question — and one that every new learner has asked at some point.  
Often, what holds beginners back is not the complexity of programming, but the **lack of immediate, meaningful application**.

So, let’s change that — right here, right now.

---

## 🎯 Why start with simple arithmetic programs?

- ✅ They’re easy to understand
- ✅ You’ve already done them before — just not using code
- ✅ You’ll see immediate results
- ✅ They help you practice writing variables, taking input, and using operators
- ✅ Most importantly — they’re **relatable** and **motivating**

These early wins, though simple, will give you confidence and purpose.  
And the moment you run your own code and see it working — that’s when you’ll realize: *“Hey, this is something I can do.”*

---

## 🛠️ Let’s build your first few programs

Each example below covers a **tiny real-world task** — something you’d usually do with pen-and-paper or a calculator. But now, **you’ll solve it using Python.**

### 🧮 Example 1: Area of a Rectangle

```python
# We want to find the area of a rectangle
# Let's say the length is 5 meters and width is 3 meters

length = 5
width = 3
area = length * width

print("The area of the rectangle is:", area, "square meters")
```

---

### 💰 Example 2: Simple Interest Calculation

```python
# We want to find the simple interest on a bank deposit
# Principal amount = 2000, rate = 5%, time = 3 years

principal = 2000
rate = 5
time = 3

simple_interest = (principal * rate * time) / 100

print("The simple interest is:", simple_interest)
```

---

### 📊 Example 3: Average of Four Numbers

```python
# Let's calculate the average of four subjects scores: 72, 85, 90, 78

Science = 72
English = 85
Mathematics = 90
Socialscience = 78

total = Science + English + Mathematics + Socialscience
average_score = total / 4

print("The average score is:", average_score)
```

---

### 📅 Example 4: Calculate Age from Birth Year

```python
# Suppose the current year is 2025 and a person was born in 2000

current_year = 2025
birth_year = 2000

age = current_year - birth_year

print("The person's age is:", age, "years")
```

---

### 🛒 Example 5: Total Cost of Grocery Items

```python
# We bought 3 apples (Rs. 20 each), 2 loaves of bread (Rs. 30 each), and 1 bottle of milk (Rs. 50)

apples = 3 * 20
bread = 2 * 30
milk = 1 * 50

total_cost = apples + bread + milk

print("The total cost of groceries is Rs.", total_cost)
```

---

## 🧭 So, what did you actually do here?

Let’s pause for a moment.

You just went through a bunch of small programs — calculating interest, averaging marks, working out grocery bills. On the surface, they might seem basic, but underneath, something important has already started.

You’ve taken your first steps into programming — and whether you realized it or not, you’ve already used some of its core building blocks:

- You **declared variables** — you created names like `length`, `rate`, `total_cost`, and used them to store values  
- You used **arithmetic operators** like `+`, `-`, `*`, and `/` to perform calculations  
- You used the `print()` command to **display results** — which, by the way, is actually a function (we’ll get to functions later)

And you did all of this in actual code — not in theory, not just watching someone else do it, but by *writing and running programs yourself*.

That’s a solid first milestone.

---

## 🔍 What this tells us about programming

Here’s something important to understand early on:

Programming is not about doing complicated things from day one — it's about learning how to break down simple problems, solve them in small steps, and **translate your thought process into code**.

At this point, you’ve done that. You may not know all the right words for it yet (we haven’t covered what a "statement" or "function" really means), but you've started using these ideas. And that’s how people learn — by doing things first, and understanding them more deeply as they go.

---

## 🔜 Where we go from here

Next, we’ll slow things down and go deeper into the **"what" and "why"** of the things you just used.

- What exactly is a **variable**, and why do we need to name things?
- What are **operators**, and what kinds are there beyond just math ones?
- What is the `print()` command really doing behind the scenes?
- And what else makes up a basic program — things like **keywords**, **comments**, **assignment**, and the overall flow?

We’ll take each of these up in small, focused chunks so you get both clarity and confidence.

---

## 👣 One step at a time

One last thing: it’s okay if some parts still feel fuzzy right now.

The goal here isn’t to master everything in one go. The goal is to *build a rhythm* — try something, understand a bit, try again, learn more. Programming is a skill that grows over time, with practice and patience.

So keep going. Explore, edit, break things, fix them again — that’s how learning sticks.

You’re doing just fine.

We’ll pick it up from here next — and unpack everything you’ve touched so far, one concept at a time.

---
---
---

## 🧩 Try it yourself: Five simple programming exercises

Here are five small programming tasks to help you practice what you've just learned.  
- Each one involves working with variables, basic arithmetic operations, and using the `print()` function to display the result.  
- Use the provided values (or experiment with your own) and validate the final output that your code generates

---

### 1. Calculate the perimeter of a rectangle  
```python
# Write a program to calculate the perimeter of a rectangle with a length of 10 and a width of 6. 
# Use the formula: perimeter = 2 * (length + width), and display the result as: 
# "The perimeter of the rectangle is: 32 units".

# ---- write your code here ----

```
---

### 2. Convert temperature from Celsius to Fahrenheit
```python
# Write a program that converts 37 degrees Celsius to Fahrenheit using the formula: 
# Fahrenheit = (Celsius × 9/5) + 32. Display the result as: 
# "37 degrees Celsius is equal to 98.6 degrees Fahrenheit".

# ---- write your code here ----
```
---

### 3. Calculate total marks, percentage, and print a summary
```python
# Write a program that calculates the total marks and percentage for five subjects 
# with scores 80, 76, 91, 85, and 88. The total is the sum of all marks, 
# and the percentage is calculated as (total / 500) * 100. 
# Display both total and percentage clearly.

# ---- write your code here ----
```
---

### 4. Calculate overall average speed
```python
# A vehicle travels 40 km in 1 hour, 60 km in 1.5 hours, and 30 km in 0.5 hours. 
# Write a program to calculate the total distance, total time, and the overall average speed 
# using: average_speed = total_distance / total_time. 
# Display all three values in a readable format.

# ---- write your code here ----
```
---

### 5. Compute CGPA across two semesters
```python
# A student scored a GPA of 7.8 in Semester 1 with 24 credits, and a GPA of 8.4 in Semester 2 with 28 credits. 
# Write a program to compute the CGPA across both semesters using the formula: 
# CGPA = (GPA1 × credits1 + GPA2 × credits2) / (credits1 + credits2). 
# Display the final CGPA as: "The overall CGPA is: 8.13".

# ---- write your code here ----
```
