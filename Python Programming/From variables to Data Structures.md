# Variables are good but what comes next?

By now, you've already learned how **variables** are one of the first and most important things in Python. They let us store values, use them again and again, and make our code easier to work with.

But as you move ahead, you’ll see that while variables are very useful, they are not enough in every situation — especially when you have to handle a lot of related information at once.

Before we go into that, let’s take one more real-life example to understand how variables can really help us.

---

## 📌 Example: Printing a Multiplication Table

Let’s say you want to print the multiplication table of a number, like 7. Here’s one way to write that using a variable:

*Note that the print() function is used very smartly here by declaring multiple arguments in it:*
- First the variable `N`
- Second the string `x .. = `
- Third a computation on the variable `N`

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

Here, the variable `N` is used again and again in every line. That’s the beauty of using variables — you write less code, and you can change things easily.

🟡 **Now imagine not using a variable at all.** You would have to write the number `7` in all 10 lines. And if you later want to print the table of `9`, you’d have to change every line by hand. That’s a lot of extra work, and it’s easy to make mistakes.

---

> 💡 **Note from a senior programmer:** A better way to write this is by using a `for` loop — something you’ll learn very soon. But even this small example shows how one variable can make your life easier.

So even if it takes a few minutes to set it up, the time you save later is worth it. For example, to print the table of 12, you only need to change one line:

```python
N = 12  # That’s it! The rest of the code stays the same.
```

---

This shows you how useful variables are when building programs. But there’s one more thing you should know — what if you need to store **many values**, like the marks of 50 students or the sales from 30 days?

Typing 50 different variable names will be a nightmare. And that's where variables reach their limit.

Let’s move on and see what we should learn next.

```

---

Let me know when you’re ready to build the **next part**, where we explain *why variables are not enough* and introduce **data structures** as the next logical step.
```
