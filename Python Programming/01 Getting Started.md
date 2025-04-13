# Where to write codes - Accessing an Online Platform

---

## 📌 Overview

One of the biggest roadblocks beginners face when learning Python is getting stuck in the **technical steps of downloading, installing, and setting up a coding environment**. For many, this becomes a barrier rather than a motivation. And honestly, it doesn’t have to be that way.

When I first started out, my biggest question was simple:  
**"Where do I even write Python code?"**

I read countless articles, watched a bunch of tutorials, and by the time I finally reached the right platform to try coding, the initial excitement had already faded. That delay — just getting started — was enough to slow me down.

That’s why this page begins with something different.  
Before we dive into learning Python, I want to **show you how quick and easy it is to access a coding platform** — no downloads, no complicated setup. Just open, type, and run.

As a beginner, it’s completely okay if you don’t know whether to call it a *platform*, a *tool*, or an *application*. What matters most is this: **you take your first step**.  

This guide will help you get a **first-hand experience** with a few beginner-friendly online platforms that let you write and run Python code — right from your browser.

👉 Once you get comfortable here and you're still curious to learn more (which I’m sure you will be!), we’ll move on to setting up Python on your own system — and I’ll guide you every step of the way.

So take a deep breath, leave the fear behind, and let’s begin!

---

## 🌐 Google Colab – The Preferred Choice

**Google Colab** is an online notebook where you can write and run Python code directly from your browser. It’s free to use and requires **no installations or setup**.

### ✅ What You Need:
- A **Google account** (like Gmail)
- A browser (Chrome, Firefox, Edge, etc.)

### 🚀 How to Get Started:
1. Visit 👉 [https://colab.research.google.com/](https://colab.research.google.com/)
2. If prompted, sign in with your Google account.
3. Click on the **"New Notebook"** button (usually found at the bottom-right or left corner).
4. A new page will open with a code cell ready to go!

### ✨ Why Colab is a Great Starting Point:
- No setup hassles — you can start coding instantly.
- Runs on the cloud, so no need for a powerful computer.
- You can save your notebooks directly to your Google Drive.

---

## 🌐 Jupyter.org – Another Beginner-Friendly Option

Another excellent way to explore Python online is through **Jupyter.org**.

### 🚀 How to Try It:
1. Visit 👉 [https://jupyter.org/try](https://jupyter.org/try)
2. Click on the **“Try Notebook”** option (you may also try "Jupyter Lab").
3. Wait a few seconds — a free, temporary notebook will open.
4. Click on **File > New > Notebook**, and select Python (usually Python 3).

That’s it! You’re now in a live Python notebook ready to write your first code.

---

## 👨‍💻 Let’s write and Run your First Python Code!

Copy the following code and paste it in **either Google Colab or Jupyter Notebook**:

```python
name = input("What is your name? ")
print(f"Hello, {name}! Welcome to your first Python session.")
```
---

### ▶️ How to Run the Code

Here’s how you can execute your first Python code on both platforms:

**🔹 On Google Colab**
- Click inside the code cell
- Press `CTRL + Enter` on your keyboard

**🔹 On Jupyter Notebook (via jupyter.org)**
- Click the code cell to select it
- Press `CTRL + Enter` to run it

💡 After you press `CTRL + Enter`, the cell will execute, and a prompt (a dialogue box) will appear asking for your input - .i.e., Your Name. Once you write your name and hit `Enter` you’ll see the code output just below the code. 

Again, the intention here is not to fully understand what is going on with the code, rather the idea is to get an initial first-hand experience of code running in an Online Platform !

---


### 🧭 What’s Next?

Now that you've taken your **first step into Python programming** by writing and running code online, here’s what you can do next:

## 🧪 Try these practical examples

These examples show how you can use Python to solve simple, everyday tasks. They also give you a chance to interact with Python by providing inputs, which is great for learning.

---

### ✅ Example 01: Find the Perimeter of a Rectangle

```python
# This example calculates the perimeter of a rectangle.
# The user is asked to input the length and width of the rectangle.

length = float(input("Enter the length of the rectangle: "))  # Taking length input from the user
width = float(input("Enter the width of the rectangle: "))    # Taking width input from the user

# Calculate the perimeter
perimeter = 2 * (length + width)

# Print the result
print("The perimeter of the rectangle is:", perimeter)
```

### ✅ Example 02: Print the Table of a Number

```python
# This example prints the multiplication table of a number.
# The user is asked to input the number for which they want the table.

number = int(input("Enter a number to print its multiplication table: "))

# Print the multiplication table
print("Multiplication Table for", number)
for i in range(1, 11):  # Loop from 1 to 10
    print(number, "x", i, "=", number * i)
```

### ✅ Example 03: Check if a Number is Prime

```python

# This example checks if a given number is a prime number.
# The user is asked to input the number they want to check.

number = int(input("Enter a number to check if it's prime: "))

# Prime number check
if number > 1:
    for i in range(2, number):
        if number % i == 0:
            print(number, "is not a prime number.")
            break
    else:
        print(number, "is a prime number.")
else:
    print(number, "is not a prime number.")

```
---

### 🔁 **Keep experimenting**  
The more you play around with code, the more comfortable you’ll become. Try changing parts of the code, experiment with different inputs, and don’t be afraid to make mistakes. Every time you tweak something, you’re learning.

### 🤹 **Don’t be afraid to make mistakes**  
Mistakes are a vital part of the process! They’re how you grow and understand the logic behind the code. Keep going, and with each mistake, you’ll come out stronger and more knowledgeable.

### 🌟 **What’s next?**  
Once you're comfortable with writing and testing code online, it’s time to take the next big step:  
👉 **Setting up Python on your own computer** (offline). This is where an IDE (Integrated Development Environment) comes into play — something we'll guide you through in the next lesson.

---

> 💡 *The journey to mastering coding is all about practice. Keep coding, exploring, and learning from your mistakes.*

> ✨ *Remember, every expert started exactly where you are now. The first line of code you write is the start of your journey — keep moving forward!*  

---
