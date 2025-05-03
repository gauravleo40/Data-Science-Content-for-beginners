# 01. Variables recap

By now, you've already learned how **variables** are an important concept in Python. They let us store values, use them again and again, and make our code easier to work with.

But as you move ahead, you’ll see that while variables are very useful, they are not enough in every situation — especially when you have to handle a lot of related information at once.

Before we go into that, let’s take one more real-life example to understand how variables can really help us.

---

## 📌 Example: printing a multiplication table

Let’s say you want to print the multiplication table of a number, like 7. Here’s one way to write that using a variable:

```python
N = 7

print(N, 'x 1 =', N * 1)
print(N, 'x 2 =', N * 2)
print(N, 'x 3 =', N * 3)
print(N, 'x 4 =', N * 4)
print(N, 'x 5 =', N * 5)
print(N, 'x 6 =', N * 6)
print(N, 'x 7 =', N * 7)
print(N, 'x 8 =', N * 8)
print(N, 'x 9 =', N * 9)
print(N, 'x 10 =', N * 10)
````
*Note that the print() function is used very smartly here by declaring multiple arguments in it:*
- First the variable `N`
- Second the string `x ... = `
- Third a computation on the variable `N`, i.e., `N * ...`

---
Here, it might have take us some time to write all these code lines, but this is just a one-time effort. By using the variable `N` we have saved the time and effort for generating a Table for some other value of `N`, let's say 12

```python
N = 12  # That’s it! The rest of the code stays the same.
```

⚠️ **Now imagine NOT using a variable at all.** You would have to write the number `7` in all 10 lines. And if you later want to print the table of `12`, you’d have to change every line by hand. That’s a lot of extra work whenever the value of `N` needs to be changed. Also it’s easy to make mistakes while making these multiple changes eveytime

> 💡 **Note from a more experienced programmer:** A better way to write this code is by using `for` or `while` loops in Python — something you’ll learn very soon. But even this small example shows how one variable can make your life easier.

---
---


# 02. Variables have their limits

You’ve seen how variables make your code flexible. But what if you have to work with **many related values** — like monthly expenses, exam scores, or daily temperatures?

Let’s walk through an everyday situation and see where variables start to struggle.

---

## 📌 Real-world example: Tracking monthly expenses

Say you’re trying to keep track of how much you spent in the first 5 months of the year.

As a beginner you might approach it like this:

```python
jan_expense = 12000
feb_expense = 15000
mar_expense = 10000
apr_expense = 11000
may_expense = 13000
````

So far, so good — the numbers are stored.

Now you want to calculate your **total spending**:

```python
total_expense = jan_expense + feb_expense + mar_expense + apr_expense + may_expense
print("Total expenses so far:", total_expense)
```

Yes, this works. But let's pause and think — what happens if you now want to:

* Add June, July, and more months?
* Calculate the average monthly expense?
* Compare each month’s expense to a budget limit?

Suddenly, your code becomes longer and harder to manage.

---

## ⚠️ What makes this a problem?

Let’s look at the issues one by one:

* **Too many variables**: You're forced to create separate variables for each month. That’s okay for 5, but terrible for 12 or more.

* **Tedious calculations**: Each time you want to calculate a total or average, you have to write all the variable names one by one.

  Imagine doing this:

  ```python
  average = (jan_expense + feb_expense + mar_expense + apr_expense + may_expense) / 5
  ```

  ...and later needing to change it when June is added.

* **Naming overload**: Coming up with variable names for each data point takes time. Also, you need to be creative in thinking of meaningful names for each variable

* **Scalability drops**: Your logic becomes harder to extend and maintain. What if you wanted to store last year’s expenses too?

---

> 💡 Mentor tip:
>  - This is a **classic case** where we are storing many related values that share a similar meaning — **monthly expenses** — but using individual variables makes the code heavy and harder to modify. That’s not ideal.
>  - As a developer, you don’t just want working code — you want code that’s clean, short, and ready to grow. If you’re repeating yourself or juggling too many variable names, that’s a sign you need to level up your data-handling skills.

---

## 🚧 A better way is coming…

What you really want is:

* A way to store **multiple values under one name**.
* A way to calculate totals, averages, minimum and maximum values easily.
* Something that keeps your code short and simple.

And that’s exactly what **data structures** in Python allow you to do.

---
---

# 03. A better way to store multiple values — First step toward data structures

In the last example, you saw how storing monthly expenses using separate variables became time-consuming and hard to manage.

Let’s now try a different style — something that helps us group all those values together in one go.

---

### 🌱 A smarter way to store multiple values

If we list all the monthly expense values separated by commas and assign them to a single variable, Python stores them as a **collection** of multiple data points.

Here’s how it looks:

```python
monthly_expenses = 12000, 15000, 10000, 11000, 13000
````

This is different from what you’ve done earlier where a variable held just **one** value. Now, the same variable is holding **five** values at once — like a bundle or a **Data Container**

Python recognizes this collection as something called a **tuple** — which is just one kind of *data structure*. Don’t worry about that term **Tuple** for now — just focus on what it allows you to do.

---

### ✅ What can we do with this?

This new way of storing data makes many operations simpler and less error-prone.

---

#### ➕ Total monthly expense

```python
total = sum(monthly_expenses)
print("Total Expense:", total)
```

**Output:**

```
Total Expense: 61000
```

Compare this with the earlier approach, where we had to manually add Five different variables. This is clearly more convenient.

---

#### 📊 Average monthly expense

```python
average = sum(monthly_expenses) / 5

# or

average = sum(monthly_expenses) / len(monthly_expenses)
print("Average Monthly Expense:", average)
```

**Output:**

```
Average Monthly Expense: 12200.0
```

You can now do this without repeating all the variable names or rewriting long expressions.

---

#### 🔍 Maximum and Minimum expenses

```python
print("Highest Expense in a Month:", max(monthly_expenses))
print("Lowest Expense in a Month:", min(monthly_expenses))
```

**Output:**

```
Highest Expense in a Month: 15000
Lowest Expense in a Month: 10000
```

No need to search manually — the structure we used allows Python to help us out.

---

### 💡 What just happened?

By storing multiple values as a collection:

* We have been able to manage information well - since we are keeping multiple data points together in a data container and calling it by a single name
* We now have the ability to perform useful operations on these multiple data points by using Pyton's builtin functions : `sum(), max(), min()`. The coding effort has gone down significantly in doing so.
* Since we are no more writing lengthy expressions involving multiple variables names , the chances of making manual errors has been greatly reduced

You should be able to clearly see how we have moved **from writing more code** to writing **better code**.

---

### 🎯 A quick recap

* **Variables** are still the best tool when we need to store **a single value**.
* But when we have **multiple related values**, it’s much better to use a **data structure** like the one we just used.
* What we used here is a **tuple**, and it gave us our first taste of how powerful this new concept can be.

In the next part of your learning journey, we’ll formally explore what **data structures** are, why they matter, and how many different types Python offers to help us store and process data in the real world.

You’ve just taken a mature step toward becoming a thoughtful programmer. Keep going — it gets more interesting from here! 🚀

