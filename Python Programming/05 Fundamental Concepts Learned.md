
# Core Programming Concepts Behind the Examples

In the previous section, you wrote simple programs and practiced solving a few problems. Now, let's slow down a little and understand the **core programming concepts** behind those examples — this will help you write your own programs much more easily!

We'll use the same familiar examples you have already seen, so it will feel natural.

---

## 1. Variables and Values

In Python, a **variable** is simply a name you give to a piece of information you want to store.  
A **value** is the actual information stored in that variable.

When you write:
```python
length = 10
width = 6
```
- `length` and `width` are variable names.
- `10` and `6` are the values assigned to them.

Think of it like this:  
```
Variable (length)  <--  Value (10)
Variable (width)   <--  Value (6)
```

---

### Assignment Operation — A Deeper Look

The `=` symbol is called the **assignment operator**. It connects the variable name to the value you want to store.

There are a few important things to know:

- You can **assign a value directly**, like:
  ```python
  temperature = 37
  ```
- Or you can **assign the result of an operation**, like:
  ```python
  perimeter = 2 * (length + width)
  ```
  Here, the right-hand side (RHS) `2 * (length + width)` is **calculated first**, and then the final result is assigned to `perimeter`.

- **No need to define variable types beforehand**:  
  In Python, you don't have to declare if a variable will hold a number or text. Python figures it out automatically.

- **Longer expressions on the RHS**:  
  Sometimes the right-hand side becomes bigger. Always **resolve the right-hand side first** (mentally or by breaking into steps), and then think about what final value is being assigned to the variable on the left.

- **Variables can update themselves**:  
  Later, you might see expressions like:
  ```python
  x = x + 10
  ```
  This simply means: "Take the current value of `x`, add `10` to it, and store the new value back into `x`."

All of this makes variables extremely powerful — they grow and change as your program runs!

---

## 2. Operators

An **operator** is a symbol that tells Python to perform some operation between two or more values.

The examples you saw earlier mostly used **arithmetic operators**:

| Operator | Meaning        | Example               | Result  |
|:--------:|:---------------|:----------------------|:-------:|
| `+`      | Addition        | `3 + 2`                | `5`     |
| `-`      | Subtraction     | `5 - 2`                | `3`     |
| `*`      | Multiplication  | `4 * 3`                | `12`    |
| `/`      | Division        | `10 / 2`               | `5.0`   |

### A bigger picture: Other Types of Operators

Python has many other types of operators too, which you will explore gradually.

Here’s a small preview:

| Type of Operator | Purpose                             | Example |
|:-----------------|:------------------------------------|:--------|
| Assignment        | Store a value in a variable         | `a = 5` |
| Arithmetic        | Perform math operations             | `b + c` |
| Comparison        | Compare two values (true/false)     | `x > y` |
| Logical           | Combine multiple conditions         | `x > 5 and y < 10` |

**Practical examples**:
```python
is_adult = age > 18          # Comparison operator (>)
can_vote = is_adult and citizen  # Logical operator (and)
```

For now, just remember: **operators help us create expressions** that do some meaningful work!

---

## 3. Functions – Understanding `print()`

A **function** is like a mini-program built into Python, ready to perform a specific task when you call it.

The first function you are using is `print()` — it **displays information on the screen**.

Example:
```python
print("The perimeter is:", perimeter, "units")
```

Inside `print()`:
- Strings like `"The perimeter is:"` are shown exactly as they are.
- Variables like `perimeter` show their current value.
- Commas `,` are used to separate multiple items — Python adds spaces automatically between them.

---

### Some important points about functions:
- **Functions always use round brackets `()`** in Python.
- **Functions are built for a specific purpose** — like printing, adding numbers, checking conditions, etc.
- **Many built-in functions exist** in Python.  
  Some examples are:
  - `print()` — display something
  - `len()` — find the length of something (like how many letters in a word)
  - `type()` — check what type of value (number, text, etc.)

**Example**:
```python
name = "Alex"
print(len(name))    # Shows: 4
```

As you move forward, you will learn how to use many more functions, and even how to **create your own functions**!

---

# Summary

In every program you wrote earlier, three powerful ideas were working together:
- **Variables**: to store values,
- **Operators**: to perform calculations,
- **Functions**: to carry out specific actions (like printing results).

The better you understand these basics, the easier and more fun programming becomes!

---

✅ **Next Steps**:
- Try defining your own variables and performing calculations.
- Play with different operators.
- Explore using more functions like `len()` and `type()`.

---
