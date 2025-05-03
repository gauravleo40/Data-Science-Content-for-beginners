# Variables are good but what comes next?

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

🟡 **Now imagine NOT using a variable at all.** You would have to write the number `7` in all 10 lines. And if you later want to print the table of `12`, you’d have to change every line by hand. That’s a lot of extra work whenever the value of `N` needs to be changed. Also it’s easy to make mistakes while making these multiple changes eveytime

> 💡 **Note from a more experienced programmer:** A better way to write this code is by using `for` or `while` loops in Python — something you’ll learn very soon. But even this small example shows how one variable can make your life easier.

---
